# Calculadora Aritmética Dinâmica

Este projeto apresenta uma calculadora aritmética interativa desenvolvida com tecnologias web fundamentais. A aplicação foca na manipulação direta do Document Object Model (DOM) para realizar operações matemáticas em tempo real, utilizando uma interface minimalista com alto contraste.

## Especificações Técnicas

A aplicação foi construída utilizando uma arquitetura front-end leve:

1. **HTML5:** Estruturação da interface utilizando tabelas para o alinhamento preciso do teclado numérico e operadores.
2. **CSS3:** * Estilização baseada em gradientes lineares (45deg).
   * Posicionamento absoluto com transformações dinâmicas para centralização em diferentes viewports.
   * Feedback visual de interatividade através de estados de pseudo-classe (:hover).
3. **JavaScript (ES6):**
   * Manipulação de strings para gerenciamento do visor.
   * Utilização da função `eval()` para processamento de expressões matemáticas complexas.
   * Implementação de funções de edição (backspace e clear).

## Funcionalidades Implementadas

* **Operações Básicas:** Soma, subtração, multiplicação e divisão.
* **Sistema de Edição:** Função para apagar o último caractere inserido e função de limpeza total do visor.
* **Lógica de Interface:** O visor detecta entradas vazias e fornece feedback visual ("Nada...") para evitar erros de execução.
* **Layout Responsivo:** Otimizado para centralização automática em qualquer resolução de tela.

## Lógica de Execução

O script JavaScript gerencia o fluxo de dados da seguinte forma:

* **insert(num):** Captura o valor atual do visor e concatena o novo dígito ou operador.
* **back():** Utiliza o método `substring` para remover o último elemento da string do visor.
* **calcular():** Avalia a expressão aritmética completa contida na string e renderiza o resultado final no visor.

## Como Executar

Por ser uma aplicação estática (Client-Side), não requer instalação de dependências ou servidores:

1. Baixe o arquivo HTML do repositório.
2. Execute o arquivo em qualquer navegador moderno.

## Estrutura do Arquivo

* **Fundo:** Camada de gradiente de tela cheia (100vh).
* **Calculadora:** Container com efeito de transparência e bordas arredondadas.
* **Display:** Visor com alinhamento à direita para melhor legibilidade numérica.
* **Script:** Lógica funcional isolada para manipulação dos eventos de clique.
