As **estruturas de repetição** permitem executar um bloco de código várias vezes enquanto uma determinada condição for atendida.

Elas são utilizadas para evitar a repetição manual de instruções e são fundamentais para trabalhar com tarefas que precisam ser executadas diversas vezes.

Em Java, as principais estruturas de repetição são `for`, `while` e `do-while`.

O `for` é utilizado principalmente quando sabemos ou conseguimos determinar a quantidade de repetições:

    for (int i = 1; i <= 10; i++) {
        System.out.println(i);
    }

Sua estrutura possui três partes principais:

- **Inicialização:** define o valor inicial do contador;
- **Condição:** determina enquanto a repetição continuará;
- **Atualização:** modifica o contador após cada repetição.

O `while` é utilizado principalmente quando a quantidade de repetições não é conhecida previamente. O bloco continua sendo executado enquanto a condição for verdadeira:

    while (condicao) {
        // instruções
    }

A condição do `while` é verificada **antes** da execução do bloco. Portanto, se ela for falsa desde o início, o bloco pode não ser executado nenhuma vez.

O `do-while` também executa um bloco enquanto uma condição for verdadeira:

    do {
        // instruções
    } while (condicao);

A principal diferença é que sua condição é verificada **depois** da execução. Por isso, o bloco será executado pelo menos uma vez.

Durante as repetições, também podemos utilizar:

- **Contador:** variável utilizada para controlar ou registrar a quantidade de repetições;
- **Acumulador:** variável utilizada para armazenar resultados progressivamente, como uma soma;
- `break`: encerra completamente o laço de repetição;
- `continue`: interrompe apenas a iteração atual e segue para a próxima.

Exemplo de acumulador:

    int soma = 0;

    for (int i = 1; i <= 5; i++) {
        soma = soma + i;
    }

Também é possível utilizar **laços aninhados**, colocando uma estrutura de repetição dentro de outra. Para cada execução do laço externo, o laço interno realiza suas próprias repetições.

De forma geral:

- `for` → indicado quando a quantidade de repetições pode ser determinada;
- `while` → indicado quando não sabemos previamente quantas repetições serão necessárias;
- `do-while` → indicado quando o bloco precisa ser executado pelo menos uma vez.

As estruturas de repetição permitem controlar o **fluxo de execução** do programa, automatizando tarefas repetitivas e possibilitando o processamento eficiente de conjuntos de dados.
