# Estabilidade das Branches
Antes de mais nada, precisamos possuir um código de qualidade e testado para ser enviado a produção. A branch que possui esse papel é **master**.

## Stable Trunk
**Branch Master** Sempre estável. As *branches temporárias* são muito utilizadas a fim de sempre deixar a principal sem erro algum. Nesse método, não utiliza *merges hell*, ou seja, merges que danificam a árvore das alterações dos códigos. Ela, de fato, é baseado num **tronco**. Esse tronco tem que ser resistente e parrudo! No entanto deve ser utilizado somente  para times bem pequenos ou projetos de duração curta. 

## Integration Pipelines
**Estável** e **Atualizado**.
Todas as *branches* são criadas a partir da *master*. 
Cada desenvolvedor trabalha **paralelamente** com sua *branch*.
No final é criado uma *realease* a partir de uma *branch* de **integração**. De fato, se a *realease* for aceita no teste, é combinada com a *master*.

## S
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNzA3Njc3MjYsMTgzNDYxOTc1LDE0Nj
c1Mzg2MDQsLTMyNjM1MzczOF19
-->