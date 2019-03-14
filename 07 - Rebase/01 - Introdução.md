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

### Conflitos
No caso, se alterarmos um arquivo igual, iria ocorrer um conflito que na qual só ser
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg5NjEyNTIzOCwzNzY3NTcyMDAsMTk3Mj
k3NTkxMSwxNjU1NTA5MTcxXX0=
-->