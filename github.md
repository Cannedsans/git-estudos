# Usando o GitHub

Upar o repositório git o github precisa saber quem é que está mandando as modificações, então para isso o GitHub usa o SSH um protocolo de comunicação seguro.

para isso abra o terminal e digite o seguinte comando 

    ssh-keygen -t ed25519 -C "seu email"

após isso aparece as opções de configuração como nome do par porém apenas deixe default apertando enter, agora vá para a pasta .ssh onde está o arquivo 

pegue o arquivo que terminar com .pub usando

    cat nomeDoArquivo.pub

e no terminal copie a chave e vá em criar nova conexão ssh, lá cole sua chave e de um nome para a conexão apó essa etapa o GitHub estará conectado 

## Pull request 

as requisisções servem para quando uma brach nova ser criada o dono do repositórido analizar antes de dar uma merge e evitar que códigos incompletos sejam enviados e você pode fazer isso para o repositório de outras pessoas, com a permissão do dono você passa a ser um contribuente do projeto
