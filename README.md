# ejerciciosJS

## ejercicio 1

```javascript

        console.log("Tabla del 5:");
        for (let i = 1; i <= 10; i++) {
            console.log("5 x " + i + " = " + (5 * i));
        }
```
## ejercicio 2

```javascript
for (let tabla = 1; tabla <= 10; tabla++) {
    console.log("Tabla del " + tabla + ":");
    for (let i = 1; i <= 10; i++) {
        console.log(tabla + " x " + i + " = " + (tabla * i));
    }
    console.log("");
        
```
## ejercicio 3

```javascript
var texto1 = prompt(" introduce el primer texto:");
var texto2 = prompt(" introduce el segundo texto:");

var esNumericoTexto1 = !isNaN(parseFloat(texto1)) && isFinite(texto1);
var esNumericoTexto2 = !isNaN(parseFloat(texto2)) && isFinite(texto2);

if (esNumericoTexto1) {
    alert("El primer texto introducido es un valor numérico.");
} else {
    alert("El primer texto introducido es una cadena.");
}

if (esNumericoTexto2) {
    alert("El segundo texto introducido es un valor numérico.");
} else {
    alert("El segundo texto introducido es una cadena.");
}
        
```

## ejercicio 4
```javascript

var texto1 = prompt("introduce el primer texto:");
var texto2 = prompt(" introduce el segundo texto:");

var textoConcatenado = texto1 + " " + texto2;

alert("El texto concatenado es: " + textoConcatenado);        
```

## ejercicio 5
```javascript
var numero1 = prompt(" introduce el primer número:");
var numero2 = prompt(" introduce el segundo número:");numero1 = parseFloat(numero1);
numero2 = parseFloat(numero2);

if (isNaN(numero1) || isNaN(numero2)) {
    alert("asegúrate de introducir números válidos.");
} else {
    var suma = numero1 + numero2;
    alert("La suma de " + numero1 + " y " + numero2 + " es: " + suma);
}
        
```

## ejercicio 6
```javascript
if (isNaN(numero1) || isNaN(numero2)) {
    alert(" asegúrate de introducir números válidos.");
} else {
    var resultado;
    switch (operacion) {
        case "+":
            resultado = numero1 + numero2;
            alert("El resultado de la suma es: " + resultado);
            break;
        case "-":
            resultado = numero1 - numero2;
            alert("El resultado de la resta es: " + resultado);
            break;
        case "*":
            resultado = numero1 * numero2;
            alert("El resultado de la multiplicación es: " + resultado);
            break;
        case "/":
            if (numero2 === 0) {
                alert("No se puede dividir por cero.");
            } else {
                resultado = numero1 / numero2;
                alert("El resultado de la división es: " + resultado);
            }
            break;
        default:
            alert("Operación incorrecta. Introduce una de las operaciones válidas: +, -, *, /");
            break;
    }
}
        
```
## ejercicio 7
```javascript
function pedirNota(numeroNota) {
    var nota;
    do {
        nota = prompt("Introduce la nota " + numeroNota + ":");
        nota = parseFloat(nota);
        if (isNaN(nota)) {
            alert("introduce una nota válida.");
        }
    } while (isNaN(nota));
    return nota;
}

var nota1 = pedirNota(1);
var nota2 = pedirNota(2);
var nota3 = pedirNota(3);

var media = (nota1 + nota2 + nota3) / 3;

var estado;
if (media >= 3) {
    estado = "Aprobado";
} else {
    estado = "Reprobado";
}

alert("La media de las notas es: " + media.toFixed(2) + "\nEl estudiante está: " + estado);
        
```

## ejercicio 8
```javascript
var numero1 = prompt("Introduce el primer número:");
var numero2 = prompt("Introduce el segundo número:");

numero1 = parseFloat(numero1);
numero2 = parseFloat(numero2);

if (numero1 === numero2) {
    alert("Los números son iguales: " + numero1);
} else if (numero1 > numero2) {
    alert("El número mayor es: " + numero1);
} else {
    alert("El número mayor es: " + numero2);
}
        
```

## ejercicio 9
```javascript
<style>
    /* Estilos para el cuadrado */
    .cuadrado {
        font-family: monospace;
        white-space: pre;
    }

    .borde {
        display: inline-block;
        border: 1px solid black;
    }

    .interior {
        display: inline-block;
        width: 40px; /* ajusta el tamaño del cuadrado */
        height: 40px; /* ajusta el tamaño del cuadrado */
    }
</style>
</head>
<body>

<div class="cuadrado">
    <div class="borde">*****
        <div class="interior">*   *</div>
        <div class="interior">*   *</div>
        <div class="interior">*   *</div>
    *****</div>
</div>

        
```

## ejercicio 10
```javascript
<style>
    .contenedor {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }

    .linea {
        white-space: pre;
        font-family: monospace;
    }
</style>
</head>
<body>

<div class="contenedor">
    <div class="linea">       *       </div>
    <div class="linea">     ***     </div>
    <div class="linea">   *****   </div>
    <div class="linea"> *******  </div>
    <div class="linea">*********</div>
    <div class="linea"> *******  </div>
    <div class="linea">  *****   </div>
    <div class="linea">   ***    </div>
    <div class="linea">    *     </div>
</div>
        
```
