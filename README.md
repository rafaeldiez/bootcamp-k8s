# Bem vindo ao bootcamp de k8s

Pré-requisitos:

  - Ter o [Docker Desktop](https://www.docker.com/products/docker-desktop) instalado no seu desktop Windows.
  
  - Habilitar o **Kubernetes** no **Docker Desktop**, conforme mostra a imagem abaixo:

   ![image](https://user-images.githubusercontent.com/28758743/121741408-e17ee780-cad4-11eb-9853-2816820d460b.png)

  - Testando o acesso ao cluster k8s:
  
   ![image](https://user-images.githubusercontent.com/28758743/121742450-37a05a80-cad6-11eb-8e60-524fbf224d04.png)
   
   Com o acesso validado, crie o namespace **bootcamp** no cluster com o comando:
   
   **kubectl create ns bootcamp**
   

  - Ter a imagem que usamos no bootcamp de docker, publicado no modo de acesso publico no seu repositório do docker hub:
  
   ![image](https://user-images.githubusercontent.com/28758743/121743450-c366b680-cad7-11eb-8129-4f78e0d03a6f.png)


# Instruções para subir a aplicação

O objetivo desse repositório é prover os manifestos que vão ser utilizados para a subir nosso container, que foi gerado no **bootcamp de docker** no kubernetes.

  -  Manifesto para criar a estrutura de deploy:
```sh
1-bootcamp-deploy-nginx.yaml
```

**OBS** - Após baixar os arquivos, devemos editar o manifesto **deploy-nginx-docker-new.yaml**, para informar qual a imagem que será utilizada no seu ambiente, aqui devemos apontar sua imagem que foi gerado no **bootcamp de docker**:

![image](https://user-images.githubusercontent.com/28758743/122944664-64623680-d34e-11eb-9b71-10cf538c2ec5.png)
    
 - Manifesto para criar o serviço "porta" de acesso a nossa aplicação
```sh
2-bootcamp-service-nginx.yaml
```

Com a aplicação rodando, devemos usar o comando:

**kubectl port-forward svc/bootcamp-k8s 8080:80  -n bootcamp**

O comando acima é uma das formas de acessar nossa aplicação pelo navegador.

![image](https://user-images.githubusercontent.com/28758743/121746312-117db900-cadc-11eb-8993-bce750323a52.png)

