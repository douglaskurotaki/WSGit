# Trabalhando com Branches

As branches, de fato, servem para trabalhar em uma **outra linha de commits**, assim, com um foco no desenvolvimento a ser seguido.
Elas são geradas através de uma hierarquia, onde a cada criação de uma, surge mais uma **ramificação** de um certo ponto. 

![Essa é uma ramificação representando a Branch](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId1250rghj58.pqt.png)
As Branches são muito uteis para separar o desenvolvimento de um grupo de pessoas, assim evitando algum corrompimento de arquivos. 
### Alteração de uma pessoa não acarreta em outra, se utilizar branch.

###  Comandos:
`git branch <nomeBranch>`
ou
`git checkout -b <nomeBranch>` 

**Para utilizar uma outra branch:**
`git checkout <nomeBranch>`

**Para criar uma branch no repositório remoto (GitHub):**
`git push --set-upstream origin <nomeBranch>`
 
 **Para deletar uma branch:**
 Antes, lembrar de voltar a uma branch existente.
 `git branch --d <nomeBranch>`
`git push --delete origin <nomeBranch>`

**Atalho:**
Voltando a uma branch anterior:
`git checkout -`


<!--stackedit_data:
eyJoaXN0b3J5IjpbMzQ1OTU2MTMsNzMwMTU1NjMyLC00NzUyOD
c4MjcsMTM0NTUwMTcyXX0=
-->