
La traducción del libro casi está completa. Este repositorio ha sido archivado
y partir de ahora, las futuras revisiones 
(y la traducción del apéndice) del libro serán llevadas a cabo en el 
repositorio de Gitlab

https://gitlab.com/uzluisf/piensaperl6/

¡Nos vemos allá!

---
# Piensa en Perl 6

Archivo LATEX de la traducción en español de Think Perl 6.

![book cover](book/figs/thinkperl6_cover.png)

Traducción por Luis F. Uceta.

La versión original en inglés por Laurent Rosenfeld con Allen Downey puede
ser encontrada en [Think Perl 6](http://greenteapress.com/wp/think-perl-6/).

**Descarga directa**: [piensaperl6.pdf]()

Si deseas el PDF con la última revisión, sigue las instrucciones en la
siguiente sección.

### Cómo crear el PDF

El directorio `book` contiene los archivos LATEX necesarios para
compilar el libro. Para recompilar el libro, ejecuta el siguiente
comando dentro de dicho directorio:
```
make
```
Este comando creará el directorio `tmpDir` donde se encuentra el
PDF (piensaperl6.pdf) del libro. 

> Nota: La posibilidad de una compilación exitosa incrementa si tiene una instalación
> casi completa de una distribución reciente de Tex Live.

Para eliminar todos los archivos intermedios (incluyendo el PDF)
que resultan del proceso de compilación, ejecuta:
```
make clean
```
Si deseas mantener el PDF, debes moverlo a un directorio diferente antes
de ejecutar `make clean`.
