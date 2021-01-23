
# Docker
-criando uma imagen no dokcer a partir do projeto:
$ docker build -t alura/forum .

- comando para o docker rodar a aplicação com a imagem alura/forum
$ docker run -p 8080:8080 
-e SPRING_PROFILES_ACTIVE='prod'
-e FORUM_DATABASE_URL='jdbc:h2:mem:alura-forum' 
-e FORUM_DATABASE_USERNAME='sa' 
-e FORUM_DATABASE_PASSWORD='' 
-e FORUM_JWT_SECRET='123456'
alura/forum