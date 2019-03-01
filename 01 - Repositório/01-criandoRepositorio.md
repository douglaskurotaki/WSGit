# Criando repositório local
Sem acesso ao conteúdo do repositório, pois sua finalidade é só um repositório local. Deve-se criar um clone desse repositório, assim, obtendo o working directory:
`git init --bare`

Pode-se armazenar pelo próprio **GitHub**!

---

# Criando repositório *remote*
Podemos criar o repositório sem arquivo nenhum (license or gitignore). Assim, teremos que referenciar na máquina local o endereço do repositório:
`git remote add origin <endereço>`

**Para mostrar o endereço exato:**
```
git remote -v
	> origin <endereço> (fetch)
	  origin <endereço> (push)
```






<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNzYzNDUyNzgsMTg4Mzc0NjkyMCwtND
I5MzA0NDU2LDIwNDAyOTc2MjJdfQ==
-->