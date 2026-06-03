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

Usando el segundo merge "Octopus"