# Indice
1. Taller de introducción a Markdown  
1.1 ¿Qué es Markdown?  
1.2 Etiquetas básicas de Markdown  
1.2.1 Encabezados  
1.2.2 Negrita y cursiva  
1.2.3 Resaltar un comando  
1.2.4 Bloques de código  
1.2.5 Enlaces  
1.2.6 Imágenes  
1.2.7 Listas  
1.2.8 Tablas  
1.2.9 Forzar un salto de línea  
1.2.10 Citar textos  
1.2.11 Comentarios  
1.2.12 Diagrama de flujo  
1.2.13 Ecuaciones matemáticas  
2. Referencias  


# 1. Taller de introducción a Markdown  
## 1.1 ¿Qué es Markdown?
Markdown es un lenguaje de marcado ligero creado por John Gruber y Aaron
Swartz que trata de **facilitar la redacción y lectura de documentos en texto plano**, utilizando un conjunto de etiquetas muy sencillas para aplicar estilo al documento.

Actualmente no existe un estándar para **Markdown**, por este motivo existen
diferentes versiones o flavors de **Markdown**.

En este curso vamos a trabajar con el flavor que se utiliza en GitHub para redactar los archivos README.md de los repositorios y la documentación técnica de los proyectos. Además *GitHub*, junto a *Discourse* o *reddit* están llevando una iniciativa para crear un estándar moderno de **Markdown** como es **CommonMark**.

En plataformas de repositorios remotos como *GitHub*, la función de este archivo es presentar información del proyecto, como:

• Descripción de su proyecto.  
• funcionalidades.  
• Cómo pueden usarlo los usuarios.  
• Donde los usuarios pueden encontrar ayuda sobre su proyecto.  
• Autores del proyecto.  

## 1.2 Etiquetas básicas de Markdown
### 1.2.1 Encabezados
#### Sintaxis Markdown:
```
\# Esto es un encabezado h1  
\# Esto es un encabezado h2  
\### Esto es un encabezado h3  
\#### Esto es un encabezado h4  
\##### Esto es un encabezado h5  
\###### Esto es un encabezado h6  
```

#### HTML renderizado en GitHub:
# Esto es un encabezado h1  
## Esto es un encabezado h2  
### Esto es un encabezado h3  
#### Esto es un encabezado h4  
##### Esto es un encabezado h5  
###### Esto es un encabezado h6  

## 1.2.2 Negrita y cursiva
| Estilo | Métodos abreviados | Sintaxis | Ejemplo | Salida |
| --- | --- | --- | --- | --- |
| Negrita | `Command + B` (Mac) o `Ctrl +B` (Windows o Linux) | ** ** o __ __ | \** Texto en negrita** | **Texto en negrita** |
| Cursiva | `Command + I` (Mac) o `Ctrl + I` (Windows o Linux) | * * o _ _ | \*Texto en cursiva* | *Texto en cursiva* |
| Tachado | Ninguno| ~~ ~~ | \~~Texto tachado~~ | ~~Texto tachado~~ |

## 1.2.3 Resaltar un comando
##### Sintaxis Markdown:
```
En esta frase estamos resaltando el comando `ls -la`.
```
##### HTML renderizado en GitHub:
En esta frase estamos resaltado el comando `ls -la` 

## 1.2.4 Bloques de código
Al inicio del bloque se puede indicar de forma opcional cuál es el tipo de contenido
que contiene el bloque para resaltar las palabras reservadas cuando se renderice.
Por ejemplo: `bash` , `python` , `yaml` , `json` , `html` , `javascript` , etc.

>Para omitir las comillas triple de bloque (```), podemos albergar todo el bloque con cuatro comillas (````), o escapar a cada comilla con (\`).

#### Sintaxis Markdown:
\```
sudo systemctl start apache2
\```
\```bash
\#!/bin/bash
echo "Hola mundo"
\```
\```python
celsius = float(input('Introduce una temperatura en grados
Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
\```
#### HTML renderizado en GitHub:
```
sudo systemctl start apache2
```
```bash
#!/bin/bash
echo "Hola mundo"
```
```python
celsius = float(input('Introduce una temperatura en grados
Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
```
## 1.2.6 Imágenes
#### Sintaxis Markdown:
Markdown:
```
![imagen1](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen"\)
```
HTML:
\<p align="center">
<img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR
\</p>

![imagen1](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen")

<p align="center">
<img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR">
</p>

### 1.2.7.2 Listas desordenadas
Puedes crear una lista anidada al dejar sangría en uno o más elementos de la lista
debajo de otro elemento.

#### Sintaxis Markdown:  
```
* Item 1
* Item 1.1  
* Item 1.2  
* Item 2  
* Item 2.1  
* Item 3  
* Item 4
```
#### HTML renderizado en GitHub:
* Item 1
    * Item 1.1
    * Item 1.2
* Item 2
    * Item 2.1
* Item 3
* Item 4
<!--COMPROBAR ESTE Y ARRIBA!-->
### 1.2.7.4 Listas ordenadas anidadas
Puedes crear una lista anidada al dejar sangría en uno o más elementos de la lista
debajo de otro elemento.
#### Sintaxis Markdown:
```
1. Item 1  
    1.1 Item 1.1  
    1.2 Item 1.2
2. Item 2  
    2.1 Item 2.1  
3. Item 3  
4. Item 4
```
#### HTML renderizado en GitHub::
1. Item 1  
    1.1 Item 1.1  
    1.2 Item 1.2
2. Item 2  
    2.1 Item 2.1  
3. Item 3  
4. Item 4  

### 1.2.11 Comentarios
Para poner un comentario en Markdown y que su contenido no sea rendereizado, se
utiliza la misma sintaxis que los comentarios de HTML. 

#### Sintaxis Markdown:  
```
Párrafo 1.  

<!-- Este texto es un comentario y no será renderizado -->  
Párrafo 2.  
```
#### HTML renderizado en GitHub:  

Párrafo 1.  
<!-- Este texto es un comentario y no será renderizado -->  
Párrafo 2.

### 1.2.13 Ecuaciones matemáticas

#### Sintaxis Markdown:
Para habilitar una comunicación clara de las expresiones matemáticas, GitHub
admite expresiones matemáticas con formato LaTeX en Markdown.
Como ya se ha comentado, al igual que ocurre con Latex, para poner una ecuación
se ha de poner entre $ la expresión concreta.  

* Para insertar una ecuación dentro de una frase, o para utilizar un carácter
especial, como letras griegas.  
```
    La ecuación, \$x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot
c}}{2 \cdot a}$, es de segundo grado.
```
* Como bloque.  
```
La ecuación de segundo grado es:  
\$$x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot
a}$$
```                                                          
#### HTML renderizado en GitHub:  
* Dentro de una frase  
La ecuación, $x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot
c}}{2 \cdot a}$, es de segundo grado.

* Como bloque.  
La ecuación de segundo grado es:
$$x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot
a}$$
# 2. Referencias  
* [GitHub](https://docs.github.com/es/get-started)  

* [IAW - Jose Juan Sánchez](https://josejuansanchez.org/iaw/taller-markdown/index.html#taller-de-introducci%C3%B3n-a-markdown)  

* [StackOverflow](https://stackoverflow.com/questions/24383700/resize-image-in-the-wiki-of-github-using-markdown)  

* [Editor de ecuaciones para Latex](https://latex.codecogs.com/eqneditor/editor.php?lang=es-es)  

* [README en tu GitHub](https://www.aluracursos.com/blog/como-escribir-un-readme-increible-en-tu-github)
