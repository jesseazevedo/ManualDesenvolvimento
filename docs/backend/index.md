# Back-end  
  
Os projetos desenvolvidos pela equipe RBCIP utilizarão para _back-end_ o NodeJS com uso do Framework NestJS. Neste documento, discutiremos padrões ques serão adotados para construção desta camada bem como padrão de diretórios.  

## Estrutura de Diretórios Back-end  
  
Para tornar a experiência do desenvolvedor mais agradável, assim como no _Front-end_ adotaremos a seguinte estrutura de diretórios:  

```  
├── src  
│   ├── app.module.ts  
│   ├── main.ts  
│   ├── modules                        (Módulos da aplicação)
│   │   └── user  
│   │       ├── dto                    (data transfer objects)  
│   │       ├── entities               (entidades do TypeORM)  
│   │       ├── user.controller.ts     (camada de apresentação - controllers)  
│   │       ├── user.module.ts         
│   │       └── user.service.ts        (camada de serviço - providers)  
│   └── shared  
│       ├── constants                  (Constantes usadas pela aplicação)  
│       ├── enums                      (enums usados na aplicação)  
│       ├── helpers                    (códigos comuns a toda a aplicação)  
│       └── interfaces                 (interfaces de comunicação com outros módulos)  
├── test  
│   └── user                           (Testes para o módulo)
├── tsconfig.build.json  
└── tsconfig.json  
```

## Convenção de Nomenclatura

- Nomes de classes devem ser escritos em PascalCase. Por exemplo: **UserController, AuthService, OrderService**.
- Nomes de métodos e variáveis devem ser escritos em camelCase. Por exemplo: **getUserById(), createOrder()**.
- Os nomes de propriedades devem ser escritos em camelCase. Por exemplo: **firstName, age, address**.
- Para serviços, é recomendado que o nome termine com o sufixo Service. Por exemplo: **UserService, OrderService**.
- Para controladores, é recomendado que o nome termine com o sufixo Controller. Por exemplo: **UserController, OrderController**.
- Para repositórios, é recomendado que o nome termine com o sufixo Repository. Por exemplo: **UserRepository, OrderRepository**.
- Os nomes dos arquivos devem ser escritos em kebab-case (separados por traço). Por exemplo: **user.service.ts, order.controller.ts, user-profile.repository.ts**.
- Os nomes dos arquivos devem refletir o nome da classe contida no arquivo. Por exemplo, a classe **UserService** deve estar definida no arquivo **user.service.ts**.

## @nestjs/swagger  

Para documentar as API's, além da documentação negocial disponível para a aplicação, será disponibilizado também o Swagger. Todos os recursos desenvolvidos no âmbito do projeto deverão ter seu swagger descrito, desta forma, utilizaremos a biblioteca @nestjs/swagger.  

A biblioteca @nestjs/swagger é um módulo oficial do NestJS que facilita a documentação da API utilizando o Swagger. Com o @nestjs/swagger, é possível gerar a documentação da API de forma automática, com base nos decorators adicionados aos endpoints.  
  
O Swagger é uma ferramenta para documentação de APIs, que permite que os desenvolvedores documentem e testem suas APIs de forma fácil e padronizada. Ele permite que os desenvolvedores definam endpoints, parâmetros e respostas, além de permitir testes de chamadas API diretamente na documentação.  
  
O @nestjs/swagger fornece decorators para definir informações sobre a API, endpoints, parâmetros e respostas. Por exemplo, o decorator @ApiTags() é usado para definir as tags da API, e o decorator @ApiOperation() é usado para definir a descrição de uma operação.  
  
Além disso, o @nestjs/swagger fornece um conjunto de recursos adicionais para personalização da documentação, como a definição de esquemas de resposta e a personalização de cabeçalhos e parâmetros.  
