O **pseudocódigo** é uma forma estruturada de representar um algoritmo utilizando uma escrita próxima de uma linguagem de programação, sem depender da sintaxe específica de uma linguagem como Java.

Uma estrutura básica pode utilizar:

- **ALGORITMO / FIM_ALGORITMO:** delimitam o algoritmo;
- **VAR / FIM_VAR:** delimitam a declaração das variáveis;
- **LEIA:** representa a entrada de dados;
- **ESCREVA:** representa a saída de dados;
- **<-:** representa a atribuição de um valor a uma variável;
- **//:** representa um comentário.

Exemplo:

    ALGORITMO Calculo_do_Frete
        VAR
            precoBase: REAL
            taxaFixa: REAL
            precoFinal: REAL
        FIM_VAR

        taxaFixa <- 10
        LEIA precoBase
        precoFinal <- precoBase + taxaFixa
        ESCREVA precoFinal
    FIM_ALGORITMO

O pseudocódigo permite organizar e verificar a **lógica da solução** antes de transformá-la em código de uma linguagem de programação.
