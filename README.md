# Sensor-de-temperatura

Este código é um programa para um sensor de temperatura e umidade. Ele foi escrito pelo Professor Thiago Antonio Marcão para a aula 29 de Robótica Paraná na Escola Otalipío. O programa usa as bibliotecas Adafruit_AM2320, U8glib e DHT para ler os valores de temperatura e umidade do sensor DHT11 conectado ao pino A0. Ele também usa a biblioteca U8GLIB_SSD1306_128X64 para exibir esses valores em uma tela OLED.

Esse código é um exemplo de um programa que utiliza um microcontrolador (possivelmente Arduino) para controlar um sistema que mede a temperatura e umidade do ambiente, exibe esses valores em um display OLED, controla LEDs e emite sons usando um buzzer de acordo com as mudanças na temperatura medida. Vou explicar as principais partes do código:

Bibliotecas e Constantes Iniciais:

O código inclui as bibliotecas necessárias para a comunicação com os sensores e o controle do display.
Também define constantes para os pinos usados pelo botão, sensor DHT, LEDs, e o buzzer.
Define um intervalo de leitura para os sensores de 2 segundos.
Função drawLetreiro e draw:

A função drawLetreiro desenha um texto em movimento no display OLED.
A função draw é responsável por desenhar os elementos estáticos no display, como os valores de temperatura e umidade.
Configuração Inicial (setup):

Inicializa a comunicação serial.
Configura os pinos como entrada ou saída.
Inicializa o sensor DHT.
Loop Principal (loop):

O loop principal executa a maior parte das operações.
A cada intervalo definido (2 segundos), os sensores de temperatura e umidade são lidos.
Os LEDs e o buzzer são controlados de acordo com as mudanças de temperatura.
Quando a temperatura atinge 30°C, o LED vermelho é ligado e o buzzer emite um som por 30 segundos.
Quando a temperatura cai para 10°C, o LED azul é ligado e o buzzer emite um som por 30 segundos.
O estado do botão é lido e o modo de exibição no display é alternado entre temperatura e umidade.
Controle dos LEDs e Buzzer:

As funções controlarLeds e controlarBuzzer são usadas para controlar os LEDs e o buzzer com base nas mudanças de temperatura.
Funções Auxiliares:

piscaLuz: Pisca rapidamente um LED para indicar mudanças de temperatura.
Resumo:
Esse código configura um sistema que lê a temperatura e umidade do ambiente usando um sensor DHT11, exibe esses valores em um display OLED, controla LEDs e emite sons através de um buzzer de acordo com as mudanças na temperatura. Também possui um botão que alterna entre exibir a temperatura e a umidade no display. Além disso, possui feedback visual e sonoro para mudanças específicas de temperatura. O programa foi desenvolvido para fins educacionais, como parte de uma aula de robótica em uma escola.

Materiais Necessários para o Projeto com Sensor DHT11 com Display OLED
Uno R3 + Cabo Usb para Arduino
Display OLED 128×64 0.96″ I2C – Azul/Amarelo
Módulo Sensor De Umidade e Temperatura DHT11 – sem Led
Push Button (Chave Táctil) 6x6x6mm
Resistor 330R 1/4W (10 Unidades)
Jumpers – Macho/Macho – 65 Unidades
Mini Protoboard 170 pontos
2 resistores 220R
Dois leds sendo um azul e um vermelho
Um buzzer passivo 
