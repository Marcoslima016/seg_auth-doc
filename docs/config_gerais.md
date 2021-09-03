

 Nesse tópico serão abordadas as configurações gerais para implementar um modulo de autenticação via Seg Auth. 


# Arquitetura

O primeiro passo é organizar a arquitetura e estrutura de pastas do nosso modulo de autenticação. O modulo de autenticação é organizado seguindo o padrão geralmente utilizadas em outros modulos, baseado no design pattern MVC. A estrutura de pastas deve ficar da seguinte forma: 



``` 
├── login
│   └── login.controller.dart
│   └── login.view.dart
├── cadastro
│   └── cadastro.controller.dart
│   └── cadastro.view.dart
```