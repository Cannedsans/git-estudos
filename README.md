# Estudo de git

### Objetivos:
   - [ ] Apreder a criar um repositório sincronizado ao GITHUB
   - [X] Aprender a criar branches de forma consiente 
   - [X] Juntar branches da forma correta sem confusão
   - [X] Saber como resolver conflitos no git 
   - [ ] Por fim aprender a fazer tudo isso pelo *VS CODE*

## COMMIt 

O commit é um "Marco" na linha do tempo do seu código

### Recomendação 
 O commit é como uma fazer num jogo quando salvo ele é para caso eu morra não ter que fazer tudo novamente  
  #### Fazer um Commit num marco impactante como:
   - inicio do projeto
   - Adição de uma função 

### Os estados do commit 

#### MODIFIED
São qualquer modificação nos arquivos, deletado, modificado, criado literalmente qualqer alteração no projeto (cor verde para novos e azul para modificados)
#### STAGING
O palco é onde estão os arquivos prontos, por exemplo se o index.html está pronto para ser commitado porém o projeto todo não ele fica lá separado apenas esperando o commit (cor verde musgo)
#### COMMITED 
Os arquivos Commitados prontos para o novo marco, é indicado por os arquivos prontos palco para caso haja um commit os arquivos inacabados não sejam parte do marco de forma prematura  

## Branch 

As branchs são as linhas do tempo, por exemplo tenho o marco *x* quando criar uma nova branch a linha do tempo nova será baseada em *x* e depois que ela for concluidas ela pode ser fundida (merge) a branch principal e elas podem ser ciradas dentro de outras branches ou seja pode virar uma arvore com diferentes ramificações da linha do tempo 