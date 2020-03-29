# utibrasil

Visualização das UTIs e unidades de isolamento por cidade utilizando a biblioteca Folium com informações baseadas no Datasus. Motivação do estudo: pandemia da COVID-19

A base de dados foi obtida no site do Datasus e seguiu este caminho:

https://datasus.saude.gov.br/informacoes-de-saude-tabnet/ rede assistencial / CNES - Recursos físicos / Hospitalar - leitos complementares

CNES é a sigla para Cadastro Nacional de Estabelecimentos de Saúde

O arquivo foi gerado com a linha 'Município', coluna 'leitos complementares', conteúdo 'quantidade existente' e período 'fevereiro de 2020'. Quantidade existente reúne rede pública e particular.

Neste dataset constam as seguintes colunas:

UTI adulto I, UTI adulto II, UTI adulto III, UTI coronariana tipo II -UCO tipo II, UTI coronariana tipo III - UCO tipo III,
UTI de Queimados, UTI neonatal I, UTI neonatal II, UTI neonatal III, UTI pediátrica I, UTI pediátrica II,
UTI pediátrica III, Unidade de cuidados intermed adulto, Unidade de cuidados intermed neonatal canguru, 
Unidade de cuidados intermed neonatal convencional', Unidade de cuidados intermed pediatrico', Unidade intermediária neonatal e
Unidade isolamento.

Para este estudo foram removidas as colunas com UTIs neonatais e mantidas apenas as adultas e pediátricas, além de unidades de isolamento.

O dataset final foi um merge do arquivo do Datasus com outro que possui as coordenadas dos municípios para fazer a visualização no mapa.

Fonte do dataset de coordenadas https://github.com/kelvins/Municipios-Brasileiros

Este estudo aceita sugestões de melhorias, apontamento de correções e demais observações. Meu e-mail é juservi@gmail.com 
