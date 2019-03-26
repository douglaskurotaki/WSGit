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

### reset mixed
O **mixed** é semelhante ao anterior, porém a única diferença é que serão desfeitas alterações, assim, voltará para o *working directory*. Nesse caso, terá que ser feito o `git add` novamente.
Esse comando pode ser feito de duas formas:
```bash
# 1ª forma:
git reset HEAD~<numeroDoCommit>

# 2ª forma:
git reset --mixed HEAD~<numeroDoCommit>
```




<!--stackedit_data:
eyJoaXN0b3J5IjpbNTU0MDgyMTM2LC0xMTg0NDg1MzksLTE0Nj
A2NDAzMDIsLTIwODg3NDY2MTJdfQ==
-->