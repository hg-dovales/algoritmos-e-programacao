Um **array** é uma estrutura de dados utilizada para armazenar uma quantidade fixa de elementos do **mesmo tipo**, organizados em posições identificadas por índices.

Em Java, os índices começam em `0`. Portanto, em um array com 5 elementos, as posições válidas são de `0` até `4`.

Um array pode ser declarado e criado da seguinte forma:

    int[] numeros = new int[5];

Também pode ser inicializado diretamente com valores:

    int[] numeros = {10, 20, 30, 40, 50};

A propriedade `.length` informa a quantidade de elementos do array:

    numeros.length

A última posição(indice) de um array pode ser obtida através de:

    numeros.length - 1

Os elementos podem ser acessados e modificados através de seus índices:

    numeros[0] = 15;

Para percorrer todas as posições(elementos) de um array, podemos utilizar um `for`:

    for (int i = 0; i < numeros.length; i++) {
        System.out.println(numeros[i]);
    }

Também podemos utilizar o **for-each** quando queremos percorrer diretamente os elementos:

    for (int numero : numeros) {
        System.out.println(numero);
    }

No `for-each`, o `:` pode ser interpretado como **"em"**:

    para cada numero em numeros

Quando trabalhamos com tipos primitivos, a variável do `for-each` recebe uma cópia do valor. Portanto, alterar essa variável não modifica diretamente o elemento original do array.

Para modificar os elementos, podemos utilizar seus índices:

    for (int i = 0; i < numeros.length; i++) {
        numeros[i] = numeros[i] * 2;
    }

A classe `Arrays`, do pacote `java.util`, disponibiliza métodos úteis para trabalhar com arrays, como:

- `Arrays.toString()` — representa o conteúdo do array como texto;
- `Arrays.sort()` — ordena os elementos;
- `Arrays.binarySearch()` — realiza uma busca em um array ordenado;
- `Arrays.copyOf()` — cria uma cópia;
- `Arrays.fill()` — preenche posições com determinado valor.

---

Uma **matriz** pode ser representada em Java através de um array multidimensional, permitindo organizar dados em **linhas e colunas**.

Exemplo:

    int[][] vendas = new int[5][4];

Nesse caso:

- `5` representa a quantidade de linhas;
- `4` representa a quantidade de colunas;
- A matriz possui `20` posições.

O acesso utiliza dois índices:

    vendas[linha][coluna]

Por exemplo:

    vendas[0][0]

representa o elemento localizado na primeira linha e primeira coluna.

Uma matriz também pode ser inicializada diretamente:

    int[][] vendas = {
        {35, 18, 12},
        {40, 21, 15},
        {32, 20, 17}
    };

Cada conjunto interno representa uma **linha** da matriz.

Para percorrer uma matriz, normalmente utilizamos **laços de repetição aninhados**:

    for (int linha = 0; linha < vendas.length; linha++) {
        for (int coluna = 0; coluna < vendas[linha].length; coluna++) {
            System.out.println(vendas[linha][coluna]);
        }
    }

Nesse caso:

- `vendas.length` representa a quantidade de linhas;
- `vendas[linha].length` representa a quantidade de elementos da linha atual(colunas).

Em Java, as linhas de um array multidimensional podem possuir tamanhos diferentes, formando estruturas conhecidas como **arrays irregulares (jagged arrays)**.

Arrays e matrizes permitem armazenar e processar vários dados relacionados utilizando uma única estrutura. A principal diferença é que o **array organiza os elementos em uma dimensão**, enquanto a 
**matriz permite organizá-los em duas ou mais dimensões**, como linhas e colunas.
