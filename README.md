
🌍 Conversor de Monedas
Este proyecto permite a los usuarios convertir entre diferentes monedas utilizando la API de ExchangeRate-API para obtener tasas de cambio actualizadas.

🛠️ Características
Convertir entre diferentes monedas 💱
Información sobre la última actualización de tasas 🔄
Registro de conversiones en archivos JSON 🗃️
Manejo de errores comunes 🚫
💻 Tecnologías
Java: Lenguaje principal
Gson: Para manipulación de JSON
ExchangeRate-API: API externa para tasas actualizadas
IntelliJ IDEA: IDE recomendado
📋 Requisitos
Antes de ejecutar, asegúrate de tener:

JDK 17 o superior ☕
Conexión a Internet 🌐
Dependencias
Gson para manipulación JSON.
🚀 Instalación
Clona el repositorio:

bash
Copiar código
git clone https://github.com/abdonsanchez/conversorDeMonedas
Configura la API:

Regístrate en ExchangeRate-API para obtener una clave API.
Configura tu clave en SearchExchangeRate.java:
java
Copiar código
String apiKey = "tu_clave_api";
Instala dependencias:

Para Maven/Gradle:
xml
Copiar código
<dependency>
<groupId>com.google.code.gson</groupId>
<artifactId>gson</artifactId>
<version>2.8.6</version>
</dependency>
O descarga gson.jar de la página de GSON.
Ejecuta el proyecto:

bash
Copiar código
javac Principal.java
java Principal
🏗️ Uso
Al iniciar, verás una lista de monedas.
Introduce el código de moneda base (ej. USD, EUR) 💵.
Introduce la moneda destino y la cantidad a convertir.
El programa mostrará el resultado y guardará las conversiones en un archivo JSON.
🗂️ Ejemplo de JSON generado
json
Copiar código
[
{
"baseCurrency": "USD",
"targetCurrency": "PEN",
"amount": 100,
"convertedAmount": 370.50,
"time_last_update_utc": "Mon, 07 Oct 2024 00:00:01",
"time_next_update_utc": "Tue, 08 Oct 2024 00:00:01",
"dateConsulta": "2024-10-06 11:07"
}
]
⚠️ Manejo de errores
Códigos de moneda incorrectos: Deben tener 3 letras.
Cantidad no numérica: Introduce un número válido.
Errores en la API: Mensaje claro sobre el error.
🤝 Contribuciones
¡Contribuye al proyecto!

Haz un fork del repositorio.
Crea una nueva rama:
bash
Copiar código
git checkout -b feature/nueva-feature
Realiza cambios y haz un commit:
bash
Copiar código
git commit -m "Añadida nueva feature"
Haz push a tu rama:
bash
Copiar código
git push origin feature/nueva-feature
Abre un Pull Request con tus cambios.