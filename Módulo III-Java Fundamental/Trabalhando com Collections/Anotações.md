# Anotações- Collections

##### Collection

- Collection é um objeto que agrupa múltiplos elementos (variáveis primitivas ou objetos) dentro de única unidade.

- Serve para armazenar e processar conjuntos de dados de forma eficiente.

- Antes do Java 2 (JDK 1.2), a implementação de coleções na linguagem Java incluía poucas classe e não tinha a organização de um framework

#### Composição Collections

- **Interfaces:** é um contrato que quando assumido por uma classe deve ser implementado.

- **Implementações de Classes:** são as materializações, a codificação das interfaces.

- **Algoritmos:** É uma sequência lógica, finita e definida de intruções que devem ser seguidas para resolver um problema.

#### - Lists

  **java.util.List** 

- Elementos duplicaod e garante ordem de inserção

"ArrayList deve ser usado onde mais operações de pesquisa são necessárias, e LinkedList deve ser usado onde mais operações de inserção e exclusão são necessárias. "

**Exemplos:**

- como criar uma lista:

-List<Double> nome = new ArrayList<>();

-ArrayList<Double> nome = new ArrayList<>();

-List<Double> nome = new ArrayList<>(Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

-List<Double> nome = Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6); --> essa forma é limitada, pois não é possivel adicionar e remover itens dentro da lista.

-List<Double> notas = List.of(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6); -> essa lista é imutavel e também não é possivel adicionar e remover.

- Métodos:

-nome.add(); --> add elementos

-nome.add(posição, elemento); --> add o elemento na posição

-System.out.println(nome); --> [  8 , 7 , 5 , 4  ,7 ]

-System.out.println(nome.toString()); -->[8, 7, 5, 4, 7]

-nome.indexOf( elemento) --> retorna a posição do elemento dentro da lista

-nome.set(posição, elemento) --> substitui o valor que esta na posição por um outro elemento que foi passdo como parametro

-nome.contains(); --> verifica se dentro da lista contem o valor informado e retorna "true" ou " false "

-nome.get(posição) --> retorna o elemento que esta na posição

-Collections.min( nome da lista) --> retorna o menor valor

-Collections.max( nome da lista) --> retorna o maior valor



**Iterator<Double> iterator = nome.iterator();**

**Double soma = 0d;**

**while( iterator.hasNext()){**

    **Double next =iterator.next();**

    **some += next;**

**}**

// soma de todos os valores dentro da lista

-nome.size(); --> retorna a quant. de elementos dentro da lista

-nome.remove(posição); --> remove o elemento da lista nessa posição

-nome.remove(elemento); --> remove o elemento dentro da lista

**Iterator<Double> iterator = nome.iterator();**

**while(itetor.hasNext()){**

   **Double next = iterator.next();**

    **if (next < 7) iterator.remove();**

**}**

//Remove todos os elementos menores do que 7 dentro da lista

-nome.clear(); --> Apaga todos os elementos dentro da lista

-nome.isEmpty(); --> Verifica se a lista esta vazia e retorna "true" ou "false"

###### Ordenação de elementos

-Collections.shuffle(Lista); --> serve para  bagunçar a lista

#### - Set

**java.util.Set**

- Não permite elementos duplicados

- Não possui índice

- Como iniciar:

-Set<Double> nome = new HashSet<>( );

-Set<Double> nome = new HashSet<>(Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

- Métodos:

-System.out.println(nome.toString());

-nome.contains(  );

-Collections.min( ) --> retorna o menor valor

-Collections.max( ) --> retorna o maior valor

-nome.size(); --> retorna a quant. de elementos dentro da lista

-nome.remove(elemento); --> remove o elemento dentro da lista

#### - Map

**java.util.Map**

- Elementos únicos (key) para cada valor (value)

- Como iniciar: 

    

-Map<TipoDaChave, TipoDoValor> nome = new HASHmAP<>( ){{

    put( , );

}}

ex:

Map<String, Double> carrosPopulares = new HashMap<>( ){{

    put("gol", 14.4);

    put("uno", 15.6);

    put("mobi", 16.1);

}}

- métodos :

-System.out.println(carrosPopulares.toString()); --> ex: {gol=14.4, uno=15.6, mobi=16.1}

-carrosPopulares.put("chave", valor); --> Como não é possivel ter chaves repetidades é possivel, colocando uma chave já existente, substituir o valor de uma chave.Ex: carrosPopulares.put("gol", 15.2);

-Substitui o valor que antes era 14.4 para 15.2.

-nome.containsKey( objeto); --> retorna true or false

-nome.get(Objeto); --> retorna o valor dentro da key que foi passada como parâmetro

-nome.keySet(); --> retorna um set.Ex:

-Set<String> modelos = carrosPopulares.keySet();

-System.out.println(modelos);--> {gol, uno, mobi}

-nome.values(); --> retorna uma Collection.Ex:

-Collection<Double> consumos = carrosPopulares.values();

-System.out.println(consumos); --> {14.4, 15.6, 16.1}

-Collections.max(carrosPopulares.values()): --> maior valor dentro do map

#### - Streams

**Classe Anônima**

    A classe anônima em Java é uma classe que não recebeu um nome e é tanto declarado e instanciado em uma única instrução. Você deve considerar o uso de uma classe anônima sempre que você precisa para criar uma classe que será instanciado apenas uma vez.

**Functional Interface**

    Qualquer interface com um SAM (Single Abstract Method) é uma interface funcional e sua implementação pode ser tratada como expressões lambda.

- Comparator

- Consumer

- Function

- Predicate

**Lambda**

    Uma função lambda é uma função sem declaração, isto é, não é necessário coloca um nome, um tipo de retorno e modificador de acesso. A idea é que o método seja declarado no mesmo lugar em que será usado. As funções lambda em Java tem a sintaxe definida como (argumento) -> ( corpo).

**Reference Method**

    Method Reference é um novo recurso do Java 8 que permite fazer referência a um método ou construtor de uma classe (de forma funcional) e assim indicar que ele deve ser itilizado num ponto específico do código, deixando-o mais simples e legível. Para utilizá-lo, basta informar uma classe ou referência seguida do símbol "::" e o nome do método sem os parênteses no final.

**Streams API**

    A Streams API traz uma nova opção para a manipulação de coleções em Java seguindo os princípios da programação fucnional. Combinada com as expressões lambda, ela proporciona uma forma diferente de lidar com conjuntos de elementos, oferecendo ao desenvolvedor uma maneira simples e concisa de escrever código que resulta em facilidade de manutenção e paralização sem efeitos indesejados em tempo de execução.
