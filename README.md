# ANÁLISE PRELIMINAR AUTOMATIZADA DO CENSO 2022
## OBJETIVOS:
1. Extrair os dados censitários em novas tabelas para o município selecionado. (CONCLUÍDO) 
2. Aplicar EDA nos dados para o município e achar possíveis clusters. (EM ANDAMENTO)
3. Agregar essas informações na camada de setores (gpkh), sendo uma camada para cada tema.

## FONTE DOS DADOS
Repositório para estudar os dados do IBGE através de Ciência de Dados.
Resultados disponíveis pelo IBGE:
https://www.ibge.gov.br/estatisticas/sociais/trabalho/22827-censo-demografico-2022.html?edicao=41852&t=resultados

Agregados_por_setores_alfabetizacao_BR.zip  
Agregados_por_setores_basico_BR.zip  
Agregados_por_setores_caracteristicas_domicilio1_BR.zip  
Agregados_por_setores_caracteristicas_domicilio2_BR.zip  
Agregados_por_setores_caracteristicas_domicilio3_BR.zip  
Agregados_por_setores_cor_ou_raca_BR.zip  
Agregados_por_setores_demografia_BR.zip  
Agregados_por_setores_domicilios_indigenas_BR.zip  
Agregados_por_setores_domicilios_quilombolas_BR.zip  
Agregados_por_setores_obitos_BR.zip  
Agregados_por_setores_parentesco_BR.zip  
Agregados_por_setores_pessoas_indigenas_BR.zip  
Agregados_por_setores_pessoas_quilombolas_BR.zip  

# EXTRAÇÃO DOS DADOS MUNICIPAIS AGREGADOS POR SETORES
## INTRODUÇÃO
Foi criado um script que acessa esses arquivos listados que foram salvos em um google drive. Como o colab conversa bem com o drive, mesmo o maior arquivo (~1,5GB) demorou cerca de 8 seg para ser baixado no ambiente colab. 

## RESULTADOS:
Para São Vicente - SP, que possui 672 setores, o arquivo final em formato zip que contém os 13 arquivos filtrados para o município teve 565kb, ou seja, ao invés de baixar 6,5GB do IBGE foi só rodar o código e levou cerca de 3 minutos o processo inteiro e gerou um arquivo bem pequeno pra ser trabalhado.  

Obrigado! Quem quiser entrar em contato, pode enviar um e-mail para: [erikmeloengenheiroambiental@gmail.com](mailto:erikmeloengenheiroambiental@gmail.com).  

## PASSO A PASSO
1. No arquivo extrair_csv_mun_censo_2022.ipynb tem um código pronto no ambiente Colab.
2. Basicamente só precisa colocar o código do município e executar tudo, que ao final será gerado automaticamente um arquivo zip, com as 13 planilhas csv só com os dados do município escolhido.
3. Caso o Colab esteja instável, é só executar o código em etapas.
4. Caso queira fazer a filtragem de uma planilha específica, é só executar o código até "Execução dos arquivos" e depois executar apenas o código da planilha escolhida. E depois executar o último código para zipar o arquivo, ou então, baixar direto o arquivo gerado clicando nos três pontinhos ao lado do arquivo.

## CONSIDERAÇÕES FINAIS
1. A vantagem de executar o código é economizar no espaço utilizado no computador e no drive também, já que a versão free de armazenamento é de apenas 15gb, ou seja, quase metade do drive seria utilizado por esses arquivos.
2. É possível criar um banco de dados, e ou um API no lugar do drive (planilhas)? sim é possível. Como faz? não sei ainda. É vantajoso? não sei ainda.
3. É possível filtrar direto no QGIS, sim é possível, porém, o QGIS armazena em cache os dados quando as planilhas são colocadas no projeto, ou seja, se tiver um computador menos robusto, pode ter travamento. Aqui na prefeitura que trabalho ficou travando várias vezes. Por isso veio essa necessidade de trabalhar os dados em nuvem.
4. Caso tenha alguma sugestão de melhoria, entre em contato ou faça o comentário aqui pelo Github.

# ANÁLISE EXPLORATÓRIA DOS DADOS DO CENSO 2022 (IBGE) RESULTADO DO UNIVERSO POR SETORES
## INTRODUÇÃO
Optou-se num primeiro momento de fazer a Análise Exploratória de cadas arquivo separado. E num momento futuro fazer análises mais complexas de dados de várias planilhas juntas.

## RESULTADOS:
1. A primeira tabela análisada foi a Agregados_por_setores_basico_BR.zip, que tem os dados de quantidades de habitantes e domicílios - Código está no arquivo colab EDA_Censo_2022_BASICO.ipynb
2. Observou-se as características dos setores, em relação a quantidade e distribuição da população.
3. Observou-se uma tendencia de taxa de ocupação média dos domicílios, e percebeu-se setores ocupados quase na totalidade, e outros mais vazios.

## PASSO A PASSO

## CONSIDERAÇÕES FINAIS

