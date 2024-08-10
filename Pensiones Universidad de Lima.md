---
creado: 2024-04-25 10:39
modificado: 2024-04-25 10:39
share: "true"
---

# Pensiones Universidad de Lima
## 1. Modelos de request:

```html
https://webaloe.ulima.edu.pe/portalUL/cc/servlets/ComandoListarRecibosAlumnosIngresantesSinValidacion?cicloPS=3185&cicloUL=20241&IndNuPaso=&colegio3=94&colegio4=94&colegio5=94&coCole5=94
https://webaloe.ulima.edu.pe/portalUL/cc/servlets/ComandoListarRecibosAlumnosIngresantesSinValidacion?cicloPS=3185&cicloUL=20241&IndNuPaso=&colegio3=358&colegio4=358&colegio5=358&coCole5=358
```

## 2. Datos de la solicitud de buscar colegio

```html
<!-- Departamentos -->

<option value="-1"> - - - - Seleccione - - - - </option><option value="01">AMAZONAS</option><option value="02">ANCASH</option><option value="03">APURIMAC</option><option value="04">AREQUIPA</option><option value="05">AYACUCHO</option><option value="06">CAJAMARCA</option><option value="07">CALLAO</option><option value="08">CUSCO</option><option value="09">HUANCAVELICA</option><option value="10">HUANUCO</option><option value="11">ICA</option><option value="12">JUNIN</option><option value="13">LA LIBERTAD</option><option value="14">LAMBAYEQUE</option><option value="15">LIMA</option><option value="16">LORETO</option><option value="17">MADRE DE DIOS</option><option value="18">MOQUEGUA</option><option value="19">PASCO</option><option value="20">PIURA</option><option value="21">PUNO</option><option value="22">SAN MARTIN</option><option value="23">TACNA</option><option value="24">TUMBES</option><option value="25">UCAYALI</option>

<!-- Provincias -->
					
		<option value="-1"> - - - - Seleccione - - - - </option><option value="02">BARRANCA</option><option value="05">CAÑETE</option><option value="03">CAJATAMBO</option><option value="04">CANTA</option><option value="06">HUARAL</option><option value="07">HUAROCHIRI</option><option value="08">HUAURA</option><option value="01">LIMA</option><option value="09">OYON</option><option value="10">YAUYOS</option>

<!-- Distritos -->


					
		<option value="-1"> - - - - Seleccione - - - - </option><option value="02">ANCON</option><option value="03">ATE</option><option value="04">BARRANCO</option><option value="05">BREÑA</option><option value="06">CARABAYLLO</option><option value="07">CHACLACAYO</option><option value="08">CHORRILLOS</option><option value="09">CIENEGUILLA</option><option value="10">COMAS</option><option value="11">EL AGUSTINO</option><option value="12">INDEPENDENCIA</option><option value="13">JESUS MARIA</option><option value="14">LA MOLINA</option><option value="15">LA VICTORIA</option><option value="01">LIMA</option><option value="16">LINCE</option><option value="17">LOS OLIVOS</option><option value="18">LURIGANCHO</option><option value="19">LURIN</option><option value="20">MAGDALENA DEL MAR</option><option value="22">MIRAFLORES</option><option value="23">PACHACAMAC</option><option value="24">PUCUSANA</option><option value="21">PUEBLO LIBRE</option><option value="25">PUENTE PIEDRA</option><option value="26">PUNTA HERMOSA</option><option value="27">PUNTA NEGRA</option><option value="28">RIMAC</option><option value="29">SAN BARTOLO</option><option value="30">SAN BORJA</option><option value="31">SAN ISIDRO</option><option value="32">SAN JUAN DE LURIGANCHO</option><option value="33">SAN JUAN DE MIRAFLORES</option><option value="34">SAN LUIS</option><option value="35">SAN MARTIN DE PORRES</option><option value="36">SAN MIGUEL</option><option value="37">SANTA ANITA</option><option value="38">SANTA MARIA DEL MAR</option><option value="39">SANTA ROSA</option><option value="40">SANTIAGO DE SURCO</option><option value="41">SURQUILLO</option><option value="42">VILLA EL SALVADOR</option><option value="43">VILLA MARIA DEL TRIUNFO</option>

```

## 3. Abrir buscador

```html

<!-- Buscado -->

https://webaloe.ulima.edu.pe/portalUL/gaad/pp/seleccionarColegio.jsp?CodVentana=SP&hdnCodigoColegio=coCole5&txtNombreColegio=txtQuintoSecundaria&ciclo=20241

<!-- DEvuelve tabla con códigos de colegios -->

https://webaloe.ulima.edu.pe/portalUL/gaad/pp/servlets/ComandoListarColegiosPP?txtNombreColegio=juan&CodDpto=15&CodProv=01&CodDist=01&TC=&ciclo=20241

```

A este buscado se pasan los datos y devuelve lista:

 - txtNombreColegio:	JUAN
 - CodDpto: 	15
 - CodProv	01
 - CodDist 	01
 - TC: vacío
 - ciclo: 20241

Esto devuelve 2 tablas (1 header, 2 el contenido),  de la segunda tabla donde hay que sacar los códigos de colegios y los nombres.

![[Pasted image 20240425110256.png|Pasted image 20240425110256.png]]

```html
<!-- Este es el ancla de donde hay que sacar los datos -->

<a href="javascript:seleccionarColegio('1374', 'ALEJANDRO SANCHEZ ARTEAGA (LIMA / LIMA / LIMA - LIMA)');"><img src="/portalUL/images/gaad/pp/IconoSeleccionar.gif" width="16" height="16" border="0" alt="Seleccionar"></a>

-->

```

Del ancla se saca el código y el nombre, con el código se realiza el request del punto 1.

Convert this JS code https://server1.torreblanca.pe/PPColegios.js this code create 9 array and populate them. Convert this 9 array in a R dataframe where every array is one variable of the dataframe.

### GTP
```r
# Load the JS code into R
js_code <- readLines("PPColegios.js")

# Extract the array data from the JS code
arrays <- str_extract_all(js_code, "var (.+?) = \\[(.+?)\\];")

# Create a data frame from the arrays
df <- data.frame(map(arrays, function(x) {
  # Convert the array string to a vector
  vec <- str_split(x[2], ",")[[1]]
  
  # Convert the vector to a numeric vector
  as.numeric(vec)
}))

# Name the variables in the data frame
names(df) <- arrays[[1]][1]
```
## Referencias
1. 

