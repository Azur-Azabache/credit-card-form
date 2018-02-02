## Identificar los siguientes puntos:
***
### Función Global:
Función que engloba a las demás:
- $(document).ready(function() {})

### Funciones Locales:
Funciones localizadas dentro de la función global:
- Función activeButton()
- Función desactiveButton()
- Función longitud(input)
- Función soloNumeros(input)
- Función isValidCreditCard(numberCard)

### Funciones Callback:
Funciones que llevan a otra función por argumento:
 - Función longitud ubicada en la siguiente línea del código --->
  var creditCardNumber = soloNumeros(longitud(numberCard));

### Funciones Expressions:
Funciones encapsuladas en una variable:
 - La función soloNumeros ha sido asignada a la variable creditCardNumber ----> var creditCardNumber = soloNumeros(longitud(numberCard));

### Funciones Statement:
Funciones dispuestas a ser invocadas en cualquier parte del código:
- Función activeButton()
- Función desactiveButton()
- Función longitud(input)
- Función soloNumeros(input)
- Función isValidCreditCard(numberCard)

### Funciones Closure:
Funciones declaradas de manera interna que utilizan variables de una función padre. Funciones que recuerdan su "entorno":
- Función activeButton()
- Función desactiveButton()

### Scope:
 #### Variables globales:
 Variables cuyo alcance es global:
 -  var $inputCard = $('#card-number');
 - var $inputMonth = $('.input-month');
 - var $inputYear = $('.input-year');
 -  var $buttonNext = $('#next');
 -  var labelErrorOrSuccessMessages = $('label[for="card-number"]');}

#### Variables locales:
Variables definidas dentro del cuerpo de una función:
 -  var regex = /^[0-9]+$/;
 - var creditCardNumber = soloNumeros(longitud(numberCard));
 - var arr = [];
 - var sumaTotal = 0;

### Stack Execution:
Funciones a forman parte de la pila de ejecucción. Funciones que se ejecutaran al cargar el navegador (en este caso):
- $(document).ready(function() {})
- console.log('Probar con el numero valido 4544164785372342');  

### Event Queue:
Funciones que forman parte de la cola de eventos. Serán llamadas a medida que se invoquen:
- Función anónima: $inputCard.on('input', function() {})
- Función activeButton()
- Función desactiveButton()
- Función longitud(input)
- Función soloNumeros(input)
- Función isValidCreditCard(numberCard)
