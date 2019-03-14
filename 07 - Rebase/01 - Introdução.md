# Rebase
### Permite recriar o histórico de commits
- Alteração de **mensagens**
- **Combinação** de commits
- **Descartando** alterações
- **Alteração** da hierarquia de commits

O *rebase*, em questão, é um método perigoso, mas com conhecimento profundo, pode ajudar bastante a **tratar os merges**

--- 
## Exemplo:
Se estou utilizando uma *branch feature* num time de desenvolvimento e um integrante atualiza a *branch master*, precisamos, no caso, atualizar a branch que estou utilizando com o **merge** ou com **rebase**
No caso, por mais simplicidade, usamos o merge para **unir** as duas branches além de não ser destrutiva, ele também não **alteara** commits já realizados
Ficaria assim:
![Merge](https://static.concrete.com.br/uploads/2017/08/image5-768x515.png)

Toda vez que é feito um *merge*, é criado um commit **irrelevante**. Isso pode trazer confusão no **histórico** de *commits*.
Para evitar esse commit *a mais*, podemos usar o **rebase**, que são parecidos, mas seus processos a chegar ao resultado são diferentes. 
O **merge** verifica todos os commits realizados por cima, mescla com a **branch** que será juntada e assim faz um **commit automático.** 
O **rebase** em si não faz esse commit, pelo fato de ele analisar por **baixo** primeiro. Assim, ele reconhece os commits que deve ser mesclado e coloca após a última alteração antes de mesclar.
Vale lembrar que **merges** do tipo **fast-forward** não cria um commit, somente quando é **3-way marge**.
**Para utilizar o rebase**:
`git rebase <nomeBranch>`


### Rebase Interativo
Além de podermos fazer *merge* com o rebase, existe a possibilidade de alterar os log dos commits para conseguirmos ter uma visualização mais coerente do que foi *commitado*
No caso,se tudo foi *mergeado* e não há nenhuma alteração a mais a se fazer, podemos usar um comando:
`git rebase -i HEAD~<número de quantos commits do maior para o menor>`
No caso:
`git rebase -i HEAD~3`
Irá retornar 3 *logs* de *commits*
**Essa é uma lista que podemos utilizar nessa parte:**

```bash
# Commands:
#  p, pick = use commit
#  r, reword = use commit, but edit the commit message
#  e, edit = use commit, but stop for amending
#  s, squash = use commit, but meld into previous commit
#  f, fixup = like "squash", but discard this commit's log message
#  x, exec = run command (the rest of the line) using shell
```

**Para renomear nome do commit:**
```bash
pick 9afe987 Ajustes de CSS e JS no slideshow.
pick 74e6f3e Mais ajustes de CSS e JS no slideshow.
reword 1ee9572 Atualiza o README.
```
Após isso irá algo como isso:
```bash
Atualiza o README.

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# Date:      Mon Dec 15 19:09:30 2014 -0200
#
# rebase in progress; onto 5644bdd
# You are currently editing a commit while rebasing branch 'develop' on '5644bdd'.
#
# Changes to be committed:
#       modified:   README.md
#
```

### Conflitos
No caso, se alterarmos um arquivo igual, iria ocorrer um conflito que na qual só seria solucionado manualmente. A pessoa que é responsável deverá escolher qual o correto e commitar. 
Nesse caso, é de extrema importância saber se é realmente requerido fazer o comando **git pull**, pois se um integrante estiver alterando o mesmo código, com certeza irá dar conflito.

<!--stackedit_data:
eyJoaXN0b3J5IjpbNjA4MTI2MDE0LDk2MzY2NDE2NSwtMTE0OD
UxMjgwOCw4ODg5ODM0MDIsLTEwNDQxODIyOTMsMzc2NzU3MjAw
LDE5NzI5NzU5MTEsMTY1NTUwOTE3MV19
-->