# Descripción

Una pequeña demo de cómo usar Quarto Markdown para generar documentos en docx o en pdf (con typst, que no requiere tener LATEX instalado (https://www.latex-project.org/)).

El arcchivo de interés es el "Documento.qmd", ya que 01.qmd y 02.qmd se insertan en el anterior como si fueran apartados o capítulos del documento principal.

En la parte inicial de "Documento.qmd" estaría el YAML, que permite definir las propiedades y formatos del documento y de sus formatos de exportación.

Para la utilización de parámetros o variables en Quarto que se puedan "llamar" posteriormente en integrar a lo largo del texto del documento final es necesario incluir "chunks" o bloques de código de los lenguajes R o Python.

En mi caso os he incluido un poco de código R para que podáis ver el efecto y funcionamiento a la hora de renderizar los documentos y generar los resultados en PDF y DOCX.

# Requerimientos

Para que funcione, es necesario instalar Quarto para tu sistema operativo: https://quarto.org/docs/get-started/

Los archivos qmd (Quarto Markdown) se pueden editar y trabajar desde VSCode, RStudio (que es el que uso yo con el lenguaje R), Jupyter (para Python) o cualquier editor de textos como Vim, SublimeText o incluso Notepad++

Para ejecutar mi ejemplo, sería necesario instalar Quarto y el lenguaje de programación R (https://www.r-project.org/).

Y para renderizar el archivo "Documento.qmd" a los formatos definidos en el YAML del archivo, se utiliza desde el terminal de tu PC el comando:

*quarto render Documento.qmd*

Si quieres especificar el formato de salida a otros compatibles con Quarto se puede especificar de la siguiente manera:;

*quarto render Documento.qmd --to docx*

*quarto render Documento.qmd --to typst* (éste genera un pdf sin la dependencia de LATEX)

Incluyo de todos modos los resultados obtenidos tras renderizar "Documento.qmd" a "Documento.pdf" y "Mi_Documento.docx" (éste nombre se ha personalizado en el YAML)
