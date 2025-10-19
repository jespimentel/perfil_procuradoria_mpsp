## Análise de dados extraídos de tabela única contida em arquivo PDF com 4 páginas, com uso da biblioteca Tabula Py.

1) O desafio técnico do projeto consiste em extrair as informações de um documento que é, normalmente, publicado em PDF (a Lista de Antiguidade dos Procuradores de Justiça do Ministério Público do Estado de São Paulo) e tratar os dados obtidos com o Pandas.
2) Optou-se pelo uso da biblioteca "Tabula Py" (no lugar de "Camelot Py" e "Excalibur Py", supostamente mais eficientes na leitura de tabelas em PDF) em razão da facilidade da instalação. O programa rodou no Google Colab.
3) O "Tabula Py" criou tabelas individuais de cada página do PDF, que foram, em seguida, concatenadas para a geração de dataframe único.
4) O resultado da extração da página 4 (última do PDF) não observou o padrão das demais páginas.
5) O script grava, ao final, uma planilha Excel com os dados extraídos e tratados.

## Atualização de 06/02/2022:

6) Para as listas de antiguidade disponibilizadas em 24/11/2021, a extração dos dados dos PDF foi feita com o emprego da biblioteca PyMuPDF. 
7) Essa nova abordagem permitiu a análise conjunta das 5 listas (Procuradores, Final, Intermediária, Inicial e Substitutos) sem a necessidade de editar manualmente os dados obtidos das últimas páginas dos documentos. 
8) O resultado pode ser conferido no notebook "antiguidade_2022.ipynb".

## Atualização de 19/10/2025

9) Usamos o camolot-py para a extração das tabelas e o método df da mesma biblioteca para a geração dos dataframes.
10) Usamos LLM ('gpt-4o-mini') para identificar os gêneros dos membros nominados.
