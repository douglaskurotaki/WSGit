# Git Reset
Esse é um comando utilizado para **voltar** alterações realizadas. Porém, é muito perigoso pois podem haver alterações **perdidas** e que serão **irreversíveis**.
As áreas **afetadas** do *git* são:

- **HEAD** (o ponteiro);
- **Área de Stage**;
- **Diretório de Working**.

<br>

O **HEAD** está sempre apontando para o **último** grupo de alterações, ou seja, o **snapshot** *commitado*.
A movimentação do ponteiro pode ser realizada por dois comando: **commit** e **reset**.

<br>

Existem 3 **tipos** de *reset*:
### reset soft
Nesse tipo de reset, o **HEAD** apontara para algum *commit* realizado. No caso, não terá nenhum arquivo perdido, ele voltará apenas para *staging area*. 

```bash
git reset --soft HEAD~<númeroDeCommitAntecessor>
# ou então podemos usar a hash
```




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyNzk2MDEyMDUsLTExODQ0ODUzOSwtMT
Q2MDY0MDMwMiwtMjA4ODc0NjYxMl19
-->