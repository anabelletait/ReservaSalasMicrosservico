Sistema de Reserva de Salas com Microsserviços  
Este projeto foi desenvolvido para aplicar conceitos de microsserviços em um sistema simples de reserva de salas. A ideia é dividir o sistema em serviços independentes, facilitando manutenção e escalabilidade.

Todos os serviços estão separados por pastas e são iniciados juntos com Docker Compose.

Como executar:

Primeiro, é necessário ter o Docker instalado na máquina. Caso não tenha, dá pra baixar no site oficial: https://www.docker.com/get-started

Depois, clone este repositório:

git clone https://github.com/anabelletait/ReservaSalasMicrosservico.git  
cd ReservaSalasMicrosservico

Dentro da pasta do projeto, rode o seguinte comando pra subir tudo:

docker-compose up --build

Esse comando já vai construir os serviços e subir todos os containers.

Com tudo rodando, os serviços ficam disponíveis nas portas:  
application → http://localhost:8080  
usuario → http://localhost:8083  
sala → http://localhost:8082  
reserva → http://localhost:8081

Se quiser parar tudo depois:  
docker-compose down --rmi all
