---
title: "¿Qué es 'Scope' en JavaScript?"
date: 2021-05-09
categories: javascript
layout: post-javascript
description: "Descripción de 'Scope' en JavaScript."
---

# ¿Qué es 'Scope' en JavaScript?

Scope es el alcance que poseen ciertos datos, ciertas variables.

## Scope global

Aquellas variables que se encuentren fuera de cualquier bloque de código son parte del scope global. Pueden ser consultadas desde cualquier parte de nuestro código.

## Scope local

Son aquellas variables declaradas dentro de los bloques de código y como parámetros de las funciones. No pueden ser consultadas en cualquier parte de nuestro código.

### Ejemplo

````js
let nombre = "Juan" //Scope global

function saludar (){
	let nombre = "Samuel"
	console.log(`Hola ${nombre}`) // output: Hola Samuel
}

function saludarGlobal(){
	console.log(`Hola ${nombre}`) //output: Hola Juan
}
````

***

- Quiero aprender más sobre: ["JavaScript"](../00/javascript)
