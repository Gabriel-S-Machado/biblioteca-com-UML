# Requisitos

## Funcionais

1. Criar **Livros**
1. Livros de **Estudos** devem ter o Nível de Graduação (brasileiro) neles
1. Livros de **Filosofia** devem ter o Eixo Filosofico deles, sendo eles:
    * Sofismo
    * Estoisismo
    * Nilismo
1. Trazer informações de Nome, Generos (estudos, terror, romance, filosofia...), **Autor** e **Editora** nos livros
1. Caso **Editora** seja o próprio **Autor**, ele não precisa ser relacionado com **Autor**, essa informação é irrelevante
1. Criar **Estantes** para organizar os livros
1. Poder organizar as estantes por:
    * Nome autor
    * Nascimento Autor
    * Morte autor
    * Editora
    * Nome livro
    * Edição livro
1. Poder classificar as estantes por:
    * Ordem crescente (a-z)
    * Ordem de-crescente (z-a)
1. Criar **Imoveis** para colocar as estantes:
    * Livraria
    * Casa
    * Prédio
1. Criar **Comodos** para representar os imoveis internamente:
    * Livraria
    * Banheiro
    * Recepção
    * Elevador
    * Escadas
1. Poder colocar as estantes nas livrarias
1. Gerar mapa do comodo da livraria
1. Ter nome nas estantes, para melhor identificação
1. Gerar mapa do imovel
1. Ter nomes para os diferentes comodos, para melhor identificação
1. Criar **Ruas** para identificar o local dos imoveis
1. Criar **Bairros** para identificar o local das ruas
1. Criar **Cidades** para identificar o local dos bairros
1. Gerar mapa da rua, bairro e cidade
1. Ter nomes para os diferentes imoveis, para melhor identificação
1. Imoveis tem que ter um **Endereço** funcional (ficticio)
1. Poder atualizar o endereço dos imoveis
1. Poder atualizar os nomes dos:
    * Comodos
    * Imoveis
    * Ruas
    * Bairros
    * Livros
    * Autores
    * Editoras
    * Estantes
1. Poder salvar o que for criado
1. Poder carregar o que foi salvo
1. Responder a programas externos (API)
1. Poder gerar os mapas em:
    * Planilha (xlsx)
    * Texto (txt)
1. Permitir localizar itens especificos de:
    * Cidades
    * Bairros
    * Ruas
    * Imoveis
    * Comodos
    * Livrarias
    * Estantes
    * Livros
1. Permitir localizar livros pelo nome popular do autor (apelido)

## Não funcionais

1. Salvar os dados localmente, em arquivo
1. Após salvar primeira vez, as consecutivas usarão as mesmas opções de antes (a menos que solicitado contrario)
1. Caso haja mais de um item correspondente em uma procura, listar opções
1. Interface gráfica para produto final (para prévisualização dos mapas)
1. JSON para comunicação API
1. Persistência em:
    * JSON (aproveita p/ API e persistência)
    * Texto tabulado (csv)
1. Para clarificar: **Editora** pode ser uma pessoa física não-editora (**EditoraPJ**), pessoa juridica com um local relevante no mapa do usuário (**EditoraPF**) ou só algo irrelevante para o contexto do usuário (**Editora** generica).

## Inversos

1. Não será suportado **Livros** e **Estantes** duplicados. Motivos de simplificação
1. Não será usada persistência online