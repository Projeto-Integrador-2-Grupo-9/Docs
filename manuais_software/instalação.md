## Manual de Instalação

Para a execução do projeto, é necessária a instalação do Docker, Docker-Compose, NodeJS e Yarn

Clone os repositórios: 

  API, Atena, Poseidon, FakeFloater e Frontend.
  
## Atena e Poseidon
  Entre na pasta de cada microsserviço e rode:
  
    docker-compose up
    
## API 
  Entre na pasta e rode:
  
    docker-compose up
    
  Em seguida, é necessário criar uma network docker para que os serviços se comuniquem, então execute os seguintes comandos:
   
    docker network create aquadata_network
    
  Logo após, adicione todos os containers a network com os comandos:
  
    docker network connect aquadata_network AD_API
    
    docker network connect aquadata_network AD_ATE
    
    docker network connect aquadata_network AD_POS
   
## Frontend

  Entre na pasta do projeto, em seguida, entre na pasta frontend. Execute os seguintes comandos
  
    yarn install
    
    yarn start
    
## FakeFloater

   Entre na pasta do projeto e execute:
   
    docker-compose up
    
Dessa forma, já é possível acessar o projeto na porta 3000.
   
   
   


  
