# Git HOW TO

## Download GIT

https://git-scm.com/downloads

## Verificar instalação
No terminal/CMD/etc... 

```
user$ git --version

git version 2.9.2
```


## Clonando repositório localmente
```
git clone 'repository'

// example
git clone https://github.com/armbrustsamuel/sist-embarcados-estacao-meteorologica.git
```

## Gerenciando repositório

### Git status
Retorna o estado atual do teu repositório local. 
- `Verde`: Arquivos adicionados para o commit
- `Vermelho`: arquivos modificados ou deletados/renomeados

#### Código de exemplo
```
git status
```

### Git add
Separa tuas alterações antes de fazer o commit, indicando que quais objetos tu queres enviar para o github.

#### Código exemplo
```
git add "nome-do-arquivo.extensao"
```

### Git commit
Salva tuas anterações locais. Somente após esse passo, teu código começa a ficar versionado e tu consegue saber o que foi alterado, ou se quer voltar para um versão anterior.

#### Código exemplo
```
git commit -m "reason for commit"
```

### Git push
Enviar tuas alterações para o repositório remoto.
#### Código exemplo
```
git push
```
