# Por que?

PE VS POO

- Paradigma Estruturado tem uma representação mais simplista

- Paradigma Orientada a Objeto tem uma representação mais realista

- Paradigma Estruturado foca em operações(funções) e dados

- Paradigma Orientado a Objetos foca na modelagem de entidades e nas iterações entre elas

- Programação Estruturada foca mais no "como fazer"

- Programação Orientada a Objetos foca mais no "o que fazer"

Vantagens da POO

- Melhor coesão

- Melhor acoplamento

- Diminuição do GAP semântico

- Coletor de lixo

# Fundamentos

**Definição**

"A Orientação a Objetos é um paradigma de análise, projeto e programação de sistemas de software baseadp na composição e iteração entre diversas unidades de software chamadas de objetos."

- Abstração
  
  "Processo pelo qual se isolam características de um objeto, considerando os que tenham em comum certos grupos de objetos."

- Reuso
  
  "Capacidade de criar novas unidade de código a partir de outras já existentes."

- Encapsulamento
  
  "Capacidade de esconder complexidades e proteger dados."

# A estrutura

- Classe

        "É uma estrutura que abstrai um conjunto de objetos com características similares. Uma classe define o comportamento de seus objetos através de métodos e os estados possíveis destes objetos através de atributos. Em outros termos, uma classe descreve os serviços promovidos por seus objetos equais infotmações eles podem armazenar."

- Atributo

        "É o elemento de uma classe responsável por definir sua estrutura de dados. O conjunto destes será responsável por representar suas características e fará parte deos objetos criados a partir da classe."

    **Atributo x Variável**

A:O que é próprio e peculiar a alguém ou a alguma coisa.

V: Sujeito a variações ou mudanças; que pode variar; inconstante, instável

- Método

        "É uma porção de código (sub-rotina) que é disponibilizada pela classe. Este é executado quando é feita uma requisição a ele. Um método serve para identificar quais serviços, ações, que a classe oferece. Eles são responsáveis por definir e realizar um determinado comportamento"

- Objeto
  
  "Um objeto é representação de um conceito/entidade do mundo real, que pode ser física (bola, carro, árvore etc.) ou conceitual (viagem, estoque, compra etc.) e possui um significado bem definido para um determinado software. Para esse concito/entidade, deve ser definida inicialmente uma classe a partir da qual posteriormente serão instanciados objetos distintos."          

- Mensagem
  
  "É o processo de ativação de um método de um objeto. Isto ocorre quando uma requisição (chamada ) a esse método é realizada, assim disparendo a execução de seu comportamento descrito por sua classe. Pode também ser direcinada diretamente à classe, caso a requisição seja a um método estático."

# As relações

- Herança
  
  "É o relacionamento entre classe em que uma classe chamada de subclasse (classe filha, classe derivada) é uma extensão, um subtipo, de outra classe chamada de superclasse (classe pai, classe mãe, classe base). Devido a isto, a subclasse consegue reaproveitar os atributos e métodos dela. Além dos que venham a ser herdados, a subclasse pode definir seus próprios membros. "
  
  - Tipos de herança:
    
    - Simples 
      
      - A classe filha tem só uma mãe
    
    - Multiplas
      
      - A classe filha tem uma ou mais classes mães   
  
  - Polimorfismo
    
    "A mesma ação, se comportando diferente."
  
  - Sobrescrita
    
    "A mesma ação, podendo se comportar diferente."

     "Possibilita um relacionamento entre classes/objetos, no qual estes possam pedir ajuda a outras classe/objetos e reperesentar de forma completa o conceito ao qual se destinam. Neste tipo de relacionamento, as classes e os objetos interagem entre si para atingir seus objetivos."

- Associação
  
   "Possibilita um relacionamento entre classes/objetos, no qual estes possam pedir ajuda a outras classe/objetos e reperesentar de forma completa o conceito ao qual se destinam. Neste tipo de relacionamento, as classes e os objetos interagem entre si para atingir seus objetivos."
  
  - Tipos:
    - Estrutural
      -  Composição:"Com parte Todo"
        - Ex: Pessoa e Endereço
      - Agregação: " Sem Parte Todo"
        - Ex: Disciplina e Aluno
    - Comportamental
      - Dependênca: "Depende de"

- Interface
  
  "Define um contrato que deve ser seguido pela classe que a implementa. Quando uma classe implementa uma interface, ela se compromete a realizar todos os comportamentos que a interface disponibiliza."

# A organização

- Pacotes 
  
  "São uma organização dísica ou lógica criada para separar classe com responsabilidades distintas. Com isso, espera-se que a aplicação fique mais organizada e seja possível separar classes de finalidade e representatividades diferentes."

- Visibilidades 
  
  "Um modificador de acesso tem como finalidade determinar até que ponto uma classe, atributo ou método pode ser usado. A utilização de modificadores de acesso é fundamental para o uso efetivo da Orientação a Objetos. Algumas boas práticas e conceitos só são atingidos com o uso corretos deles."
  
  - Tipos:
    
    - Private: Só dentro a classe
    
    - Protected: Dentro da classe, mesmo pacote e subclasses
    
    - Public: Em qualquer lugar






