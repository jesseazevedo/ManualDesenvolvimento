# Framework Scrum

## Reunião de planejamento (Sprint Planning)
**Duração:** 4 horas - das 14h ~ 18h  
Realizada na primeira segunda-feira da sprint  
  
[**Planning Poker**](https://planningpokeronline.com/)  
Pontuação Planning Poker  
1 = 1h ou menos  
2 = um período (uma manhã, uma tarde, etc)  
3 = um dia  
5 = dois dias  
8 = uma semana  

## Reunião diária (Daily)
**Duração:** 15 minutos - das 9h ~ 9h15  
Realizada todos os dias, exceto nos dias de planejamento e review  
  
**Perguntas:**  
- O que foi feito?  
- O que será feito?  
- Algum impedimento?  

## Review
**Duração:** 1 hora - das 14h ~ 15h  
Realizada na última sexta-feira da sprint

## Retrospectiva
**Duração:** 1 hora - das 15h30 ~ 16h30  
Realizada na última sexta-feira da sprint  
  
[**Metodologia 4L**](https://www.atlassian.com/team-playbook/plays/4-ls-retrospective-technique)  
**O que amamos?**  
- Quais foram os aspectos positivos do sprint?  
- O que funcionou bem e queremos manter?  
- Quais foram os momentos de sucesso e celebração?  
  
**O que não gostamos?**  
- Quais recursos, ferramentas ou processos nos faltaram?  
- O que poderia ter sido melhorado para facilitar nosso trabalho?  
- Como podemos suprir essas necessidades no futuro?  
  
**O que aprendemos?**  
- Quais lições tiramos do sprint?  
- Que novos conhecimentos e habilidades adquirimos?  
- Como podemos aplicar essas lições no futuro?  
  
**O que desejamos?**  
- Quais são nossos objetivos para o próximo sprint?  
- O que queremos alcançar e como podemos melhorar?  
- Quais são nossas expectativas para o futuro do projeto?  


## Histórias de Usuário (HU) - modelo

**Descrição**  
- Inserir descrição para complementar as informações sobre a funcionalidade que será desenvolvida  

**Tarefas**  
- [ ] [insira a tarefa aqui]

**Critério de aceite (BDD - Dado, Quando, Então, E, Mas)**  
- **Given (pt: Dado)**: Utilizado para especificar uma pré condição, dentro desse step é feita a validação de uma condição antes de se prosseguir para os próximos passos. Por se tratar de uma pré condição, normalmente vem escrito no passado;  
- **When (pt: Quando)**: Utilizado quando será executada uma ação de que se espera uma reação vinda do sistema, que será validada no step “Then”. Este passo vem escrito no presente;  
- **Then (pt: Então)**: Valida se o esperado aconteceu. Segue sempre um passo do tipo “Quando”, pois aqui é validada a reação da ação recebida. Por se tratar do resultado esperado, normalmente vem escrito na forma de futuro próximo;  
- **And (pt: E)**: Caso seja necessário mais uma interação com o sistema para complementar um fluxo, mas que não necessariamente se trata de uma ação ou reação, se utiliza “And”;  
- **But (pt: Mas)**: No geral serve a mesma funcionalidade do “And”, porém é normalmente utilizado após uma validação negativa depois do “Then”;  

Caso tenha mais de 5 cenários BDD, quebrar a HU em duas ou mais histórias  

**Definição de pronto**  
- A funcionalidade deve estar completa e funcional.  
- Todos os critérios de aceite devem ser atendidos.  
- A história deve ter sido testada e validada.  
- A documentação da história deve estar completa.  

**Modelo de Dados**  

| Nível | Atributo | Descrição | Cardinalidade | Tipo de dado | Tamanho | Formato | Obrigatoriedade |
| ----- | -------- | --------- | ------------- | ------------ | ------- | ------- | --------------- |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

**Design conceitual**  
- Inserir os desenhos ou protótipos de tela