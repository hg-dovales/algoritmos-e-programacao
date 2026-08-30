As **estruturas de dados** são formas de organizar e armazenar dados para que possam ser acessados, modificados e processados de maneira adequada durante a execução de um programa.

Um **dado** representa uma informação que pode ser armazenada e manipulada pelo programa. O **tipo de dado** determina quais valores podem ser armazenados, como esses valores são interpretados 
e quais operações podem ser realizadas sobre eles.

Uma estrutura de dados permite realizar diferentes operações, como:

- Inserir dados;
- Acessar dados;
- Buscar informações;
- Alterar valores;
- Remover elementos;
- Percorrer os dados;
- Ordenar;
- Agrupar;
- Contar elementos.

As estruturas podem ser classificadas de diferentes maneiras.

### Estruturas homogêneas

Armazenam elementos do **mesmo tipo**.

Exemplos:

    int[] idades;
    double[] notas;

### Estruturas heterogêneas

Permitem representar informações compostas por dados de diferentes tipos.

Por exemplo, um aluno pode possuir:

    nome
    idade
    nota

Em Java, objetos e classes podem ser utilizados para representar esse tipo de informação.

As estruturas também podem possuir tamanho **fixo** ou **variável**.

Um **array** possui tamanho definido no momento de sua criação:

    double[] notas = new double[10];

Já estruturas como `ArrayList` podem aumentar ou diminuir sua quantidade de elementos durante a execução.

Existem diferentes estruturas para diferentes necessidades:

- **Array:** sequência de elementos do mesmo tipo e tamanho fixo;
- **Matriz:** organiza dados utilizando linhas e colunas;
- **ArrayList:** lista cuja quantidade de elementos pode variar;
- **HashSet:** conjunto utilizado quando não queremos elementos duplicados;
- **HashMap:** associa uma chave a um valor;
- **Queue:** organiza elementos seguindo uma ordem de atendimento.

Por exemplo:

    7 temperaturas da semana → Array

    Alunos × disciplinas → Matriz

    Quantidade variável de pedidos → ArrayList

    Códigos sem repetição → HashSet

    Produto localizado pelo código → HashMap

    Ordem de chegada de clientes → Queue

Não existe uma única estrutura de dados ideal para todas as situações. A escolha depende das características do problema.

Alguns critérios importantes são:

- Formato dos dados;
- Quantidade de elementos;
- Necessidade de crescimento;
- Necessidade de manter uma ordem;
- Possibilidade ou não de elementos duplicados;
- Frequência de inserções, buscas, alterações e remoções;
- Forma como os dados precisam ser acessados.

Portanto, estudar estruturas de dados significa aprender **como organizar os dados de um programa e escolher a estrutura mais adequada para as operações que precisam ser realizadas sobre eles**.
