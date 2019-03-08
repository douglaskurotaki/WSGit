Para criar um arquivo **.gitignore** deve usar, criar manualmente no **repositório**. 
### Dentro desse arquivo, colocar os arquivos que não desejar.
Desse modo, eles não iram ser vinculados ao repositório mesmo estando no mesmo diretório.

### Se utilizar o Alias que retorna dados da API do site gitinore.io, utilizar esses comandos:
`gi <linguagem, tecnologia> >> .gitignore`

**Exemplo:**
`gi ruby >> .gitignore`

--- 

### Patterns do git
\# - Comentário
/ - Só ignora no diretório que indicar
\ - Escape
/** - Ignora um pattern específico

**Exemplos:**
Ignora todos os html's:
`*.html`

Exceção:
`!index.html`

Ignora no diretório atual, mas permite em outros:
`/README`

Ignora todos arquivos do diretório que indicar:
`build/`

Ignora os arquivos **txt** do diretório que indicar:
`doc/*.txt`

Ignora todos os **.pdf** na árvore **doc/** 
`doc/**/*.pdf`
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc5NDI4NzIyMV19
-->