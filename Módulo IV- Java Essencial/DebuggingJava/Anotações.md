# Debugging Java

- processo de encontrar e corrigir os bugs é chamada de debugging ou depuração.

- É uma tarefa deifícil e trabalhosa, e a dificuldade varia de acordo com o ambiente de desenvolvimento

- Existem duas grandes categorias que englobam a natureza do erro:

- **Erros de Sintaxe:**
  
  - É um erro de regras estabelecidade da linguagem:    
    
    - Parênteses, chaves, colchetes que abrem mas não fecham.
    
    - Duas intruções sem um ponto e vírgula entre elas;
    
    - III. Uma palavra-chave sendo usada numa posição inesperada.

- **Erros de Semântica:**
  
  - É um erro na "lógica do código", em sua semântica, o código está sintaticamente correto, porém não faz o que se esperava dele.
    - Tentar dividir um número por uma String ou por zero.
    - Atribuir um valor incoerente a um tipo de dado. Por exemplo: int n = "Alexandre".
    - Tentar fechar um arquivo que não foi aberto.
      
          
      
         

# Pilha de Execução de um Programa Java/Stack Trace

**Pilha de Execução:**

Toda invocação de método é empilhada em uma estrutura de dados que isola a área de memória de cada um. Quando um método termina (retorna), ele volta para o método que o invocou

**Stack Trace:**

É a matriz onde encontramos a pilha de execução da exceção. Em outras palavras, podemos dizer que o rastreamento da pilha busca( rastrio) para a próxima linha onde a exceção pode surgir.
