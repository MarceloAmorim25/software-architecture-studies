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
