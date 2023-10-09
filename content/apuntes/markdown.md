+++
title = 'Markdown'
date = 2023-09-25T10:08:10+02:00
+++

En este apartado vamos a ver toda la sintaxsis que tiene Markdown, para poder explotarla y utilizarla al maximo 😃.

### 1. Encabezados

Se pueden crear encabezados utilizando el símbolo #. Cuantos más # uses, más pequeño será el encabezado.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
{{< /highlight >}}

Aqui un ejemplo de como se verian: 

# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6

### 2. Parrafos

Los párrafos se crean simplemente escribiendo texto. Markdown trata automáticamente los saltos de línea como un nuevo párrafo.

Aqui va un ejemplo:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
Esto es un párrafo.

Esto es otro párrafo.

{{< /highlight >}}


## 3. Enfasis

Puedes hacer que el texto se vea en cursiva o en negrita utilizando asteriscos * o guiones bajos _.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
*Texto en cursiva*
_Texto en cursiva_

**Texto en negrita**
__Texto en negrita__
{{< /highlight >}}

Aqui va un ejemplo de como se veria:

*Texto en cursiva*

_Texto en cursiva_

**Texto en negrita**

__Texto en negrita__

### 4. Listas

Se pueden crear listas tanto ordenadas como no ordenadas.

##### Listas no ordenadas

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
- Elemento 1
- Elemento 2
  - Subelemento 2.1
  - Subelemento 2.2
- Elemento 3
{{< /highlight >}}

Aqui va un ejemplo:

- Elemento 1
- Elemento 2
  - Subelemento 2.1
  - Subelemento 2.2
- Elemento 3

##### Listas ordenadas

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
{{< /highlight >}}

Aqui va un ejemplo:

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

### 5. Enlaces

Para crear enlaces se haria de esta manera:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
[texto del enlace](URL)
{{< /highlight >}}

Por ejemplo:

[Google](https://google.com)

### 6. Imagenes

Para incluir imagenes se haria de esta manera:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
![texto alternativo](URL de la imagen)
{{< /highlight >}}

Por ejemplo:

![Logo de Markdown](https://markdown-here.com/img/icon256.png)


### 7. Citas

Para crear citas se utilizaria el simbolo '>' al principio de una linea.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
> Esto es una cita
{{< /highlight >}}

Aqui va un ejemplo:
> Esto es una cita

### 8. Codigo

Se puede formatear texto como codigo utilizando comillas simples ` o triples ```

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
Inline code: `codigo`
{{< /highlight >}}

Aqui va un ejemplo: 

Inline code: `codigo`

Y asi seria con comillas triples:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
```python
def funcion():
    print("Hola, mundo!")
{{< /highlight >}}

Aqui un ejemplo:

```python
def funcion():
    print("Hola, mundo!")
```

### 9. Reglas Horizontales

Se pueden crear reglas horizontales utilizando tres o más guiones, asteriscos o guiones bajos en una línea.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
---
{{< /highlight >}}

Por ejemplo:

--- 
### 10. Tablas

crear tablas en Markdown utilizando barras verticales (|) para separar las celdas y guiones (-) para indicar las filas de encabezado. Aquí tienes un ejemplo de cómo crear una tabla simple:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
| Encabezado 1 | Encabezado 2 | Encabezado 3 |
| ------------ | ------------ | ------------ |
| Celda 1,1    | Celda 1,2    | Celda 1,3    |
| Celda 2,1    | Celda 2,2    | Celda 2,3    |

{{< /highlight >}}

Aqui un ejemplo de como se veria una tabla:

| Encabezado 1 | Encabezado 2 | Encabezado 3 |
| ------------ | ------------ | ------------ |
| Celda 1,1    | Celda 1,2    | Celda 1,3    |
| Celda 2,1    | Celda 2,2    | Celda 2,3    |


### 11. Tachado

Para tachar texto en Markdown, puedes utilizar el doble símbolo de tilde (~~) alrededor del texto que deseas tachar.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
Este es un texto ~~tachado~~.
{{< /highlight >}}

Asi se veria:

Este es un texto ~~tachado~~.

