# Front-end  
  
Após análise do mercado atual e considerando que os presentes projetos serão mantidos também em seus estados e municípios, optamos por desenvolver o frontend usando o React.  
O React é uma popular biblioteca JS de código aberto desenvolvida pela equipe do Facebook usada para criar interfaces de usuário. Tornou-se popular por ser fácil, altamente flexível e escalável. Atualmente é largamente utilizada por grandes corporações como a Meta, Instafram e Airbnb.  
  
## Estrutura de Diretórios

Com finalidade de melhorar a experiência dos desenvolvedores, adotaremos uma estrutura de diretório para todos os projetos desenvolvidos conforme segue abaixo:  

```
├── public ==> Diretório de arquivos publicos da aplicação (exemplo: imagens estáticas, fonts, svgs...)  
│  
├── src  
│ └─ pages      ==> Diretório de páginas da aplicação  
│   ├── _app.tsx  
│   ├── _document.tsx  
│   ├── index.tsx  
│   └── home-exemplo  
│       └── index.tsx  
├── shared      ====> Geralmente definimos nesse diretórios o que é comum a aplicação  
│   ├── components  
│   │   └── Exemplo  
│   │       └── Exemplo.tsx  
│   ├── constants  
│   │   └── index.ts  
│   ├── contexts  
│   │   └── Exemplo  
│   │       └── ExemploContext.tsx  
│   ├── enums  
│   │   └── routes.enum.ts  
│   ├── guards  
│   │   └── ExemploGuard.jsx  
│   ├── hooks  
│   │   └── useExemplo.jsx  
│   ├── models  
│   │   ├── global.ts  
│   │   └── index.ts  
│   ├── services  
│   │   └── index.ts  
│   └── utils  
│       └── index.ts  
├── modules      ====> Segue mesma estrutura da pasta shared, porém com módulos funcionalidades/responsábilidade isolada  
│   ├── components  
│   ├── constants  
│   ├── contexts  
│   ├── enums  
│   ├── guards  
│   ├── hooks  
│   ├── models  
│   └─ services  
├── store.ts  
└── styles  
    └── globals.css  
```
  
- Use uma arquitetura modular para organizar a aplicação em módulos específicos.  
- Armazene os recursos compartilhados em um diretório shared, como models, services, utils, enums, etc.  
- Armazene os componentes compartilhados em um diretório shared/components.  
- Armazene as páginas principais da aplicação em um diretório src/pages.  
- Armazene os componentes específicos da feature dentro dos subdiretórios das páginas específicas da feature.  
- Evite aninhamento excessivo de diretórios para evitar problemas de legibilidade e manutenção.  

#### Organização do código

- Use interfaces para definir a forma dos objetos complexos, como modelos de dados.
- Use tipos TypeScript fortemente tipados sempre que possível para melhorar a legibilidade e evitar erros.
- Mantenha as funções e métodos o mais curtos possível, preferencialmente abaixo de 30 linhas.  
- Adote a lingua portuguesa para sua codificação.  

## Dependências

### Estilização

Para a estilização do código, utilizaremos o a biblioteca react-bootstrap. Para maiores detalhes cosnulte a documentação:  

[React Bootstrap](https://react-bootstrap.netlify.app/docs/getting-started/introduction)  
  
### Internacionalização  
  
Há perspectivas de que o código produzido no âmbito do projeto seja adotado por nações de lingua espanhola e inglesa. Desta forma, recomenda-se o uso do i18n para viabilizar a tradução dos textos no frontend. Para maiores detalhes, consulte a documentação:  
  
[i18n](https://www.npmjs.com/package/i18next)  
  
### Configuração de rotas
  
Para rotas, utilizaremos uma das bibliotecas mais conhecidas entre os desenvolvedores react, o react-router. Para conhecer mais, consulte a documentação oficial:  
  
[React Router](https://reactrouter.com/en/main)
  
### Gerenciamento de estados
  
Para gerenciar estados, utilizaremos o REDUX, uma biblioteca muito popular entre os desenvolvedores react. Para conhecer mais, consulte a documentação oficial:  
  
[Redux](https://redux.js.org/)
  
### Validação  
  
A validação de formulários será realizada com o uso da biblioteca yup. Para maiores detalhes, consulte a documentação:  
  
[YUP](https://www.npmjs.com/package/yup)  
  
### Requisições
  
Para realizar requisições, o front-end utilizará a biblioteca axios. Para conhecer, acesse a documentação:  

[AXIOS](https://axios-http.com/ptbr/docs/intro)  
  
### Outras dependências  
  
- jest (testes)  
- classnames (estilização)  
