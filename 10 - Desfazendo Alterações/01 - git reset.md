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
Nesse tipo de reset, o **HEAD** apontara para o antecessor *commit* realizado. No caso, não terá nenhum arquivo perdido, ele voltará apenas para *working directory*. 

```bash
git reset --soft 
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE5OTgwMzM0NCwtMTE4NDQ4NTM5LC0xND
YwNjQwMzAyLC0yMDg4NzQ2NjEyXX0=
-->