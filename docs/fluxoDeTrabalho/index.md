# Fluxo de trabalho

Neste módulo abordaremos o fluxo de trabalho da equipe e o uso do GIT como ferramenta de versionamento de código de forma a orquestrar de forma harmoonica o trabalho de desenvolvimento colaborativo a ser conduzido durante o processo de desenvolvimento dos códigos.  
Para o proceso de trabalho, utilizaremos o modelo/estratégia Git Flow.  
O Git Flow é uma estratégia para organizar o fluxo de trabalho publicada em 2010, pelo engenheiro de software holandês Vincent Driessen. O Objetivo é padronizar  e organizar as branches dentro dos repositórios e, desta forma, dar fluidez ao processo de desenvolvimento de novas funcionalidades, correções de bugs e lançamentos de versões. Seu uso é recomendado para projetos que utilizam versionamento semântico ou que precisam oferecer suporte a várias versões do seu código.

## Como funciona o Git Flow

O Git Flow trabalha com duas branches principais, a Develop e a Master, que duram para sempre; e três branches de suporte, Feature, Release e Hotfix, que são temporários e duram até realizar o merge com as branches principais. De forma simplificada a branch master funciona como o repositório da versão estável do sistema, é ideal que todos os commits na branch master sejam marcados (tageados) com um número de versão. A Branch Developer atua como uma branch de integração para recursos. Abaixo temos um modelo conceitual do que abordamos no texto.  

![Git Flow](../assests/img/gitFlow.png)

## Estratégia de nomenclatura

Considerando o exposto, teremos sempre duas branches que serão mantidas durante todo o decorrer do projeto, as branchs main e develop. Haverão no entando outras 2 branches que nascerão a medida que
