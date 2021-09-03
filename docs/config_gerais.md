

 Nesse tópico serão abordadas as configurações gerais para implementar um modulo de autenticação via package Seg Auth. 


## Dependências

&emsp;Clone os repositórios dos packages ``seg_app`` e ``seg_auth``, através do github. 

&emsp;No arquivo ``pubspec.yaml``, instale os packages, indicando o diretório onde os packages foram clonados. Por exemplo: 

``` yaml
dependencies:

  seg_app: 
    path: ../../../seg_packages/projeto-seg_app/seg_app

  seg_auth: 
    path: ../../../seg_packages/projeto-seg_auth/seg_auth
``` 

<br/>

## Arquitetura

   &emsp;Depois de instalar todas as dependencias, o próximo passo é organizar a arquitetura e estrutura de pastas do nosso modulo de autenticação. O modulo de autenticação é organizado seguindo o padrão geralmente utilizadas em outros modulos, baseado no design pattern MVC. A estrutura de pastas deve ficar da seguinte forma: 



``` 
├── login/
│   └── login.controller.dart
│   └── login.view.dart
├── cadastro/
│   └── cadastro.controller.dart
│   └── cadastro.view.dart
├── models/

```

   &emsp; O modulo é dividido em dois grupos: ``login`` e ``cadastro``. Cada grupo segue o design pattern MVC, ou seja, é composto de uma camada view e de outra camada controller. Além desses dois grupos, o modulo contém a pasta referente a camada models, essa pasta irá conter models que são utilizados quando há a necessidade de uma maior personalização, por exemplo o model de um usuário que contém parametros além do model de usuário default. <br/>
   &emsp; Essa é a estrutura minima necessária, mas dependendo do projeto pode ser necessário utilizar dentro do grupo outros tipos de pastas genéricas, como por exemplo pasta widgets, components, etc. 