
# JTaskPlanner

**Um Framework Agendador de Scripts JAVA**

## Autores

- **Pedro Daniel de Oliveira Hoeller**  
  Estudante de Bacharelado em Ciência da Computação, IFC - Campus Rio do Sul.  
  E-mail: pdanieldeoliveirahoeller@gmail.com

- **Rodrigo Curvello**  
  Orientador, Professor Rodrigo Curvello EBTT, IFC - Campus Rio do Sul.  
  E-mail: rodrigo.curvello@ifc.edu.br

## Resumo

JTaskPlanner é um framework Java voltado para a criação de agendamentos de execução de códigos programados em Java. Sua principal funcionalidade é oferecer recursos para o agendamento de tarefas, utilizando o modelo cron e um modelo próprio baseado em intervalos. O projeto destaca-se por funcionalidades como o processamento paralelo, permitindo a execução simultânea de múltiplas crons ou a combinação de um cron com outra funcionalidade principal.

O principal objetivo deste projeto foi promover o aprendizado durante o desenvolvimento, utilizando princípios de programação orientada a objetos, práticas de documentação com GIT, JavaDoc e diagramas UML. O projeto alcançou seu objetivo, apresentando uma série de funcionalidades e um nível de encapsulamento que o qualificam como um framework robusto e eficiente.

**Palavras-chave:** Cron; Agendador; Framework.

## Introdução

O JTaskPlanner foi desenvolvido durante a disciplina de Programação Orientada a Objetos II, com o objetivo de atender à demanda de agendamento de códigos em Java. Apesar da existência de diversos frameworks para agendamento de scripts no formato cron, poucos oferecem suporte para gerenciamento de agendamentos em outros formatos.

Diante dessa limitação, foi proposto o desenvolvimento de um framework em Java que fosse capaz de realizar agendamentos em diferentes formatos. Foram estabelecidas as seguintes metas:

- Desenvolvimento do framework;
- Criação de diagrama de classes UML;
- Documentação extensiva;
- Execução de testes unitários;
- Disponibilização do framework no formato `.jar`;
- Produção de um artigo referente ao projeto.

## Procedimentos Metodológicos

Ao iniciar o desenvolvimento, foi escolhido o Java como linguagem de programação. Java é amplamente utilizado em conjunto com o Maven para gerenciamento de dependências e recursos. O framework foi projetado para ser genérico, permitindo sua execução em qualquer dispositivo que implemente o Java.

O projeto foi desenvolvido seguindo os princípios do SOLID:

- **S**ingle Responsibility Principle (Princípio da Responsabilidade Única)
- **O**pen-Closed Principle (Princípio Aberto-Fechado)
- **L**iskov Substitution Principle (Princípio da Substituição de Liskov)
- **I**nterface Segregation Principle (Princípio da Segregação da Interface)
- **D**ependency Inversion Principle (Princípio da Inversão da Dependência)

### Diagrama de Classes

