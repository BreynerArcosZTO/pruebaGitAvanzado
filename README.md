# Prueba comandos para ramas mas limpias en GIT HUB

## Merge squash process
1. **Checkout the main branch**
`$ git checkout main`
2. **Create a squash commit of all data-cleanup changes**
`git merge --squash data-cleanup`
3. **Commit the squash commit to main branch history** 
`git commit -m "Implement and optimize data cleanup"`

## Octopus merge commands
Git Octopus Merge Command

`git merge -s`

octopusExample:

`$ git merge -s octopus ingest transform load`
`Trying simple merge with ingest`
`Trying simple merge with transform`
`Trying simple merge with load`
`Merge made by the 'octopus' strategy.`

Primera prueba de los merge

Usando el segundo merge "Octopus" despues de borrar la rama pruebaMerge

## Comandos:

#### #p, pick <commit> = usar commit
#### #r, reword <commit> = usar commit, pero editar el mensaje del commit
#### #e, edit <commit> = usar commit, pero detenerse para modificar
#### #s, squash <commit> = usar commit, pero fusionarlo con el commit anterior
#### #f, fixup [-C | -c] <commit> = similar a "squash", pero conservar solo el mensaje de registro del commit anterior, a menos que se use -C, en cuyo caso
#### #conservar solo el mensaje de este commit; -c es igual que -C pero
#### #abre el editor
#### #x, exec <comando> = ejecuta el comando (el resto de la línea) usando la shell
#### #b, break = detente aquí (continúa el rebase más tarde con 'git rebase --continue')
#### #d, drop <commit> = elimina el commit
#### #l, label <etiqueta> = etiqueta el HEAD actual con un nombre
#### #t, reset <etiqueta> = restablece el HEAD a una etiqueta
#### #m, merge [-C <commit> | -c <commit>] <etiqueta> [# <línea única>]
#### #crea un commit de fusión usando el mensaje del commit de fusión original
#### #(o la línea única, si no se especificó ningún commit de fusión original);
#### #usa -c <commit> para reformular el mensaje del commit
#### #u, update-ref <ref> = registra un marcador de posición para la <ref> que se actualizará
#### #a esta posición en los nuevos commits. La <ref> se
#### #actualiza al final del rebase