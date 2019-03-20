# Trabalhando com Tags
Apelido aos *commits* deixando mais amigáveis.
Numeração ao estado específico (*hash*)
<br>
Normalmente usa-se **versionamento semântico**:
**x.y.z**

- **x** - Major - Mudanças incompatíveis;
- **y** - Minor - Novas funcionalidades;
- **z** - Correções rápidas.

Para **criar** uma tag, declaramos:
```bash
git tag <x.y.z>
```
Após isso, podemos fazer nossas alterações, *commitando* e alocando para o repositório remoto.
```bash
git push origin master
git push origin --tags
```
Esse último serve para fazer as *tags* criadas para integrar ao repositório remoto.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIzMDQyNDkzMSwtMTgxNDc5NjI3MF19
-->