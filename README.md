# Laravel ASAWL - 09. Fallos de validación de entrada

## Fallos de validación de entrada

Los fallos de validación de entrada en Laravel ocurren cuando los datos enviados por los usuarios no se verifican adecuadamente antes de ser procesados por la aplicación. Esto puede permitir a los atacantes manipular estos datos para realizar acciones no autorizadas o causar comportamientos inesperados en la aplicación.

Los fallos de validación de entrada suelen ocurrir de distintas maneras:

-	Entrada de datos: Los usuarios envían datos a la aplicación a través de formularios, parámetros de URL, cargas de archivos u otras interfaces. 
-	Validación insuficiente: La aplicación no verifica correctamente si los datos enviados cumplen con las reglas de negocio, los tipos de datos esperados o las restricciones de seguridad. 
-	Explotación: Los atacantes pueden aprovechar esta falta de validación para enviar datos maliciosos, como código JavaScript (XSS), consultas SQL (SQL Injection), o valores inesperados que pueden causar errores o comportamientos no deseados en la aplicación.

### Directrices de fallos de validación de entrada en Laravel

Laravel proporciona un sistema de validación robusto y fácil de usar para ayudarte a prevenir fallos de validación de entrada:

`Form Requests`: Las peticiones de formularios son clases personalizadas que encapsulan la lógica de validación para una solicitud específica (Laravel, 2023t). Pueden definir reglas de validación claras y concisas para cada campo de entrada, y Laravel se encargará de validar los datos automáticamente.

`Reglas de validación`: Laravel ofrece una amplia gama de reglas de validación integradas, como required, email, numeric, min, max, etc (Laravel, 2023u). También puedes crear tus propias reglas personalizadas para requisitos específicos.

`Mensajes de error personalizados`: Puedes personalizar los mensajes de error que se muestran al usuario (Laravel, 2023v) cuando la validación falla, proporcionando información clara y útil.

`Prevenir la inyección SQL`: tomar en cuenta todas las directrices de Inyección SQL.

`Prevenir la Cross-Site Scripting XSS`: tomar en cuenta todas las directrices de XSS.

`Prevenir la exposición de datos sensibles`: tomar en cuenta todas las directrices de exposición de datos sensibles.

### Recomendaciones para prevenir los fallos de validación de entrada en Laravel

-	Nunca confíes en los datos enviados por los usuarios sin validarlos primero.
-	Siempre utiliza el sistema de validación integrado de Laravel para facilitar y agilizar la validación de entradas.
-	Siempre sigue las recomendaciones para evitar la inyección SQL.
-	Siempre sigue las recomendaciones para evitar el Cross-Site Scripting XSS.
-   Siempre sigue las recomendaciones para evitar el Cross-Site Request Forgery CSRF, y.
-	Siempre sigue las recomendaciones para evitar la exposición de datos sensibles.

### Mitigación de fallos de validación de entrada en Laravel

La mitigación de fallos de validación de entrada se la realiza mediante:

-	Mitigación de inyección SQL.
-	Mitigación de Cross-Site Scripting XSS.
-	Mitigación de Cross-Site Request Forgery CSRF, y.
-	Mitigación de exposición de datos sensibles.
