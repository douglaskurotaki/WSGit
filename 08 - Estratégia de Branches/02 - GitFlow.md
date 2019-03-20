# GitFlow

**Git Flow** é uma extensão do próprio *git* para **organizar** as *branches*. Esse modelo serve para evitar possíveis problemas de agrupamentos de *releases* (o que foi gerados pelas *features*).
Umas da primeiras organizações, é o uso de **nomenclaturas** para as *branches*. Desse modo, pela convenção de nomes gerados por esse método é possível ver qual a funcionalidade de cada *branch*.

 - **Branch Master** - Quando vemos essa *branch* temos que saber que ela é a mais **estável**. Desse modo, podemos concluir que é essa a de **produção**.
 - **Branch Develop** - É a junção das *features* finalizadas, ou seja, que estão preparadas para o próximo *deploy.
 - **Branch Feature/\*** - São *branches* criados a partir da *branch develop*, pois a partir dela pode haver dependência de outros recursos para finalizar a *feature*. Por **convenção**, o nome da *branch* tem essa predominancia: `Branch feature/<nome-do-que-vai-ser-criado>`
 - **Branch Hotfix/\*** - São *branches* para **correção** das *master*. Assim, após a alteração, ela é juntada com a *master* e também com a *develop*, que no caso serve para os futuros *deploys*. Existe sua **convenção** aqui também: `hotfix/<x.y.z>`. Nesse caso é usado um padrão de **versionamento semântico**.
 - **Branch Release/\*** - É uma *branch* de confiança que faz a ligação da *develop* com a *master*. Assim, caso tenha ocorrido algum *bug* em algum *commit*, ainda há chance de fazer uma correção com mais facilidade. Essa *branch* tem a mesma **convenção** da *hotfix*, utilizando-se o versionamento semantico. `release/x.y.z`.
 
 ### Ação do merge das branches release e hotfix gera um git tags!
 Esses **git tags** são **atalhos** para acessar o *commit* realizado de acordo com a sua *hash*. No entanto, o diferencial está no *flow* conseguir alterar essa *hash* por um nome mais **amigável**.

# Tutorial!

Primeiramente, devemos **instalar** o *git flow*:
```bash
$ sudo apt-get install git-flow
```

<br>

Para verificar se foi instalado:
```bash
git flow
```
 
 <br>
 
 Após criar o **repositório**, temos que dar a inicialização do *git flow*:
 ```bash
 git flow init
 ```
 Assim, o *git* irá fazer algumas perguntas para trocar o nome das *branches*, porém é recomendável **manter** as que já vem por padrão.
 No final desse processo, o *git* automaticamente irá fazer um *checkout* na *branch develop*.
 
<br>

Para criar um *branch* **feature**:
```bash
# git flow feature start <nome-branch-feature>
# Exmplo:
git flow feature start recurso-milionario
```
Após isso, o *git* automaticamente irá dar *checkout* para essa nova *branch*

<br>

Agora, nós precisaremos de uma arquivo para **juntar** com a *branch develop*.
Depois de criar o arquivo, vamos juntar:
```bash
git flow feature finish <recurso-milionario>
```
Assim, a *branch* **recurso-milionario** foi integrada a *develop* e deu o *checkout* para essa mesma. A *branch* **recurso-milionario** é excluído depois desse processo.

<br>

Depois de terminar a *feature*, temos que criar uma *release branch* para, assim, poder colocar em **produção**. 
```bash
git flow release start 0.1.0
# Não esquecendo que esse é o número de versionamento semântico
```
Nessa *branch*, como é uma intermediação de **confiança**, as correções encontradas podem estar sendo realizadas aqui, ou então alguma alteração que tenha esquecido se inserir.

<br>

Nessa etapa, iremos **integrar** a *release 0.1.0* com a *master* e também com a *develop*.
```bash
git flow release finish 0.1.0
```
O **editor de texto** irá abrir **3 vezes!**

 - **1ª vez** - Edição do texto do *merge commit* entre *release 0.1.0* e *master*
 - **2ª vez** - Descrição da *tag* 0.1.0 para **facilitar mudanças**
 - **3ª vez** - Edição do texto do *merge commit* entre *release 0.1.0* e *develop*

Nessas etapa de edição dos *commits*, por convenção
 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc0MzQ1NTcyMywyMDQ3NDA5NjEwLC0xMD
g4MDI4MTM3LDcyOTM4OTAxMiwxNDE4NTI4NDU4LDE1MzEwNzY0
ODgsODQ5MTY4MDIyLDc1MzgwNjg0MiwtMzQwMzk0NzM4XX0=
-->