# As etapas das ALTERAÇÕES

![Imagem](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId5vy54ke00.5h3.png)

> **Working directory** é o local onde os arquivos de navegação estão. Sua função é dar disponibilidade a seus arquivos para alterações na qual assim poderão ir ao **Staging Area**. Esse área, são locais que estão os arquivos adicionados (*git add*). Podemos então adicionar esses arquivos alterados ao repositório (*git commit -m "mensagem"*).

--- 

### Essas são as possibiliades entre Working Directory e Staged Area
![Imagem1](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId6n7ia1810.jh7.png)

---

```mermaid
sequenceDiagram
Working Directory ->> Staging Area: Stage Fixes
Staging Area ->> Repository: Commit
Repository ->> Working Directory: Checkout
 
```

```mermaid
sequenceDiagram
Alice ->> Bob: Hello Bob, how are you?
Bob-->>John: How about you John?
Bob--x Alice: I am good thanks!
Bob-x John: I am good thanks!
Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

Bob-->Alice: Checking with John...
Alice->John: Yes... John, how are you?
```








<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMxMzYwOTQwNywxMzYyMjEyODgxLDEzNj
IyMTI4ODEsLTc2MDA5NTA4Niw0Njk5OTUwMTgsLTYxMzEyNzM4
NiwxMTgzNzM0MTIyXX0=
-->