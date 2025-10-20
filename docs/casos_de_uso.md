Ator: Usuário

Objetivo: Login ( matrícula e senha ) 

Relacionamento : Include --- senha 
                 Include --- matrícula

Ator: Aluno


Objetivo: Pesquisar o acervo de livros ( fisicos e onlines )
          Empréstimos de livro
          Receber notificações lembrando da devolução
          Realizar a devolução dos livros


Relacionamento: Include --- Empréstimos de livro ( Aprovar o emprestimo de livros ( bibliotecario ))
                Include --- Receber notificações lembrando da devolução (Enviar mensagens de lembrete, advertencias e punições ( bibliotecario ))


Ator: Bibliotecario 


Objetivo: Saber de todos os livros do acervo
          Aprovar o empréstimos de livros
          Enviar mensagens de lembrete, advertência e punições
          Registrar o estado do livro 


Relacionamento: Include --- Registrar o estado do livro ( avaliar o estado do livro devolvido )

Ator: Professor


Objetivo: Sugerir e adicionar, livros , audiobooks e podcasts
          Utilizar livros durante a aula


Relacionamentos : Extend --- Sugerir e adicionar, livros , audiobooks e podcasts ( Saber de todos os livros do acervo ( bibliotecario))
                  Include --- Utilizar livros durante a aula ( Aprovar o empréstimos de livros (bibliotecario))

