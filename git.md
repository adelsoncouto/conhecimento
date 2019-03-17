# Ajudas sobre o git

## Apagar histórico do repositório

Cria um novo branch

```bash
git checkout --orphan tmp
```

Adiciona tudo nesse novo branch

```bash
git add -A .
```

Faz um commit

```bash
git commit -m 'reiniciar commit'
```

Deleta o branch master

```bash
git branch -D master 
```

Renomeia o branch para master

```bash
git branch -m master 
```

Faz o push, para o gitlab deve desbloquear o branch master em (português) _Configurações/Repositório/Protected Brancher_

```bash
git push -f origin master
```

Apagar os arquivos antigos

```bash
git gc --aggressive --prune=all
```

Fonte

https://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository
