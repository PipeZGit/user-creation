# user-creation
App for creating users - Technique Test

Pasos para probar la aplicación:

1. Descarga la carpeta comprimida con el nombre "userscreation" que se encuentra en este repositorio.
2. Descomprime el contenido de la carpeta descargada en el paso 1.
3. Con tu IDE de preferencia (por ejemplo IntelliJ) abre un proyecto existente File - Open - (Seleccionas la carpeta descargada en el paso 2)
4. Corre la aplicación para levantar el servicio, puedes hacerlo dando click derecho en la clase "ProyectoCreacionDeUsuariosApplication" y presionando el botón "Run"
5. Sabras que el servicio esta arriba al ver en la consola de tu IDE un mensaje como este:  "Started ProyectoCreacionDeUsuariosApplication in 3.772 seconds (JVM running for 4.554)"
6. Abre un explorador (ej: Chrome) y digita la siguiente url: http://localhost:8080/swagger-ui.html#/user-controller. Aqui ya podras acceder a los servicios implementados.
7. Para crear usuarios debes utilizar el endPoint llamado "/api/usarios/createUser" y debes hacerlo usando un request con la siguiente estructura de ejemplo:
{
  "email": "diegofz16@gmail.com",
  "name": "Diego Felipe Zapata",
  "password": "passPASS2023",
  "phones": [
    {
      "cityCode": "01",
      "countryCode": "001",
      "number": "3200000000"
    },
	{
      "cityCode": "01",
      "countryCode": "001",
      "number": "3202401918"
    },
	{
      "cityCode": "01",
      "countryCode": "001",
      "number": "3201234567"
    }
  ]
}
8. Una vez hayas creado usuarios podras utilizar los otros endPoints.
9. Para ver la base de datos deberas abrir un nuevo explorador y digitar la siguiente url: "http://localhost:8080/h2-console". El password que debe utilizar es "sa".
