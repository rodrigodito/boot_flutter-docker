# boot_flutter-docker
Boot de flutter com docker

## Dependencias
  * Docker
  * Visual Studio Code
  * Remote Development (Extensão para Visual Studio Code)
  
  Para instalar a extensão "Remote Development" acesse o [Link](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) ou pesquise a extensão dentro do Visual Studio Code
  
  
## Criando o container
Faça o download ou clone esse repositório na pasta de sua preferencia

Abra o Visual Studio Code

Clique no icone do Remote Development, localizado no canto inferior esquerdo do programa ou use o atalho "ctrl + shift + p"

![Icone Remote Development](https://blog.codemagic.io/uploads/2020/04/docker_1.png)

Selecione a opção "Remote-Containers: Open folder in Container"
![Remote-Containers: Open folder in Container](https://blog.codemagic.io/uploads/2020/04/docker_2.png)

Selecione a pasta onde o projeto foi clonado, deve ser a pasta raiz, onde se encontra o Dockerfile

Após isso o seu container começará a ser criado, isso pode demorar alguns minutos, no canto inferior direito você pode ver o progresso.

Finalizada a criação do container seu workspace já está pronto para trabalhar com o flutter.



## Rodando o Projeto

Para testar, conecte seu celular em uma porta USB do seu computador e certifique de deixar seu celular liberado para debugger.

Abra o terminal do VSCode e digite 
```
flutter doctor
```
Deve ficar assim: 

![flutter doctor](https://blog.codemagic.io/uploads/2020/04/docker_6.png)


Note que neste repositório já existe um projeto em flutter criado, para rodar esse projeto, abra o terminal do VSCode e digite:
```
cd MyApp
```
```
flutter run
```

Caso queria criar um projeto novo, no terminal volte para a pasta raiz do container e digite:
```
flutter create NomeDoProjeto
```
```
cd NomeDoProjeto
```
```
flutter run
```
