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

## Ignorar arquivos 

As vezes não queremos que um arquivo seja mandado para os comits como .env então como podemos evitar isso? 

Criando o .gitignore! os arquivos listados dentro dele serão iginorados pelo git e não irão ser versionados 

## adicionando uma branch 

para ver as branchs precisamos usar o 

    git branch 

porém depois se quisermos cirar uma nova agente escreve 

    git branch nome_dela

e para trocar o checkout também, funciona 

    git checkout Nome_branch


e caso queira deletar, coloque um -d ou D no comando de criar 

agora hora da fusão! 

vá para a main de *DESTINO* e execute o seguinte código

    git merge branch

e todos os arquivos dessas branchs irão para a main 
em caso de conflitos quando for dar o merge o git ira mostrar os 2 códigos dentro do arquivo em conflito, resolva manualmente e quando terminar pode dar um commit sem a mensagem

## GITHUB 

Após a confuguração do *SSH* para mandar tudo para um repositório já existente digite 

    git push link_do_repositório.git branch 

em seguida após informar o repositório e a branch ele será upado no GitHub

