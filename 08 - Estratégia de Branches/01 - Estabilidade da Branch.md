# Estabilidade das Branches
Antes de mais nada, precisamos possuir um código de qualidade e testado para ser enviado a produção. A branch que possui esse papel é **master**.

## Stable Trunk
**Branch Master** Sempre estável. As *branches temporárias* são muito utilizadas a fim de sempre deixar a principal sem erro algum. Nesse método, não utiliza *merges hell*, ou seja, merges que danificam a árvore das alterações dos códigos. Ela, de fato, é baseado num **tronco**. Esse tronco tem que ser resistente e parrudo! No entanto deve ser utilizado somente  para times bem pequenos ou projetos de duração curta. 

## Integration Pipelines
**Estável** e **Atualizado**.
Todas as *branches* são criadas a partir da *master*. 
Cada desenvolvedor trabalha **paralelamente** com sua *branch*.
No final é criado uma *realease* a partir de uma *branch* de **integração**. De fato, se a *realease* for aceita no teste, é combinada com a *master*.

## Single Branch
**Uso de apenas uma branch**.
Essa é usada apenas para caso o integrante seja único.
![Lone Wolf](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId20wtyy91xi.1a6.png)

<!--stackedit_data:
eyJoaXN0b3J5IjpbNjI0OTM5Nzc4LC0xMzMwMTk3MzI1LDExNz
MxMzEyMzcsMTgzNDYxOTc1LDE0Njc1Mzg2MDQsLTMyNjM1Mzcz
OF19
-->