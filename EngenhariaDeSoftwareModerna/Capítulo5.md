# Capítulo 5

"The most fundamental problem in computer science is problem decomposition: how to take a complex problem and divide it up into pieces
that can be solved independently. - John Ousterhout"

## 5.1 Introdução

## 5.4 Coesão

- "A implementação de qualquer classe deve ser coesa, isto é, toda classe deve implementar uma única funcionalidade ou serviço."

## 5.5 Acoplamento

- "Acoplamento é a força (strenght) da conexão entre duas classes."

- O autor do livro traz dois contextos de acoplamento, a saber, o acoplamento aceitável e o acoplamento ruim.

- O que define esse limite entre o aceitável e o ruim é o nível de estabilidade entre as classes dependentes.

- "Maximize a coesão das classes e minimize o acoplamento entre elas.".

## 5.6 SOLID e Outros Princípios de Projeto

* Responsabilidade única -> Coesão
* Segregação de Interfaces -> Coesão
* Inversão de Dependências -> Acoplamento
* Prefira Composição a Herança -> Acoplamento
* Demeter -> Ocultamento de Informação
* Aberto/Fechado -> Extensibilidade
* Substituição de Liskov -> Extensibilidade

### Responsabilidade Única

- "Esse princípio é uma aplicação direta da ideia de coesão. Ele propõe o seguinte: toda classe deve ter uma única responsabilidade."

### Princípio da Segregação de Interfaces

- As interfaces não devem ter métodos não utilizados pela classe que a implementa. Isso retoma o conceito de coesão.

### Princípio de Inversão de Dependências

- "...em vez de depender de classes concretas, clientes devem depender de interfaces. Portanto, um nome mais intuitivo para o princípio seria Prefira Interfaces a Classes."

### Prefira Composição a Herança

- Não é proibido usar herança, mas esta gera um alto acoplamento entre as classes.

### Princípio de Demeter (Principle of Least Privilege)

- Quatro casos nos quais métodos podem invocar outros métodos:

    a) "de sua própria classe"
    b) "de objetos passados como parâmetros"
    c) "de objetos criados pelo próprio método"
    d) "de atributos da classe do método"

### Princípio Aberto/Fechado

- "uma classe deve estar fechada para modificações e aberta para extensões."

### Princípio de Substituição de Liskov

- As subclasses realizando um método herdado da classe pai não deve alterar o resultado final.

## 5.7 Métricas de Código Fonte

- Tamanho (LOC = Lines of Code)
- Tamanho (número de métodos, número de atributos, número de classes, número de pacotes)
- Coesão (LCOM - Lack of Cohesion Between Methods)
- "LCOM parte do pressuposto que, em uma classe coesa, qualquer par de métodos deve acessar pelo menos um atributo em comum. Ou seja,
 o que dá coesão a uma classe é o fato de seus métodos trabalharem com os mesmos atributos.".
- Acoplamento (CBO - Coupling Beetween Objects)
- Complexidade (CC - Complexidade Ciclimática)