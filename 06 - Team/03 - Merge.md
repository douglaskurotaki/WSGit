# Utilizando o Merge
### É a ação de combinar duas branches.
Se usa o seguinte código:
`git merge <nomeBranch>`

### Existem tipos de se fazer merge:
**Fast Forward** - Move a referencia da branch trabalhada com o **HEAD** da branch a ser combinada gerando um histórico de commits **linear**.
![Commit Linear](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId14km5kv44u.ktl.png)


**3-Way Merge** - Quando há novos commits que não fazem parte da branch a ser combinada. Nesse caso são feitos **3 commits** para gerar o merge. Um commit é feito somente para juntar as branches. 
![Commits distintos](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId15q356ecnz.46f.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTY0MjI1Mjk5NV19
-->