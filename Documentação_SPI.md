# Comunicação SPI (Serial Peripheral Interface)
## Definição

 
 
    É um protocolo de dados seriais síncronos usado por microcontroladores para comunicar-se com um ou mais dispositivos SPIs em curtas distâncias.
 Tipo de comunicação serial síncrona que faz uso do conceito mestre-escravo (master-slave).

 O gerador dos sinal de sincronismo é definido como mestre e os dispositivos que utilizam o sinal de sincronismo gerado são definidos como escravos. 


![alt text](https://github.com/23032000/Avionica---Minerva-Rockets/blob/main/master_slave.png?raw=true)

Trabalha em regime de comunicação full-duplex, toda troca de dados acontece sempre em ambas as direções. Ou seja, cada bit trocado entre do Master para um Slave traz um bit do Slave para  o Master. 


## Pinos básicos de comunicação entre dispositivos SPI


|Pino                   |   Nome Padrão      |   Significado             |
| --------------------- |--------------------| ------------------------- |
| Do Master para o Slave| MOSI               | Master Output Slave Input |
| Do Slave para o Master| MISO               | Master Input Slave Output |
| Clock                 | SCLK               | Serial Clock              |
| Seleção de Slaves     | SS                 | Slave Select              |

## Esquema Padrão de Ligação 
O sinal de SS funciona como seleção de escravo. É um sinal ativo em nível baixo, o que significa que o dispositivo é selecionado quando este pino se encontra em nível baixo.

**OBS:** O pino SS (Slave Select) pode ser ligado a qualquer pino digital do Arduino.

![alt text](https://github.com/23032000/Avionica---Minerva-Rockets/blob/main/esquema_padr%C3%A3o.png?raw=true)

## Exemplo de Comunicação SPI com Micro SD Card
![alt text](https://github.com/23032000/Avionica---Minerva-Rockets/blob/main/sdcard-diagrama-1.jpg?raw=true)


| Pino Módulo | SD Pino Arduino      |
| ----------- | -------------------- |
| SS          | 4 ( Jumper Amarelo)  |
| SCK         | 13 ( Jumper Marrom)  |
| MOSI        | 11 ( Jumper Verde)   |
| MISO        | 12 ( Jumper Laranja) |
| VCC         | 5V (Jumper Vermelho) |
| GND         | GND (Jumper Preto)   |


