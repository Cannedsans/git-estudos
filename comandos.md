# Comandos em GIT
## Comando para ver as configurações de perfil 

    git config --global --list

A saida dever retornar os:

- user.name 
- user.email
  
## Para adicionar uma configuração

    git --global user.name "Seu nome aqui"
    git --global user.email Seu@email.com

## Para criar um repositório 

    git init

## Ver os estatus do repositório

    git status 

ele vai retornar: 

- a branch em que se está 
- os comits feitos 
- e os arquivos alterados/rastreados
## Adicionar os arquivos 

    git add arquivo ou .

ele vai colocar esses arquivos no palco, prontos para o commit (se por ponto ou .extenção vai colocar de forma filtrada)

## Remover do palco 

    git rm --cached nome do arquivo

## Primeiro commit 

    git commit -m "Sua mensagem aqui"

-m é um parametro opicional que irá adicionar uma mensagem descritiva sobre o commit

## Histórioco de commits 

Digamos que depois que fiz meu commit eu queira ver quais foram feitos, para isso usamos o:

    git log --oneline

## Trocar de ponto 

Para acessar um ponto anterior na linha do tempo precisa dar um checkout 

    git checkout id_do_ponto

e claro depois de ir para o ponto e queira voltar para a verão mais rescente pode usar o checkout 

    git checkout nome_Branch

## Reverter alterações 

Para quando queira retirar as alterações de um commit passado use 

    git revert id_do_ponto

*Atenção isso está sujeito a conflitos* e caso use o --hard ele apaga as alterações do futuro já feitas 