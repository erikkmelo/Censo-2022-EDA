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

## CONSIDERAÇÕES FINAIS

# ANÁLISE EXPLORATÓRIA DOS DADOS DO CENSO 2022 (IBGE) RESULTADO DO UNIVERSO POR SETORES
