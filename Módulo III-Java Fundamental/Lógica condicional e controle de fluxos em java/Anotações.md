# Anotações

### Operadores Relacionais

#### Tipos:

- Similaridade: igaul,diferente

- Tamanho:maior, maior igual, menor, menor igual

Similaridade

- Igualdade: determina se um operando é igual ao outro

- Diferença: determina se um operando não é igual ao outro

Simbologia

- Igualdade: == 

- Diferença: !=

Tamanho

- Maior: determina se um operando é maior do que outro

- Maior Igual:determina se um operando é menor ou igual a outro

Simbologia

- Menor: <

- Menor Igual: =<

### Operadores Lógicos

##### - Conceituação

"São s[imbolos especiais auais são capazes de realizar comparações lógicas entre operandos lógicos ou expressões e, em seguida, retornar um resultado"

Tipos:

- Conjunção

- Disjunção

- Disjunção exclusiva

- Negação





- Conjunção: operação lógica que só é verdadeira quando ambos os operandos ou expressões envolvidas são verdade

- Simbologia: &&

- Terminologia: and(e)

| O-E | O-E | R   |
| --- | --- | --- |
| V   | V   | V   |
| V   | F   | V   |
| F   | V   | F   |
| F   | V   | F   |



- Disjunção: operação que só é falsa quando ambos os operandos ou expressões envolvidas são falsos

- Simbologia: || 

- Terminologia: or(ou)

| O-E | O-E | R   |
| --- | --- | --- |
| V   | V   | V   |
| V   | F   | V   |
| F   | V   | V   |
| F   | F   | F   |



- Disjunção exclusiva: operação que só é verdade quando ambos os operandos ou expressões são opostos

- Simbologia:  ^

- Terminologia: xor

| O-E | O-E | R   |
| --- | --- | --- |
| V   | V   | F   |
| V   | F   | V   |
| F   | V   | V   |
| F   | F   | F   |



- Negação: operação que inverte o valor lógico de um operando ou expressão

- Simbologia: !

- Terminologia: inverção

| O-E | R   |
| --- | --- |
| V   | F   |
| F   | V   |



###### Boas práticas

- Crie variáveis auxiliares para guardar resultados intermediários



(salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes)



pode ser



(salarioBaixo) && (muitoDependentes)

boolean recebeAuxilo = (salarioBaixo) && (muitosDependenstes);



#### Controle de fluxo

##### - Conceituação

"São estruturas que tem a capacidade de direcionar o fluxo de execução do código"



Tipos: 

- Decisão: if, if-else, if-else-if, switch e operador ternário

- Repetição: for, while, do while

- Interrupção: break, continue e return



- Decisão: estrutura que avalia uma condição boleana ou variável para direcionar o fluxo de execução

- Opções: if(se), switch(escolha) e operador ternário



##### Boas práticas

- Switch é para valores exatos e if para expressões booleanas

- Evitar usar o default do switch para "case genéricos"

- Evitar o efeito"flecha" dos if's

- Evitar muitos if's aninhados

- Usar a boa prática da aula 2 para diminuir o tamanho if



### Blocos:

###### - Conceituação

"É um grupo de 0 ou mais códigos quais trabalham em conjunto para executar uma operação"

Tipos: 

- Locais:dentro de métodos

- Estáticos: dentro de classes

- Instância: dentro de classes
