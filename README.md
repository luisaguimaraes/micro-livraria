# Micro-Livraria: Exemplo Prático de Microsserviços
# Atividade desenvolvida sob orientação da Profa. Caroline Queiroz - 2020/2 - Disciplina de Engenharia de Software 2.

Este repositório contem o desenvolvimento de uma micro livraria virtual construída usando uma **arquitetura de microsserviços**.

O exemplo foi projetado para ser usado em uma **aula prática sobre microsserviços**, que pode, por exemplo, ser realizada após o estudo do [Capítulo 7](https://engsoftmoderna.info/cap7.html) do livro [Engenharia de Software Moderna](https://engsoftmoderna.info).

O objetivo da aula é permitir que o aluno tenha um primeiro contato com microsserviços e com tecnologias normalmente usadas nesse tipo de arquitetura, tais como **Node.js**, **REST**, **gRPC** e **Docker**.

Como nosso objetivo é didático, na livraria virtual estão à venda apenas três livros, conforme pode ser visto na próxima figura, que mostra a interface Web do sistema. Além disso, a operação de compra apenas simula a ação do usuário, não efetuando mudanças no estoque. Assim, os clientes da livraria podem realizar apenas duas operações: (1) listar os produtos à venda; (2) calcular o frete de envio.

## Arquitetura

A micro-livraria possui quatro microsserviços:

-   Front-end: microsserviço responsável pela interface com usuário, conforme mostrado na figura anterior.
-   Controller: microsserviço responsável por intermediar a comunicação entre o front-end e o backend do sistema.
-   Shipping: microserviço para cálculo de frete.
-   Inventory: microserviço para controle do estoque da livraria.

Os quatro microsserviços estão implementados em **JavaScript**, usando o Node.js para execução dos serviços no back-end.

No entanto, **você conseguirá completar as tarefas práticas mesmo se nunca programou em JavaScript**. O motivo é que o nosso roteiro já inclui os trechos de código que devem ser copiados para o sistema.

Para facilitar a execução e entendimento do sistema, também não usamos bancos de dados ou serviços externos.


## Comentários Finais

Nesta aula, trabalhamos em uma aplicação baseada em microsserviços. Apesar de pequena, ela ilustra os princípios básicos de microsserviços, bem como algumas tecnologias importantes quando se implementa esse tipo de arquitetura.

No entanto, é importante ressaltar que em uma aplicação real existem outros componentes, como bancos de dados, balanceadores de carga e orquestradores.