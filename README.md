# Projeto#1: Fonte de Tensão

## DESCRIÇÃO:
Projeto de uma Fonte de Tensão entre 3V a 12V com capacidade de 100mA

## Diagrama da Fonte

![Circuito](circuito.png)

### Link para o circuito
http://tinyurl.com/ydc6hb5x

### Explicação dos valores escolhidos:
- Capacitor:
  
  A partir da equação para cálculo da tensão:
  
  ![equation](https://latex.codecogs.com/gif.latex?%5CDelta%20V%20%3D%20%5Cfrac%7B1%7D%7B2.f.C.R%7D) 
  
  Assumindo ![equation](https://latex.codecogs.com/gif.latex?%5CDelta%20V%20%3C%201%25) e sabendo que ![equation](https://latex.codecogs.com/gif.latex?f%20%3D%2060Hz), temos:
  
  ![equation](https://latex.codecogs.com/gif.latex?C%20%3C%20%5Cfrac%7B1%7D%7B12%7D%5Ccdot%2010%5E%7B-4%7D%5Ccong%208.3%5Ccdot%2010%5E%7B5%7D)
  
  Dessa forma, um Capacitor de ![equation](https://latex.codecogs.com/gif.latex?80%5Cmu%20F) é suficiente para a fonte do projeto.

- Circuito Regulador de Tensão:
  
  A partir da datasheet da "Texas Instruments"(https://tinyurl.com/y7voskoq), obtêm-se a fórmula:

  ![equation](https://latex.codecogs.com/gif.latex?V_%7Bs%7D%20%3D%201.25%5Ccdot%20%5Cleft%20%28%201%20&plus;%20%5Cfrac%7BR2%7D%7BR1%7D%20%5Cright%20%29&plus;%5Cleft%20%28%2050%5Ccdot%2010%5E%7B-6%7D%5Ccdot%20R2%20%5Cright%20%29)
	
  Onde:
	- ![equation](https://latex.codecogs.com/gif.latex?V_%7Bs%7D) é a tensão de saída.
	- ![equation](https://latex.codecogs.com/gif.latex?R1) é um resistor.
	- ![equation](https://latex.codecogs.com/gif.latex?R2) é a resistência do potênciometro.
  
  Assim, para obter ![equation](https://latex.codecogs.com/gif.latex?3V) na saída com o potênciometro em seu valor mínimo e ![equation](https://latex.codecogs.com/gif.latex?12V) com o potênciometro em seu valor máximo, os seguintes valores são necessários para satisfazer a equação:
  
  Para ![equation](https://latex.codecogs.com/gif.latex?3V), o potêncimetro deve estar em um valor próximo de ![equation](https://latex.codecogs.com/gif.latex?3V). Logo, ![equation](https://latex.codecogs.com/gif.latex?R1%5Ccong%20714%5COmega).

  E para ![equation](https://latex.codecogs.com/gif.latex?12V), utilizando ![equation](https://latex.codecogs.com/gif.latex?714%5COmega), ![equation](https://latex.codecogs.com/gif.latex?R1%20%5Ccong%206k%5COmega).
	

->E um video mostrando o Projeto funcionando ou simulando e explicando porque escolheu os valores dos componentes (Upa no Youtube e poe um link no teu Github).

### Componentes:
* Diodo (x6) - R$ 0,66
* Transformador 110v para 12v - R$ 35,00
* Capacitor 100μF - R$ 0,10
* Capacitor 10μF (x3) - R$ 0,42
* Potenciômetro 6kΩ - R$ 1,09
* Resistor 1kΩ - R$ 0,08
* Resistor 700Ω (a partir de (1x) 1kΩ + (1x) 100Ω em paralelo com (2x) 220Ω + (1x) 100Ω) - R$ 0,40
* LM 317 - R$ 2,75
**TOTAL: R$ 5,85**

## Participantes:
* **Gabriel da Cunha Dertoni(11795717)** - [GabrielDertoni](https://github.com/GabrielDertoni)

* **Eduardo Henrique Porto Silva(11796656)**  - [EduardoPortoSilva](https://github.com/EduardoPortoSilva)

* **Pedro Henrique Borges Monici(10816732)** - [pedromonici](https://github.com/pedromonici)

* **Tulio Santana Ramos(11795526)** - [Tulip-bcc](https://github.com/Tulip-bcc)




