# cep-problems

### Como agregar un nuevo problema:

- vayan a la carpeta `_posts/`
- crear un archivo con la fecha actual en el siguiente formato `%Y-%m-%d-nombre-del-problema.md`

No olviden poner lo siguiente en la cabecera del archivo:

    ---
    layout: post
    title:  "Titulo del Problema"
    ---

El archivo está en formato `markdown`, y también soporta fórmulas matemáticas con formato `latex` (ver los anteriores posts como ejemplo).


### Correr proyecto localmente

Este es un proyecto en jekyll, asi que necesitar tener [jekyll](http://jekyllrb.com) instalado.


    git clone git@github.com:cs-ucsp/cep-problems.git
    cd cep-problems
    jekyll serve

Luego te especificará la dirección donde esta corriendo, normalmente es en:

    http://localhost:4000
