# As etapas das ALTERAÇÕES

```mermaid
sequenceDiagram
Working Directory ->> Staging Area: Stage Fixes
Staging Area ->> Repository: Commit
Repository ->> Working Directory: Checkout
 
```
> **Working directory** é o local onde os arquivos de navegação estão. Sua função é dar disponibilidade a seus arquivos para alterações na qual assim poderão ir ao **Staging Area**. Esse área, são locais que estão os arquivos adicionados (*git add*). Podemos então adicionar esses arquivos alterados ao repositório (*git commit -m "mensagem"*).

--- 

### Essas são as possibiliades entre Working Directory e Staged Area
![Imagem1](https://d2v0x26thbzlwf.cloudfront.net/prod/190/img/rId6n7ia1810.jh7.png)









<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExMjExOTkzMTUsMTM2MjIxMjg4MSwtNz
YwMDk1MDg2LDQ2OTk5NTAxOCwtNjEzMTI3Mzg2LDExODM3MzQx
MjJdfQ==
-->