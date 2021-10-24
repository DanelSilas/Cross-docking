# Crossdocking

 O problema de crossdocking é um problema de sequenciamento de caminhões em uma estação de carga e descarga com vagas limitadas 

## O Problema 
![Cd](/imagem/cd.jpg)

Em um centro de crossdockig os caminhões chegam  nas docas de 
entrada com diversos produtos e os mesmos devem ser encaminhados para os 
caminhões de saída . Os caminhões i devem ser direcionados 
para uma doca disponível. Cada caminhão i de entrada possui um conjunto j de 
caminhões de saída que deve atender (Sij > 0). Logo, o caminhão de saída j só 
pode começar a ser carregado quando seus caminhões de entrada i estão totalmente
descarregados. Os caminhões de entrada possuem uma data de chegada r (antes disso
eles não estão disponíveis). O número de docas de entrada (maq1) e de saída (maq2)
é conhecido, bem como o número de caminhões de entrada (nv1) e de saída (nv2). O 
tempo de descarga e carga de cada caminhão é conhecido e definido como p. 
Inicialmente, os gestores de produção devem minimizar a previsão de sequenciamento 
do dia tentando entregar tudo o mais breve. Dado isso, cada produto passa a ter uma
data de entrega limite (d), e uma penalidade por atraso (w) estabelecidas. Dado isso, 
ao longo do dia deve-se verificar a posição prevista de chegada de cada caminhão (r). 
Esta posição é atualizada horahora, casa ocorra algum atraso impactante (violação do 
caminho crítico), o sequenciamento deve ser alterado visando minimizar a data 
prometida ponderando a importância de cada cliente (min WT).

## Considerações

 A formulação para esse problema não é indexado ao tempo e utiliza uma heurística construtiva gulosa para encontrar uma solução rápida para o problema. 


## Uso
 Utilizando o console do AMPL com o comando
```bash
include run.txt
```
## Modelo Matemático
