Criação de Pipeline de Extração, Limpeza, Transformação e Enriquecimento de Dados em linguagem Python:
------------------------------------------------------------------------------------------------------

1 - Extrair os dados da origem (arquivo .CSV) Esse arquivo contem dados fictícios de produção de alimentos.
2 - Aplicar limpeza, transformação e enriquecimento
3 - Carregar os dados no destino (um banco de dados relacional SQLite).
    fazer download do banco de dados nesse link: https://sqlitebrowser.org/dl/	
    Abrir SQLite no Windows: tecla windows + digita DB


* Passos a seguir:

1 - Carga de dados:

	Executar arquivo connect.py somente testar conectividade. Isso vai carregar os dados brutos direto no destino, no banco de dados.


2 - Limpeza dos dados:

        Regra de negócio: Carregar somente registros com quantidade produzida superior a 10.
        Script limpeza.py carregar no banco de dados somente os dados quando a quantidade produzida for superior a 10.


3 - Trasnformação de Dados:

        Regra de negócio: Remover o caracter "ponto" na última coluna do arquivo para evitar que o número seja truncado. 
        Script transformação.py


4 - Enriquecimento dos Dados:

	Regra de negócio: Enriquecer os dados adicionando no destino uma coluna com a margem de lucro de cada produto.
	Script enriquecimento.py


5 Formatação dos Dados:

	Script formatacao.py
