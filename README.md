<h1>Repositório do docker-composer para executarmos o sonar localmente.</h1>

<h4>Temos como pré-requisito o docker e o docker-composer instalados e configurados.</h4>

Recomendo baixar, copiar ou clonar o arquivo em arquivo chamado docker-compose.yaml, que pode ser criado no diretório de sua preferência.

Após a criação do arquivo abrir seu programa de terminal favorito e navegar até o diretório, dentro do diretório executar o comando:

docker compose up -d

Esse comando irá baixar as imagens dos contêineres(caso elas ainda não existam em seu computador), irá criar os volumes e os contêineres necessários 
para a execução do sonarqube e liberar o terminal por conta do parâmetro -d.
Após a execução poderemos acessar o sonar localmente na url: http://localhost:9000/.
O primeiro acesso ao sonar tem como usuário admin e senha admin e deveremos alterar a senha do admin no primeiro acesso.
Caso você obte por parar os serviços é só digitar:

docker compose down

Como utilizamos volumes para a persistência, quando você quiser executar novamente é só navegar até o diretório e digitar:
docker compose up -d

Deixo um link para o vídeo de instalação no meu canal do youtube.
https://www.youtube.com/watch?v=7y0OPsXkr9Y

E um link para a instalação do scanner que você vai precisar em um segundo momento para configurar os projetos:
https://dev.to/jhonywalkeer/sonarqube-instalacao-do-scanner-no-ubuntu-linux-3jc6
