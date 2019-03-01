# Criando repositório local
Sem acesso ao conteúdo do repositório, pois sua finalidade é só um repositório local. Deve-se criar um clone desse repositório, assim, obtendo o working directory:
`git init --bare`

Pode-se armazenar pelo próprio **GitHub**!

---

# Criando repositório *remote*
Podemos criar o repositório sem arquivo nenhum (license or gitignore). Assim, teremos que referenciar na máquina local o endereço do repositório:
`git remote add origin <endereço>`

**Para mostrar o endereço exato:**
```git
git remote -v
	> origin <endereço> (fetch)
	  origin <endereço> (push)
```
**Para sincronizar com GitHub:**
`git push origin -u origin master

```markdown
    # foo
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMxMTU3NTE0NiwzNDgzOTA4NDgsMzYzOT
IzODUwLDE4ODM3NDY5MjAsLTQyOTMwNDQ1NiwyMDQwMjk3NjIy
XX0=
-->