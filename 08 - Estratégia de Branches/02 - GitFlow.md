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

Para verificar se foi instalado:
```bash
git flow
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTczMjc5NzgyNSw3MjkzODkwMTIsMTQxOD
UyODQ1OCwxNTMxMDc2NDg4LDg0OTE2ODAyMiw3NTM4MDY4NDIs
LTM0MDM5NDczOF19
-->