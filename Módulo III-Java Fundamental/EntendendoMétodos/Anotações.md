# Anotações 

###### - Conceituação:

"É uma porção de código(sub-rotina) que é disponibilizada por uma classe. Este é executado quando é feita uma requisiçãoa ele.São responsáveis por definir e realizar um determinado comportamento."



###### Criação:

   <?visibilidade?><?tipo?><?modificador?> retorno nome (<?parâmetros?>)<?exceções?> corpo

- **V**: "public", "protected" ou "private"

- T: concreto ou abstrato

- M: "static" ou "final"

- **R**: tipo de dado ou "void"

- **N**:nome que é fornecido ao método

- **P**:parâmetros que pode receber

- E: exceções que pode lançar

- **C**: código que possui ou vazio



###### Particularidade

- Assinatura: é a forma de identificar unicamente o método
  
      Ass=nome +parâmetros
  
  
  
      **Método:** 

            public double calcularTotalVenda(double precoItem1, double precoItem2, double precoItem3){



}

            **Assinatura:**

            calcularTotalvenda(double precoItem1, double precoItem2, double precoItem3)



- Construtor e Destrutor: são métodos especiais usadados na Orientação a Objetos.

- Mensagem: é o ato de solicitar ao método que o mesmo execute. Esta pode ser direcionada a um objeto ou a uma classe.

- Passagem de parâmetros:
  
  - Por valor(cópia)
  
  - Por referência(endereço)



###### Boas práticas

- Nomes devem ser descritivos, mas curtos

- Notação camelo
  
  verificarSaldo(); executarTransferencia(); existeDebito();

- Deve possur entre 80 e 120 linhas

- Evite lista de parâmetros longas

- Visibilidades adequadas



###### - Sobrecarga:

###### Conceituação:

"É a capacidade de definir métodos para diferentes contextos, mas

preservando seu nome."



###### Criação

**Alterar a assinatura do método:**

    **Ass=nome + parâmetros**



converterParaInteiro(float f);

converteParaInteiro(double d);

converterParaInteiro(String s);



###### - Retornos

-  É uma instrução de interrupção

- Simbologia: return

###### Funcionamento

**O método executa seu retorno quando:**

- Completa todas suas intruções internas

- Chega a uma declaração explicita de retorno

- Lança uma exceção



###### Considerações

- O tipo de retorno do método é definido na sua criaçõa e pode ser um tipo primitivo ou objeto;

- O tipo de dado do return deve ser compatível com o deo método;

- Se o mérodo for sem retorno(void), pode ou não ter um "return" para encerrar sua execução.
