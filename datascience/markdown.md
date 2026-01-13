---
title: "Markdown"
format: html
editor: visual
---

## Introducción a Markdown

Markdown es un lenguaje de marcado ligero que permite añadir elementos de formato a documentos de texto sin formato. Creado por [John Gruber](https://daringfireball.net/projects/markdown/) en 2004, Markdown es actualmente uno de los lenguajes de marcado más populares del mundo. Markdown se puede usar para todo. Se usa para crear sitios web, documentos, notas, libros, presentaciones, correos electrónicos y documentación técnica. Markdown es independiente de la plataforma.

![El flujo de Markdown](https://mdg.imgix.net/assets/images/markdown-flowchart.png?auto=format&fit=clip&q=40&w=1080)

## ¿Por qué usar Markdown?

- **Simplicidad**: Sintaxis sencilla y fácil de aprender
- **Portabilidad**: Archivos de texto plano que funcionan en cualquier sistema
- **Versatilidad**: Se puede convertir a HTML, PDF, Word, y más
- **Control de versiones**: Ideal para Git y GitHub
- **Ampliamente adoptado**: Usado en GitHub, Jupyter, Stack Overflow, Reddit, y más

## Recursos de ayuda

- [Markdown Guide](https://www.markdownguide.org/) - Guía completa de Markdown
- [GitHub Flavored Markdown](https://github.github.com/gfm/) - Especificación de GFM
- [Markdown Tutorial](https://www.markdowntutorial.com/) - Tutorial interactivo
- [CommonMark](https://commonmark.org/) - Especificación estándar
- [Communicate using Markdown](https://github.com/skills/communicate-using-markdown?tab=readme-ov-file#communicate-using-markdown) - Curso de GitHub Skills sobre Markdown

Rich content editors. [*Link*](https://markdownguide.offshoot.io/tools/)
    -   Dillinger. [*Link*](https://dillinger.io/).
    -   Prosemirror. [*Link*](https://prosemirror.net/).
    -   StackEdit. [*Link*](https://stackedit.io/)

## Sintaxis básica

### Encabezados

```markdown
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
```

### Énfasis

```markdown
*cursiva* o _cursiva_
**negrita** o __negrita__
***negrita y cursiva*** o ___negrita y cursiva___
~~tachado~~
```

Ejemplo:
- *cursiva* o _cursiva_
- **negrita** o __negrita__
- ***negrita y cursiva***
- ~~tachado~~

### Listas

#### Listas no ordenadas

```markdown
- Elemento 1
- Elemento 2
  - Sub-elemento 2.1
  - Sub-elemento 2.2
- Elemento 3

* También funciona con asteriscos
+ O con signos más
```

#### Listas ordenadas

```markdown
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
   1. Sub-elemento 3.1
   2. Sub-elemento 3.2
```

### Enlaces

```markdown
[Texto del enlace](https://www.ejemplo.com)
[Enlace con título](https://www.ejemplo.com "Título del enlace")
<https://www.ejemplo.com>
```

Ejemplo: [Markdown Guide](https://www.markdownguide.org/)

### Imágenes

```markdown
![Texto alternativo](ruta/a/imagen.png)
![Texto alternativo](ruta/a/imagen.png "Título de la imagen")
```

### Código

#### Código en línea

```markdown
Usa `código en línea` con comillas invertidas.
```

Ejemplo: El comando `git status` muestra el estado del repositorio.

#### Bloques de código

````markdown
```
Bloque de código simple
```

```python
# Código Python con resaltado de sintaxis
def hola_mundo():
    print("Hola, mundo!")
```

```javascript
// Código JavaScript
const saludo = "Hola, mundo!";
console.log(saludo);
```
````

### Citas

```markdown
> Esta es una cita.
> Puede tener múltiples líneas.
>
> Y múltiples párrafos.

> Nivel 1
>> Nivel 2
>>> Nivel 3
```

Ejemplo:
> Esta es una cita de ejemplo.
> Markdown hace que sea fácil citar texto.

### Líneas horizontales

```markdown
---
***
___
```

---

### Tablas

```markdown
| Encabezado 1 | Encabezado 2 | Encabezado 3 |
|--------------|--------------|--------------|
| Celda 1      | Celda 2      | Celda 3      |
| Celda 4      | Celda 5      | Celda 6      |

| Alineación izquierda | Centrado | Alineación derecha |
|:---------------------|:--------:|-------------------:|
| Texto                | Texto    | Texto              |
```

Ejemplo:

| Lenguaje   | Año  | Creador         |
|------------|------|-----------------|
| Python     | 1991 | Guido van Rossum|
| JavaScript | 1995 | Brendan Eich    |
| Ruby       | 1995 | Yukihiro Matsumoto|

## Sintaxis extendida (GitHub Flavored Markdown)

### Listas de tareas

```markdown
- [x] Tarea completada
- [ ] Tarea pendiente
- [ ] Otra tarea pendiente
```

Ejemplo:
- [x] Aprender sintaxis básica de Markdown
- [ ] Practicar con ejemplos
- [ ] Crear mi primer documento

### Menciones y referencias

```markdown
@usuario - Mencionar a un usuario
#123 - Referencia a un issue
```

### Emojis

```markdown
:smile: :heart: :thumbsup: :rocket:
```

Ejemplo: :smile: :rocket: :heart:

### Bloques de código con información adicional

````markdown
```python {.line-numbers}
def ejemplo():
    print("Código con números de línea")
```
````

### Notas al pie

```markdown
Texto con una nota al pie[^1].

[^1]: Esta es la nota al pie.
```

## Markdown en diferentes contextos

### GitHub

GitHub usa GitHub Flavored Markdown (GFM) que incluye:
- Autoenlaces para URLs
- Tachado con `~~`
- Listas de tareas
- Tablas
- Menciones de usuarios y equipos
- Referencias a issues y pull requests

### Jupyter Notebooks

Jupyter usa Markdown en las celdas de texto para:
- Documentar análisis de datos
- Explicar código
- Incluir ecuaciones matemáticas con LaTeX

### Quarto

Quarto extiende Markdown con:
- Callouts (cuadros de alerta)
- Divs y spans
- Atributos de código
- Referencias cruzadas
- Citas y bibliografía

Ejemplo de callout en Quarto:

```markdown
::: {.callout-note}
Esta es una nota importante.
:::

::: {.callout-warning}
Esta es una advertencia.
:::

::: {.callout-important}
Esto es muy importante.
:::
```

## Matemáticas con LaTeX

### Ecuaciones en línea

```markdown
La ecuación $E = mc^2$ es famosa.
```

### Ecuaciones en bloque

```markdown
$$
\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$
```

Ejemplo:

La ecuación de Einstein: $E = mc^2$

Fórmula cuadrática:
$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

## Herramientas útiles

### Editores de Markdown

- **Visual Studio Code**: Con extensiones como Markdown All in One
- **Typora**: Editor WYSIWYG de Markdown
- **Obsidian**: Para tomar notas con Markdown
- **MarkText**: Editor gratuito y de código abierto
- **Dillinger**: Editor online de Markdown

### Conversores

- **Pandoc**: Conversor universal de documentos
- **Markdown to PDF**: Herramientas online
- **kramdown**: Procesador de Markdown en Ruby

### Cheatsheets

- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- [GitHub Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## Buenas prácticas

1. **Usa espacios en blanco**: Deja líneas en blanco entre elementos para mejor legibilidad
2. **Consistencia**: Mantén un estilo consistente (por ejemplo, siempre usa `*` para listas)
3. **Nombres de archivo**: Usa nombres descriptivos con extensión `.md` o `.markdown`
4. **Previsualización**: Siempre previsualiza tu documento antes de publicar
5. **Control de versiones**: Usa Git para rastrear cambios en archivos Markdown
6. **Documenta código**: Usa README.md para documentar proyectos
7. **Simplicidad**: No sobrecargues con formato innecesario

## Diferencias entre sabores de Markdown

| Característica | CommonMark | GFM | Pandoc | Quarto |
|----------------|------------|-----|--------|--------|
| Sintaxis básica | ✓ | ✓ | ✓ | ✓ |
| Tablas | - | ✓ | ✓ | ✓ |
| Listas de tareas | - | ✓ | ✓ | ✓ |
| Notas al pie | - | ✓ | ✓ | ✓ |
| Atributos | - | - | ✓ | ✓ |
| Divs/Spans | - | - | ✓ | ✓ |
| Callouts | - | - | - | ✓ |

## Ejemplos prácticos

### README de proyecto

```markdown
# Nombre del Proyecto

## Descripción
Una breve descripción del proyecto.

## Instalación
```bash
pip install mi-paquete
```

## Uso
```python
import mi_paquete
mi_paquete.funcion()
```

## Contribuir
Por favor lee [CONTRIBUTING.md](CONTRIBUTING.md) para detalles.

## Licencia
Este proyecto está bajo la Licencia MIT - ver [LICENSE.md](LICENSE.md)
```

### Documentación de API

```markdown
# API Reference

## `funcion_ejemplo(parametro1, parametro2)`

### Descripción
Realiza una operación específica con los parámetros dados.

### Parámetros
- `parametro1` (str): Descripción del primer parámetro
- `parametro2` (int): Descripción del segundo parámetro

### Retorna
- `dict`: Un diccionario con los resultados

### Ejemplo
```python
resultado = funcion_ejemplo("texto", 42)
print(resultado)
```
```

## Videos tutoriales

- [Markdown Crash Course](https://www.youtube.com/watch?v=HUBNt18RFbo) - Traversy Media
- [Markdown Tutorial for Beginners](https://www.youtube.com/watch?v=2JE66WFpaII) - Corey Schafer

## Recursos adicionales

- [The Markdown Guide Book](https://www.markdownguide.org/book/) - Libro completo sobre Markdown
- [Awesome Markdown](https://github.com/mundimark/awesome-markdown) - Lista curada de recursos
- [Markdown Style Guide](http://www.cirosantilli.com/markdown-style-guide/) - Guía de estilo
