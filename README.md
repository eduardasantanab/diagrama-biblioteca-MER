# **Diagrama Entidade Relacionamento**

#### Maria Eduarda Santana da Silva Barros

#### Modelo conceitual para um sistema de gerenciamento de biblioteca

### > Diagrama desenvolvido:

<img src="diagrama-biblioteca.png"/>

#
#### Apresentação:
Neste sistema, a biblioteca oferece serviços de *empréstimo* de livros [1],  *aluguel de salas de estudos* [2], *venda* de obras literárias [3] e a realização de *eventos temáticos*, como palestras e debates [4]. Os eventos fazem parte do oferecimento da instituição em incentivar a construção do pensamento crítico para os seus consumidores, e são escolhidos a partir do *registro de avaliação* [5] que cada *pessoa* – *usuário* ou *bibliotecário* [6] – pode realizar sobre o livro, após a leitura. Assim, a obra melhor avaliada do mês será utilizada como tema para debates, dinâmicas ou palestras. 

A biblioteca estará disponível para coleta de *doações literárias* [7] de todo o público que desejar ou não realizá-la, como incentivo do núcleo de sustentabilidade da instituição para a rotatividade de obras, manutenção e enriquecimento do acervo da biblioteca.

O bibliotecário é responsável por *realizar o cadastro* [8] de livros ou usuários no sistema da biblioteca e operar a venda das obras disponíveis. Cada pessoa cadastrada recebe todo ano, na data do seu aniversário, o *benefício* [9] de um cupom com 10% de desconto, para ser usufruído no espaço da biblioteca ou em livros da livraria parceira.

Os *livros* [10] são organizados em *categorias* [11], de forma que cada livro pertence a uma categoria e cada categoria pode conter muitos livros. Essa estruturação tem o objetivo de promover o conforto do leitor que desejar identificar os livros físicos em cada endereço de sessão no espaço da biblioteca, de acordo com a categoria área de conhecimento ou a categoria gênero abordada no livro, por exemplo. 

No projeto desenvolvido, ainda, cada livro pode pertencer a 1 ou mais *autores* [12], e ser disponibilizado nos *modelos: físico; e-book; audiobook e braile*, abrangendo assiduamente os formatos com adaptações para acessibilidade. 

Em casos de compra ou empréstimo, os livros físicos podem oferecer o *serviço de entrega ou retirada* na biblioteca, se desejável [13]. Ademais, aqueles que não efetuarem a devolução na data de vencimento do empréstimo, serão penalizados com uma taxa, ou *multa*, no valor fixo de R$20. 
#

> 1. um empréstimo contém 1 ou mais livros, mas 1 livro pode estar associado a nenhum empréstimo ou a um.
  > * 1.1. um empréstimo pode estar associado a nenhuma ou a 1 multa, mas uma multa sempre está associada a 1 empréstimo.
  > * 1.2. um empréstimo pode ser realizado por 1 pessoa, mas 1 pessoa pode estar associada a nenhum ou a muitos empréstimos.
> 2. uma sala de estudo só pode ser reservada por 1 pessoa e 1 pessoa só pode ocupar a reserva de apenas 1 sala.
> 3. uma venda contém 1 ou muitos livros e 1 livro pode se associar a 1 ou muitas vendas.
  > * 3.1. um bibliotecário pode operar 1 ou mais vendas, mas 1 venda só pode ser associada a 1 bibliotecário. 
> 4. uma instituição de biblioteca pode promover nenhuma ou muitas palestras e 1 palestra pode ser promovida por no mínimo 1 ou mais instituições colaboradoras.
  >  * 4.1. uma instituição de biblioteca contém no mínimo 1 bibliotecário ou muitos, e 1 bibliotecário pode estar contido em 1 ou mais instituições (no caso de ter 2 empregos distintos).
> 5. uma pessoa pode não registrar nenhuma avaliação literária ou muitas, mas 1 avaliação sempre será referente ou registrada por 1 pessoa.
  >  * 5.1. cada (1) avaliação é referente a 1 livro, mas 1 livro pode ser referenciado por nenhuma ou muitas avaliações.
> 6. restrição de sobreposição
  >  * 6.1. um bibliotecário efetua no mínimo 1 ou muitos cadastros, de livros ou usuários, mas 1 cadastro por vez é efetuado por apenas 1 bibliotecário.
> 7. uma pessoa pode efetuar nenhuma ou muitas doações, mas 1 doação pode estar associada a 1 ou mais doadores (pessoas).
> 8. um cadastro pode se associar com 1 ou muitos usuários, mas 1 usuário só pode ser identificado por 1 cadastro.
  > * 8.1. um cadastro pode se associar com 1 ou muitos livros, mas 1 livro só pode ser identificado por 1 cadastro.
> 9. uma pessoa recebe 1 ou muitos benefícios, de acordo com o tempo de cadastro, mas 1 benefício só pode ser recebido por 1 pessoa.
> 10. um livro é publicado por 1 editora, mas 1 editora pode publicar 1 ou mais livros.
  > * 10.1. um livro tem restrições de sobreposição para os modelos: físico, e-book, audiobook e braile. Ou seja, um mesmo livro pode ter nas versões e-book, audiobook, braile e físico.
> 11. uma categoria pertence a 1 ou muitos livros, mas cada livro só pertence a 1 categoria.
> 12. um autor produz 1 ou mais livros e 1 livro pode ser produzido por 1 ou mais autores.
> 13. um livro físico pode pertencer a muitos ou a nenhum serviço de entrega/retirada, enquanto um serviço pode estar relacionado a 1 ou muitos livros físicos.
  > * 13.1. um livro em braile pode pertencer a muitos ou a nenhum serviço de entrega/retirada, enquanto um serviço pode estar relacionado a 1 ou muitos livros em braile.
