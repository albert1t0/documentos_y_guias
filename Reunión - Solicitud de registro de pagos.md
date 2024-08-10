---
creado: 2022-05-19 09:31
tags:
  - admisión
  - inscripción
share: "true"
---
# Reunión - Solicitud de registro de pagos

## Requerimientos

1. Se necesita realizar el registro de los pagos por las plataformas que ofrece DTI.
2. El posible procedimiento es el siguiente:
	1. Se crea una plataforma de actividad o curso pagado en la plataforma de educación contínua.
	2. En esta se activa la opción de pago.
		- La opción de pago puede ser por tarjeta o por banco.
		- Además, se crea un enlace único de pago de la actividad.
		- Considerar que con enlace único, no se sabe quien realizó el pago.
	3. Se necesita solicitar el registro de los que pagan desde la plataforma de Education CLoud (EC).
		- Para esto se necesitan los datos a registrar en la plataforma creada de educación contínua.
		- Solictar si requeire pagopor banco o con tarjeta.
	4. Luego de confirmado el pago, el que se registra en la plataoforma de educación contínua, es necesario regresar el dato a EC, para que el postulante pueda seguir su proceso de inscripción.
	5. Al finalizar se tendrá ya los datos de los interesados con código F, de candidato PUCP.
		- Esto puede ser bueno ya que el candidato quedaría registrado en el sistema.
		- Pero puede ser un problema para los que ya tengan correos registrados en la PUCP.
		- Además que puede generarse un problema al registrarlos como candidatos en el proceso de admsión en el que deben de participar.
3. Esto se espera hacerlo con RPA (Procesos automatizados por robots) o utilziar una aplicción que procese el requerimiento de registro de los candidatos.
4. Se necesita:
	1. Crear un curso o actividad en Educación Contínua.
	2. Determinar el flujo de registro.
	3. Exportar los datos necesarios desde EC.
	4. Preparar un PA (proceso automatizado) que  registre a los candidatos de esta plantilla
	5. Recuperar la información de pago, sea banco o tarjeta.
	6. Comunicar al candidato que debe de realizar el pago, por mensaje o correo.
	7. Recuperar el estado del pago
	8. Los que hayan sido pagados, deben de registrarse en EC.
	9. Los que aún no se paga, se les debe de apurar. **Enlace de pago solo dura 24 horas**.
5. Las actualizaciones serán programadas:
	1. Se informa a los candidatos que al terminar la revisión de susu documentos se les envía el enlace de pago.
	2. Dos veces al día se descargan los postulantes que aptos para pago.
		- Exporta data de EC validada por **Inscripciones**.
		- Registrarla en plataforma de EC para generar el pago.
		- Se enviuan correos correspondientes.
		- Se verifica el estado de pagos.
		- Se registra en EC el estado del pago.
	3. De igual forma 2 veces al día se actualiza estado de pago en EC.
6. Es necesario considerar el impacto que puede tener este proceso en el registro o inscripción de los candidatos en la plataforma de inscripciones.
7. Crear un proceso de Admisión con las necesidades mínimas para cubrir las necesidades del proceso.
8. _Verificar el impacto que pueda tener el registro de estudiantes_
	- Ver si es posible la carga automática por código F existente.
	- Ver si se puede hacer el registro con herramientas de la PUCP.
	- Finalmente se puede realizar le registro manual con PA.
