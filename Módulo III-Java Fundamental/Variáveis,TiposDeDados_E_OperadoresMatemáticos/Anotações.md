# Anotações

### - Variáveis:

- #### Conceituação

"Um espaço na memória do computador, onde se pode armazenar valores"

- Instância: Objeto

- Classe: classe

- Local: dentro de métodos

- Parâmetro: Na assinatura do método
  
  ###### Padrão de definição :
  
  <?visibilidade?>
  
  <?modificador?>
  
   tipo nome < ?=valorInicial?>;
  
  V:"public", "protected" e "private"

        M: "static" e "final"

        T: tipo de dado

        N:nome que é fornecido a variável

        VI: um valor inicial ,caso deseje

###### Converções e regras:

- Não devem começar com números;

- Embora permitido,"$" e "_" devem ser evitados;

- São case-sensitive (c e C são diferentes);

- Sem espaços;

###### Boas práticas

- Sempre começar com letra minúscula;

- Nomes expressivos;

- Notação camelo;

- Quando constante(final) maiúscula e separado por "_";

#### -Tipos de dados

###### Conceituação:

    "São os valores e consequentemente operações que as variáveis

                                            podem assmir e sofre, respectivamente."

###### Tipificação:

- Estática(forte) vs Dinâmica(fraco)

- Primitivo vs Composto

###### Opções de tipos:

- Textual

- Numeral

- Lógico

- Objeto

###### Exemplos numeral:

- byte: -128 até 127 => byte b =15;

- short: =32.768 até 32.767 => short s = -15785;

- int -2.147.483.648 até 2.147.483.647 => int i = 8515785;

- long : -9.223.372.036.854.775.808 até 9.223.372.036.854.775.807 =>  long l = 5938515785L;

- float:  +- 9.40282347E+38F => float f = 3.14... (f);

- double +- 1.79769313486231570E+308 => double d = 2.14... (d);

###### Exemplos textual:

- char: caracteres de 16-bit unicode => char c= '/u0084'; ou char c ='T' ;

- String: um tipo " especial" => String s = "T";

###### Exemplos lógico:

- boolean: true e false => boolean s = false;

    

###### Utilização:

| Tipo de dado      | Valor default |
| ----------------- |:------------- |
| byte              | 0             |
| short             | 0             |
| int               | 0             |
| long              | 0L            |
| double            | 0.0d          |
| char              | '/u0000'      |
| String(e objetos) | null          |
| boolean           | false         |

### - Operadores Aritméticos:

###### Conceituação:

"São simbolos especiais quais são capazes de realizar ações 

específicas em um, dois ou mais operandos e, em seguida,

                                                                 retornar um resultado."



###### Tipos:

- pós-fixado: exp++ ou exp--

- prefixado: ++exp --exp

- aritmético: +, - , *, /, e %

- atribuição: =, +=, -=,*=, /= e %=  

###### Precedências:

| Operador       | Precedência       |
| -------------- | ----------------- |
| Pós fixado     | exp++, exp--      |
| Prefixado      | ++exp, --exp      |
| Multiplicativo | *, /, %           |
| Aditivo        | +, -              |
| Atribuição     | =, +=, -=, *=, %= |

### - Conversões(casting):

###### Conceituação:

    "É a transformação de uma determinada variável de tipo menos

                    específico para um tipo mais específico ou vice-versa."



###### Tipos:

- Upcast (implícito)

- Downcast (explícito)



###### Utilização:

|        | byte | short | char | int | long | float | double |
| ------ |:----:|:-----:|:----:|:---:|:----:|:-----:|:------:|
| byte   | -    | U-I   | char | U-I | U-I  | U-I   | U-I    |
| short  | D-E  | -     | char | U-I | U-I  | U-I   | U-I    |
| char   | D-E  | D-E   | -    | U-I | U-I  | U-I   | U-I    |
| int    | D-E  | D-E   | D-E  | -   | U-I  | U-I   | U-I    |
| long   | D-E  | D-E   | D-E  | D-E | -    | U-I   | U-I    |
| float  | D-E  | D-E   | D-E  | D-E | D-E  | -     | U-I    |
| double | D-E  | D-E   | D-E  | D-E | D-E  | D-E   | -      |

U-I: Upcast - Implícito         D-E: Downcast -   Explícito



###### Exmplo:

- long L; int i=10; L=i

- int; long L=100; i= (int )L;

- double d; float f =10.5d; d=f;

- float f; double d=10.5d; f=(float) d;

- int i;float f = 10.5f; **i=(int)f**;
  
  


