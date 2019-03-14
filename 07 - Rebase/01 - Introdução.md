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

### Conflitos
No caso, se alterarmos um arquivo igual, iria ocorrer um conflito que na qual só seria solucionado manualmente. A pessoa que é responsável deverá escolher qual o correto e commitar. 
Nesse caso, é de extrema importância saber se é realmente requerido fazer o comando **git pull**, pois se um integrante estiver alterando o mesmo código, com certeza irá dar conflito.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNDg1MTI4MDgsODg4OTgzNDAyLC0xMD
Q0MTgyMjkzLDM3Njc1NzIwMCwxOTcyOTc1OTExLDE2NTU1MDkx
NzFdfQ==
-->