![Diagrama de Classes](https://www.plantuml.com/plantuml/dsvg/hLLDRzim3BtxL-ZeOCrXzouerZN0W6ujkc8xgpAJ295bGwAI5aF_-qpBTJcLpIxB8RRv-F4eFaaN4NN0rBggrsQljw1CwBpwNQdXPvoEKLqEXgl7Fa2CTeRejrG_C5Y_LQtr2U6jVTUbyDRQwAURpRVEuqx8L9fPo2-0_GnzA6ZLaoVCbWNpVUWw1zghLgFPGQmljGFVw30aHbYmUeNZse9hNb9lwEDCMO_ge5rYSIKPPJf_W81rTdckdgjvUNkdlOV0LrZT3hRFoRg6x8nDH8tMg6iRyVmsnwt6196LdfmcN7auJgzKlVGwTBPHUu3-Bda_D5Kl5Ev2TupggqS88VK8pTMZWHw7FYRszC_PvlII4Bg4VK9c7wbdSALSjuqCkmzskuMWC3yvekDUeOvyt5E5BU3DM8HtDrEACye98NUTgbAYwPLdoWiKNx6297SbbfI6dd8E0kPU9BuqIt8eovofas4cl0hUPEL94JCLrAH5BjUkxHsWVd2mJfW2dFyS75TAnoTlriaRchv4VPapmYEOXC0wP-0nM8JhOTRttTewa3O19PtqOqbt6srWRE0BeBQEe9ahBpZdOdAaC4cBNhV0h2mxLM_6Lr5VtuT0QPuPODcv3qjFafY_wj991V3_oCErmpc_qtnvSh3jJZ2T2FGKvs1R2kG9oSANamOq-WcdP80UD1Q-Wv6IHFL9BJyoh3mYXq_UDzNDOZXeLrEY26PHUambwtU15xQHUv2HfcB5mMPWZfJk3HllMDqYUeB-NXIX_DsqC48I1l8bBBiKT_wxzrpPRZ41eaGMYKu6X8b94YHYfpH8E8bmV15LI8TUgKDkApUsBCRa1ybjj8iCpTMppeLBGDwBfLTnVZBak0DVinAB_tUWCEabUKPaPys_5KkMl7p1POHpvwFbGpWvtEoHnvjV-O1VqELobIbL-GRBbemMDhhqwO--sA5QZU5aB5HSNO1lKkl-0000](https://www.plantuml.com/plantuml/dsvg/hLLDRzim3BtxL-ZeOCrXzouerZN0W6ujkc8xgpAJ295bGwAI5aF_-qpBTJcLpIxB8RRv-F4eFaaN4NN0rBggrsQljw1CwBpwNQdXPvoEKLqEXgl7Fa2CTeRejrG_C5Y_LQtr2U6jVTUbyDRQwAURpRVEuqx8L9fPo2-0_GnzA6ZLaoVCbWNpVUWw1zghLgFPGQmljGFVw30aHbYmUeNZse9hNb9lwEDCMO_ge5rYSIKPPJf_W81rTdckdgjvUNkdlOV0LrZT3hRFoRg6x8nDH8tMg6iRyVmsnwt6196LdfmcN7auJgzKlVGwTBPHUu3-Bda_D5Kl5Ev2TupggqS88VK8pTMZWHw7FYRszC_PvlII4Bg4VK9c7wbdSALSjuqCkmzskuMWC3yvekDUeOvyt5E5BU3DM8HtDrEACye98NUTgbAYwPLdoWiKNx6297SbbfI6dd8E0kPU9BuqIt8eovofas4cl0hUPEL94JCLrAH5BjUkxHsWVd2mJfW2dFyS75TAnoTlriaRchv4VPapmYEOXC0wP-0nM8JhOTRttTewa3O19PtqOqbt6srWRE0BeBQEe9ahBpZdOdAaC4cBNhV0h2mxLM_6Lr5VtuT0QPuPODcv3qjFafY_wj991V3_oCErmpc_qtnvSh3jJZ2T2FGKvs1R2kG9oSANamOq-WcdP80UD1Q-Wv6IHFL9BJyoh3mYXq_UDzNDOZXeLrEY26PHUambwtU15xQHUv2HfcB5mMPWZfJk3HllMDqYUeB-NXIX_DsqC48I1l8bBBiKT_wxzrpPRZ41eaGMYKu6X8b94YHYfpH8E8bmV15LI8TUgKDkApUsBCRa1ybjj8iCpTMppeLBGDwBfLTnVZBak0DVinAB_tUWCEabUKPaPys_5KkMl7p1POHpvwFbGpWvtEoHnvjV-O1VqELobIbL-GRBbemMDhhqwO--sA5QZU5aB5HSNO1lKkl-0000)](https://www.plantuml.com/plantuml/dsvg/hLLDRzim3BtxL-ZeOCrXzouerZN0W6ujkc8xgpAJ295bGwAI5aF_-qpBTJcLpIxB8RRv-F4eFaaN4NN0rBggrsQljw1CwBpwNQdXPvoEKLqEXgl7Fa2CTeRejrG_C5Y_LQtr2U6jVTUbyDRQwAURpRVEuqx8L9fPo2-0_GnzA6ZLaoVCbWNpVUWw1zghLgFPGQmljGFVw30aHbYmUeNZse9hNb9lwEDCMO_ge5rYSIKPPJf_W81rTdckdgjvUNkdlOV0LrZT3hRFoRg6x8nDH8tMg6iRyVmsnwt6196LdfmcN7auJgzKlVGwTBPHUu3-Bda_D5Kl5Ev2TupggqS88VK8pTMZWHw7FYRszC_PvlII4Bg4VK9c7wbdSALSjuqCkmzskuMWC3yvekDUeOvyt5E5BU3DM8HtDrEACye98NUTgbAYwPLdoWiKNx6297SbbfI6dd8E0kPU9BuqIt8eovofas4cl0hUPEL94JCLrAH5BjUkxHsWVd2mJfW2dFyS75TAnoTlriaRchv4VPapmYEOXC0wP-0nM8JhOTRttTewa3O19PtqOqbt6srWRE0BeBQEe9ahBpZdOdAaC4cBNhV0h2mxLM_6Lr5VtuT0QPuPODcv3qjFafY_wj991V3_oCErmpc_qtnvSh3jJZ2T2FGKvs1R2kG9oSANamOq-WcdP80UD1Q-Wv6IHFL9BJyoh3mYXq_UDzNDOZXeLrEY26PHUambwtU15xQHUv2HfcB5mMPWZfJk3HllMDqYUeB-NXIX_DsqC48I1l8bBBiKT_wxzrpPRZ41eaGMYKu6X8b94YHYfpH8E8bmV15LI8TUgKDkApUsBCRa1ybjj8iCpTMppeLBGDwBfLTnVZBak0DVinAB_tUWCEabUKPaPys_5KkMl7p1POHpvwFbGpWvtEoHnvjV-O1VqELobIbL-GRBbemMDhhqwO--sA5QZU5aB5HSNO1lKkl-0000))

## Resultados e Discussão

O JTaskPlanner é uma biblioteca com escopo fechado, seguindo os princípios do SOLID, tornando-se aberto para extensões e fechado para modificações diretas. A documentação foi realizada utilizando JavaDoc, garantindo clareza e acessibilidade.

### Exemplos de Uso

- **Tarefa:** Define uma tarefa a ser executada.

```java
public class TarefaTeste implements TaskDetail {
    @Override
    public void execute() {
        System.out.println("Teste script");
    }
}
```

- **Task:** Cria uma nova tarefa utilizando o `TaskBuilder`.

```java
Task task = TaskBuilder.newTask()
    .rename("Tarefa de teste")
    .setTask(new TarefaTeste());
```

- **Timer:** Gerencia o tempo de execução de uma tarefa.

```java
TimerBuilder.newTimer()
    .interval(1000)
    .repeat(10);
```

- **Trigger:** Cria uma execução baseada em tempo para uma tarefa específica.

```java
Trigger trigger = TriggerBuilder.newTrigger()
    .rename("Nova tarefa")
    .when(
        TimerBuilder.newTimer()
            .interval(1000)
            .repeat(10)
    );
```

- **Planner:** Associa uma tarefa a um trigger e define o plano de execução.

```java
PlanBuilder.newPlanner()
    .setOutput("./logs/")
    .planTask(trigger, task)
    .start();
```

- **Execução contínua:** Garante que o código continue rodando após a finalização do método principal.

```java
PlanBuilder.keepRunning();
```

## Considerações Finais

O desenvolvimento do JTaskPlanner demonstrou a eficácia dos princípios de Programação Orientada a Objetos no desenvolvimento de frameworks Java. A documentação extensiva e a aplicação rigorosa dos princípios do SOLID resultaram em um framework robusto, preparado para evoluir conforme as demandas futuras.

## Referências

- [IBM. Java: O que é, história, benefícios, aplicações e recursos](https://www.ibm.com/br-pt/topics/java)
- [ALURA. O que é SOLID? Princípios da Programação Orientada a Objetos](https://www.alura.com.br/artigos/solid)
- [WIKIPÉDIA. Javadoc](https://pt.wikipedia.org/wiki/Javadoc)
- [ORACLE. Javadoc - Windows Command Reference](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javadoc.html)
