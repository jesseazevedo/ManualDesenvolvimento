# Banco de dados

No âmbito do desenvolvimento dos projetos e-SUS AF e SisDAF, serão utilizadas o mesmo padrão de nomenclatura e mesma estratégia de migração, no entanto, a estrutura de pastas poderá mudar um pouco, posto caracteristicas específicas de cada projeto.  
  
Em especial o e-SUS AF terá um processo de migração mais cuidadoso posto a necessidade de gerenciar versões da aplicação bem como a pretensão de homologar a aplicação para os SGBD's Postgres, Oracle, MySQL e SQLServer.  

## Padrão de nomenclatura

Para a nomenclatura dos objetos de banco de dados utilizaremos o padrão definido pelo DATASUS e publicado no documento Padronização de Nomenclatura para objetos de Banco de Dados. Para saber mais, acesse os documentos logo abaixo:  
  
- [Padronização de Nomenclatura para objetos de Banco de Dados](../assests/docs/Padronizacao%20de%20Nomenclatura%20para%20Objetos%20de%20Banco%20de%20Dados%20Sugestao%20CGIIS.pdf)  
- [Cartilha de Administração de Dados](../assests/docs/Cartilha%20de%20Administracao%20de%20Dados.pdf)  
  
## Estrutura de Pastas  

Para garantir que as migrações ocorram de forma mais fluída e intuitiva, adotaremos uma estrutura de diretório rígida e com papel bem definido:  

```
├── mr                (Nesta pasta ficarão apenas os arquivos sql de features ainda não mergeadas)
│   ├── mysql
│   ├── oracle
│   ├── postgres
│   └── sqlserver
└── versions          (Este arquivo guarda versões consolidadas do banco de dados)  
    ├── mysql
    ├── oracle
    ├── postgres
    └── sqlserver
```

- Organize suas migrações no diretório MR adicionando os arquivos para cada um dos banco de dados descritos.  
- Trabalhe suas migrações em 2 arquivos distintos, onde 0 1º arquivo deve realizar todas as operações de DML necessárias a migração e o 2º arquivo deve trazer alterações em DDL.  
- Ao fim de cada sprint, o líder técnico deverá consolidar todos os arquivos produzidos em seus respectivos arquivos de versão.  

### Automação de migrações

Em breve
