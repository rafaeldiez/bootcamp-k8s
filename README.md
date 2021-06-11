# Bem vindo ao bootcamp de k8s

Pré-requisitos:

  - Ter o [Docker Desktop](https://www.docker.com/products/docker-desktop) instalado no seu desktop Windows.
  
  - Habilitar o Kubernetes no Docker Desktop, conforme mostra a imagem abaixo:

   ![image](https://user-images.githubusercontent.com/28758743/121741408-e17ee780-cad4-11eb-9853-2816820d460b.png)

  - Testando o acesso ao cluster k8s:
  
   ![image](https://user-images.githubusercontent.com/28758743/121742450-37a05a80-cad6-11eb-8e60-524fbf224d04.png)


  - Ter a imagem que usamos no bootcamp de docker, publicado no modo de acesso publico no seu repositório do docker hub:
  
   ![image](https://user-images.githubusercontent.com/28758743/121743450-c366b680-cad7-11eb-8129-4f78e0d03a6f.png)



O objetivo desse repositório é prover os manifestos que vão ser utilizados para a subir nosso container gerado no bootcamp de docker no kubernetes.

  - 1-deploy-nginx-docker-new.yaml -> Manifesto para criar a estrutura de deploy
  - 2-bootcamp-k8s-service.yaml -> Manifesto para criar o serviço "porta" de acesso a nossa aplicação
