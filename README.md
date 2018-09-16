# Estação Meteorológica - Sistemas Embarcados

## Como usar o git: Em Construção
[Link](how-to-git.md)

## Pendente
- Como carregar a bateria com placa fotovoltáica?
- Formato do Documento de Descrição Funcional
- De quanto em quanto tempo trocar bateria 
1. definição de consumo

## Escopo
- Produto deve ser o mais próxima da produção
- Sistema de análise meteorológica
- Medir temperatura
- Medir luminosidade
- Medir umidade
- Medir pressão atmosférica
- Medir horas de radiação por dia
- Funcionará com bateria
- Terá sistema de carregamento a partir de placa fotovoltáica
- Interface do usuário 
	- Exibir valores de medição das últimas 24 horas
	- 4 Medições por hora -> gera média
	- Utilizará bluetooth para comunicar com o sistema e o celular

## Requisitos funcionais
- Sistema deve ter aplicativo
- Sistema deve exibir valores de medição
- Sistema deve fazer média de leituras em cada hora
- Registrar tempo de luminosidade
- Deve ter sinalização em função da altura

## Requisitos não funcionais
- Sistema deve ter bateria
- Sistema deve operar em baixo consumo
- Sistema terá acionamento para o bluetooth - diminuir consumo
- Sistema deve ter gráfico com 24 pontos
- Será um aplicativo android

## Interface usuário
- Como conectar bluetooth com celular
- Como criar app que use bluetooth

## Particionamento Hardware-Software
### Hardware
- M4 (ARM) 
- LDR (analog) 
- DHT11 (serial) [Documentação Protocolo](http://www.ocfreaks.com/basics-interfacing-dht11-dht22-humidity-temperature-sensor-mcu/)
- Bluetooth HC05 (serial)
- Bmp180 (i2c) [Documentação Protolo](https://learn.sparkfun.com/tutorials/bmp180-barometric-pressure-sensor-hookup-)
- Bateria 9V (com regulador)
- Bateria de BACKUP

### Software
- Android
- Material Design
- Atollic
- STM32CubeMX

## Requisitos
- Estudo dos objetivos e funcionalidade do sistema a ser desenvolvido
- Levantamento dos requisitos funcionais e não funcionais - Revisar
- Estudo do particionamento HW/SW - 
- Estudo da metodologia de projeto que será empregada para desenvolver o sistema embarcado

## Metodologia de Projeto
- 

## Comentários

### Caso escolhido
Caso 1: Estação meteorológica  que deverá fornecer os  dados de:

- temperatura - LM35 (DHT11)
- umidade relativa - DHT11
- radiação solar - LDR 
- pressão atmosférica - Sensor Pressão Atmosférica Barômetro Bmp180 Arduino / Pic 
- horas de radiação solar por dia

A estação deverá funcionar continuamente, sua instalação não ficará próxima a alguma fonte de alimentação. 
- Bateria + Placa Solar

Deverá ser possível acessar as últimas  N medições de alguma forma  fácil e amigável ao usuário leigo.
- Módulo bluetooth para conectar

Qual a melhor forma de amostrar? 
- Ler sobre estações meteorológicas e frequência de medição
