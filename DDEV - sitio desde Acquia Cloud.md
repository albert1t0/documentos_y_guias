---
share: "true"
---
DDEV es una excelente herramienta para desarrollar sitios Drupal localmente, y puedes usarla para levantar tu sitio existente con su código, base de datos y archivos (assets) de manera sencilla. A continuación, te guío paso a paso para configurar DDEV con tu proyecto Drupal, asumiendo que ya tienes el código fuente (incluyendo el archivo composer.json), la base de datos exportada y los archivos subidos (como los de sites/default/files). Si algo no está claro o necesitas ajustes específicos, no dudes en decírmelo.

---

Requisitos previos

1. Instalar DDEV: Asegúrate de tener DDEV instalado en tu máquina. Si no lo tienes, sigue las [instrucciones oficiales](https://ddev.readthedocs.io/en/stable/users/install/ddev-installation/) según tu sistema operativo (Windows, macOS o Linux). Necesitarás Docker como dependencia.
    
2. Código fuente: Tienes el código de tu sitio Drupal (descargado desde Acquia Cloud o tu repositorio Git).
    
3. Base de datos: Tienes un archivo SQL exportado (por ejemplo, backup.sql) de tu base de datos de Acquia.
    
4. Archivos subidos: Tienes la carpeta de assets (como sites/default/files) descargada de Acquia.
    
5. Composer: Tu proyecto incluye un archivo composer.json y, idealmente, el directorio vendor/ o estás dispuesto a regenerarlo.
    

---

Paso 1: Preparar el directorio del proyecto

1. Crea un directorio para tu proyecto (si no lo tienes ya):
    
    bash
    
    ```bash
    mkdir mi-sitio-drupal
    cd mi-sitio-drupal
    ```
    
2. Copia el código fuente: Mueve o clona el código de tu sitio Drupal dentro de este directorio. Por ejemplo:
    
    - Si lo descargas de un repositorio Git (como el de Acquia):
        
        bash
        
        ```bash
        git clone <URL_DEL_REPOSITORIO> .
        ```
        
    - O si tienes una carpeta comprimida, descomprímela aquí.
        
3. Verifica la estructura: Asegúrate de que el directorio contenga composer.json, web/ (donde está el núcleo de Drupal), y otros archivos típicos de un proyecto Drupal.
    

---

Paso 2: Configurar DDEV

1. Inicializar DDEV: En el directorio raíz de tu proyecto, ejecuta:
    
    bash
    
    ```bash
    ddev config
    ```
    
    DDEV te hará unas preguntas:
    
    - Project name: Ingresa un nombre (por ejemplo, mi-sitio-drupal). Esto define la URL local (como mi-sitio-drupal.ddev.site).
        
    - Docroot: Especifica la carpeta que contiene el núcleo de Drupal. Si usas una estructura moderna con Composer, suele ser web/. Si es un Drupal más antiguo, podría ser . (raíz).
        
    - Project type: Selecciona drupal (DDEV detectará automáticamente la versión: Drupal 7, 8, 9 o 10). Presiona Enter para aceptar los valores predeterminados cuando sea aplicable.
        
    
    Ejemplo de salida:
    
    ```text
    Project name (mi-sitio-drupal): mi-sitio-drupal
    Docroot Location (web): web
    Project Type [drupal10, drupal7, drupal8, drupal9] (drupal10): drupal9
    ```
    
2. Resultado: DDEV creará un archivo .ddev/config.yaml con la configuración básica.
    

---

Paso 3: Instalar dependencias con Composer

1. Ejecuta Composer: Si tu proyecto no incluye el directorio vendor/ (porque lo excluiste del repositorio), usa DDEV para instalar las dependencias:
    
    bash
    
    ```bash
    ddev composer install
    ```
    
    Esto descargará Drupal core, módulos contribuidos y cualquier otra dependencia listada en composer.json.
    
    - Si ya tienes vendor/, puedes omitir este paso.
        
2. Verifica: Asegúrate de que el directorio web/ contenga los archivos necesarios (como core/ y modules/) después de Composer.
    

---

Paso 4: Importar la base de datos

1. Copia el archivo SQL: Coloca tu archivo de base de datos exportado (por ejemplo, backup.sql) en el directorio raíz del proyecto (mi-sitio-drupal/).
    
2. Inicia el entorno DDEV: Levanta los contenedores de Docker:
    
    bash
    
    ```bash
    ddev start
    ```
    
    Esto inicia el servidor web, la base de datos y otros servicios.
    
3. Importa la base de datos: Usa el comando de DDEV para importar el archivo SQL:
    
    bash
    
    ```bash
    ddev import-db --src=backup.sql
    ```
    
    - Si el archivo está comprimido (por ejemplo, backup.sql.gz), DDEV lo manejará automáticamente:
        
        bash
        
        ```bash
        ddev import-db --src=backup.sql.gz
        ```
        
    - DDEV creará una base de datos predeterminada llamada db y la llenará con los datos del archivo.
        

---

Paso 5: Copiar los archivos subidos (assets)

1. Ubicación de los archivos: En Drupal, los archivos subidos suelen estar en web/sites/default/files/ (o una ruta personalizada definida en settings.php).
    
2. Copia los archivos: Mueve tu carpeta de assets descargada desde Acquia a la ubicación correcta. Por ejemplo:
    
    bash
    
    ```bash
    cp -r /ruta/a/tus/files/ web/sites/default/files/
    ```
    
3. Ajusta permisos: Asegúrate de que los archivos sean escribibles por el servidor web:
    
    bash
    
    ```bash
    chmod -R 775 web/sites/default/files
    chown -R $(whoami):www-data web/sites/default/files  # En Linux/macOS
    ```
    

---

Paso 6: Configurar settings.php

1. Verifica la configuración: Abre web/sites/default/settings.php y asegúrate de que las credenciales de la base de datos coincidan con las de DDEV. Por defecto, DDEV usa:
    
    - Host: db
        
    - Database: db
        
    - Username: db
        
    - Password: db Ejemplo:
        
    
    php
    
    ```php
    $databases['default']['default'] = [
      'database' => 'db',
      'username' => 'db',
      'password' => 'db',
      'host' => 'db',
      'port' => '3306',
      'driver' => 'mysql',
      'prefix' => '',
      'collation' => 'utf8mb4_general_ci',
    ];
    ```
    
    Si tu settings.php tiene configuraciones específicas de Acquia (como conexiones a Memcached o Varnish), coméntalas o elimínalas por ahora.
    
2. Añade ajustes locales: Si necesitas configuraciones específicas para tu entorno local, crea un archivo settings.local.php y haz que se incluya en settings.php:
    
    php
    
    ```php
    if (file_exists(__DIR__ . '/settings.local.php')) {
      include __DIR__ . '/settings.local.php';
    }
    ```
    

---

Paso 7: Levantar y probar el sitio

1. Inicia el sitio: Asegúrate de que DDEV esté corriendo (ddev start).
    
2. Accede al sitio: Abre tu navegador y visita la URL local generada por DDEV, como:
    
    ```text
    https://mi-sitio-drupal.ddev.site
    ```
    
    - DDEV usa HTTPS por defecto con certificados autofirmados.
        
3. Ejecuta comandos de Drupal:
    
    - Limpia la caché:
        
        bash
        
        ```bash
        ddev drush cr
        ```
        
    - Actualiza la base de datos (si es necesario):
        
        bash
        
        ```bash
        ddev drush updb
        ```
        

---

Paso 8: Solucionar problemas comunes

- Error de base de datos: Si la importación falla, verifica que el archivo SQL sea compatible con la versión de MySQL/MariaDB de DDEV (por ejemplo, usa ddev describe para ver la versión).
    
- Módulos faltantes: Si ves errores sobre módulos no encontrados, ejecuta ddev composer install nuevamente o instala módulos específicos con ddev composer require drupal/<modulo>.
    
- Assets no visibles: Si las imágenes o archivos no aparecen, revisa las rutas en settings.php (variable $settings['file_public_path']) y asegúrate de que los permisos sean correctos.
    

---

Ejemplo completo de comandos

bash

```bash
# 1. Preparar el proyecto
mkdir mi-sitio-drupal
cd mi-sitio-drupal
git clone <URL_DEL_REPOSITORIO> .

# 2. Configurar DDEV
ddev config
# Responde: mi-sitio-drupal, web, drupal9 (o tu versión)

# 3. Instalar dependencias
ddev composer install

# 4. Iniciar DDEV
ddev start

# 5. Importar base de datos
ddev import-db --src=backup.sql

# 6. Copiar archivos
cp -r /ruta/a/tus/files/ web/sites/default/files/
chmod -R 775 web/sites/default/files

# 7. Limpiar caché y probar
ddev drush cr
ddev launch
```

---

Conclusión

Con estos pasos, deberías tener tu sitio Drupal de Acquia corriendo localmente con DDEV, incluyendo el código, la base de datos y los assets. Si usabas Acquia Site Studio y quieres mantenerlo, asegúrate de que los módulos de Site Studio estén en composer.json y configurados correctamente. Si tienes problemas específicos (como errores al importar la base de datos o módulos faltantes), compártelos y te ayudaré a resolverlos. ¿Todo claro hasta aquí?