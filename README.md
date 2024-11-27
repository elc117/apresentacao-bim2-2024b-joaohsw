# Classe Array da libGDX
O LibGDX é um framework open-source para o desenvolvimento de jogos e aplicações multimídia em Java. A classe Array da LibGDX é uma implementação própria de uma lista dinâmica, projetada para oferecer melhor desempenho em comparação com coleções padrão do Java, como ArrayList. Ela é otimizada para situações comuns em jogos, nas quais operações como adição, remoção e iteração de elementos precisam ser rápidas e eficientes.
# Relacionando com conceitos de POO
O primeiro conceito que fica claro ao analisar a classe é a maneira com a qual ela utiliza o conceito de ***encapsulamento*** para abstrair os detalhes internos do funcionamento de um array dinâmico. A classe Array esconde a complexidade envolvida e isso permite que o usuário foque no uso prático da classe, sem precisar se preocupar com a implementação interna. 
Exemplo:
```java 
Array<String> nomes = new Array<>();
nomes.add("Joao"); 
```
Graças a classe Array, uma operação como criar um array e adicionar um elemento ao array que em outras linguagens pode ser algo chato de se lidar torna-se extremamente simples. 
Além disso, a classe utiliza o conceito de ***abstração***, fornecendo métodos intuitivos que ocultam a lógica detalhada do gerenciamento de elementos. Exemplo:
```java
if (nomes.contains("Joao", false)) {
    System.out.println("Joao está na lista!");
}
nomes.removeIndex(0);
```
A flexibilidade da classe também se destaca por sua aplicação de ***polimorfismo***, possibilitando o armazenamento de diferentes tipos de objetos com a mesma interface. Exemplo:
```java
Array<Integer> numeros = new Array<>();
numeros.add(42);
numeros.add(13);

Array<Float> decimais = new Array<>();
decimais.add(3.14f);
decimais.add(2.71f);
``` 

