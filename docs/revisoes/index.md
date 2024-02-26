# Estratégia de Revisão de Código

Para que uma feature possa ser incorporada a branch main ele deverá atender aos requisitos de qualidade descritos neste documento e definidos pelo líder técnico da equipe.  
O processo de revisão abordará 3 pilares que culminarão na incorporação (ou não) de uma feature a branch main, conforme segue:  
  
1. **Testes Automatizados**: Uma feature só é elegível a merge se apresentar ao menos testes relacionados ao fluxo básico e fluxos alternativos daquilo que se propõe a implementar. Além disso, deverá passar em todos os testes já disponíveis na aplicação.  
2. **Revisão de código:**: O código deverá passar por uma revisão do líder técnico da equipe de desenvolvimento, que deverá zelar pela qualidade do código e pelos padrões descritos neste documento.  
3. **Revisão Negocial:** O código deverá ser avaliado pela equipe de negócio da aplicação que será responsável por executar os testes de usuário. Apenas após realizados os testes de usuário e aprovado pela equipe de negócio, uma branch poderá ser mergeada.  
  
Abaixo, segue figura com esquema de revisão:  

![Fluxo de Revisão](../assests/img/revisão%20de%20código.png)  

## Testes automatizados  
  
Para os testes, será priorizado a adoção de testes e2e (end to end) que deverão cobrir o fluxo básico e fluxos alternativos da feature proposta. Quanto a inclusão de testes unitários, os mesmos poderão ser adicionados mediante necessidade identificada pelo desenvolvedor/líder técnico. É importante pontuar que não definiremos aqui um valor mínimo de cobertura para o código uma vez que a ideia é naõ tornar custoso o processo de desenvolvimento.  
Para exemplificar, imaginemos a funcionalidade "Manter Localização Física", o Fluxo Básico da feature em questão envolve:  

1. Consultar localização física.
2. Criar uma localização física.
3. Alterar uma localização física.
4. Desativar uma localização física.  

Os fluxos Alternativos poderiam ser:  

1. Retorna erro ao tentar criar localização física existente.
2. Retorna mensagem de alerta ao desativar localização física com item armazenado.
3. Retorna mensagem de alerta ao alterar o nome de uma localização física em uso.
4. Retorna mensagem de insucesso ao não encontrar a localização física pesquisada.  
  
No exemplo em tela, deverão estar presentes no mínimo 1 teste para cada um dos fluxos descritos acima.  

## Revisão do líder técnico  

O Líder técnico deverá primar pela qualidade de código descrita, devendo observar o atendimento da existência dos testes, padrão de diretórios conforme descrito neste documento e boas práticas a ser adotada por ele. A negativa de uma MR deverá ser acompanhada de uma descrição clara das melhorias que deverão ser realizada bem como a atribuição da responsabilidade ao respectivo desenvolvedor que irá implementar as melhorias.  

## Revisão Negocial  

Deverá ser conduzido pelo analista de negócio em parceria com o PO da aplicação. Deverá ser conduzida com base na documentação negocial. A reprovação de uma feature deverá ser acompanhada de uma descrição detalhada do que precisa ser feito e definido, em parceria com o líder técnico, o responsável pelo responsável por implementar as correções/melhorias identificadas.  
