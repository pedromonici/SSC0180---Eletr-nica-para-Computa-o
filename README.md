# Projeto#1: Fonte de Tensão

## DESCRIÇÃO:
Projeto de uma Fonte de Tensão entre 3V a 12V com capacidade de 100mA

## Diagrama da Fonte

![Circuito](circuito.png)
**NOTA: A resistência de 30 ohms que pode ser vista no circuito é apenas uma forma de representar a presença do regulador de tensão LM 317. A única função dessa resistência é causar uma queda de tensão similar a do LM 317 que permite a simulação no falstad**
### Link para o circuito
http://tinyurl.com/yc745h6d

### Explicação dos valores escolhidos:
- Capacitor:
  
  A partir da equação para cálculo da tensão:
  
  ![equation](https://latex.codecogs.com/gif.latex?%5CDelta%20V%20%3D%20%5Cfrac%7B1%7D%7B2.f.C.R%7D) 
  
  Assumindo ![equation](https://latex.codecogs.com/gif.latex?%5CDelta%20V%20%3C%5Cfrac%7B1%7D%7B100%7D) e sabendo que ![equation](https://latex.codecogs.com/gif.latex?f%20%3D%2060Hz), temos:
  
  ![equation](https://latex.codecogs.com/gif.latex?C%3E%5Cfrac%7B1%7D%7B132%7D%5CRightarrow%20C%3E7.6%5Ccdot%2010%5E%7B-3%7DF)
  
  Dessa forma, um Capacitor de ![equation](https://latex.codecogs.com/gif.latex?8mF) é suficiente para a fonte do projeto.

- Circuito Regulador de Tensão:
  
  A partir da datasheet da "Texas Instruments"(https://tinyurl.com/y7voskoq), obtêm-se a fórmula:

  ![equation](https://latex.codecogs.com/gif.latex?V_%7Bs%7D%3D1.25%5Ccdot%20%5Cleft%20%28%201&plus;%5Cfrac%7BR2&plus;R2%27%7D%7BR1%7D%20%5Cright%20%29&plus;%20%5Cleft%28%2050%5Ccdot%2010%5E%7B-6%7D%5Ccdot%20%5Cleft%20%28%20R2&plus;R2%27%20%5Cright%20%29%5Cright%20%29)
	
  Onde:
	- ![equation](https://latex.codecogs.com/gif.latex?V_%7Bs%7D) é a tensão de saída.
	- ![equation](https://latex.codecogs.com/gif.latex?R1) é um resistor.
	- ![equation](https://latex.codecogs.com/gif.latex?R2) é o potênciometro.
	- ![equation](https://latex.codecogs.com/gif.latex?R2%27) é a resistência em série do potênciômetro.
  
  Assim, para obter ![equation](https://latex.codecogs.com/gif.latex?3V) na saída com o potênciometro em seu valor mínimo e ![equation](https://latex.codecogs.com/gif.latex?12V) com o potênciometro em seu valor máximo, os seguintes valores são necessários para satisfazer a equação:
  
  Para ![equation](https://latex.codecogs.com/gif.latex?3V), o potêncimetro deve estar em um valor próximo de ![equation](https://latex.codecogs.com/gif.latex?0) e ![equation](https://latex.codecogs.com/gif.latex?R2%27%3D1k%5COmega). Logo, ![equation](https://latex.codecogs.com/gif.latex?R1%5Ccong%20714%5COmega).

  E para ![equation](https://latex.codecogs.com/gif.latex?12V), utilizando ![equation](https://latex.codecogs.com/gif.latex?714%5COmega), ![equation](https://latex.codecogs.com/gif.latex?R2%5Ccong%205k%5COmega).
	
### Video da simulação do projeto
https://youtu.be/dQlkS4CVClo

### Componentes:
* Diodo (x6) - R$ 0,66
* Transformador 110v para 24v - R$ 29,90
* Capacitor 100μF - R$ 0,10
* Capacitor 10μF (x3) - R$ 0,42
* Capacitor de 8mF (1mF x 8) - R$ 3,84
* Potenciômetro 5kΩ - R$ 1,09
* Resistor 110Ω - R$ 0,12
* Resistor 1kΩ - R$ 0,08
* LM 317 - R$ 2,75
* Fusível - R$ 0,42
* **TOTAL: R$ 39,38**

## Esquemático do circuito no EAGLE

![Circuito](esquematico.png)

## PCB do circuito no EAGLE

![Circuito](pcb.png)

## Participantes:
* **Gabriel da Cunha Dertoni(11795717)** - [GabrielDertoni](https://github.com/GabrielDertoni)

* **Eduardo Henrique Porto Silva(11796656)**  - [EduardoPortoSilva](https://github.com/EduardoPortoSilva)

* **Pedro Henrique Borges Monici(10816732)** - [pedromonici](https://github.com/pedromonici)

* **Tulio Santana Ramos(11795526)** - [Tulip-bcc](https://github.com/Tulip-bcc)




