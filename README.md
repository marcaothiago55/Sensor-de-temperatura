# Programa de Controle de Temperatura e Umidade com Sensor DHT11 e Display OLED com sinais de visuais e auditivos 

Introdução:
Este código é um exemplo de um programa desenvolvido pelo Professor Thiago Antonio Marcão para a aula 29 de Robótica Paraná na Escola Otalipío. O programa utiliza um microcontrolador (possivelmente Arduino) para monitorar a temperatura e umidade do ambiente, exibindo os valores em um display OLED, controlando LEDs e emitindo sons através de um buzzer em resposta às mudanças de temperatura.

Bibliotecas e Constantes Iniciais:
Importação das bibliotecas Adafruit_AM2320, U8glib e DHT para a comunicação com sensores e controle do display.
Definição de constantes para os pinos de botão, sensor DHT, LEDs e buzzer.
Estabelecimento de um intervalo de leitura de 2 segundos.

Função drawLetreiro e draw:
A função drawLetreiro cria um texto em movimento no display OLED.
A função draw desenha elementos estáticos no display, como valores de temperatura e umidade.

Configuração Inicial (setup):
Inicialização da comunicação serial.
Configuração dos pinos como entrada ou saída.
Inicialização do sensor DHT.

Loop Principal (loop):
Execução principal do programa.
Leitura dos sensores de temperatura e umidade a cada 2 segundos.
Controle dos LEDs e do buzzer baseado nas mudanças de temperatura.
Ativação do LED vermelho e do buzzer quando a temperatura atinge 30°C.
Ativação do LED azul e do buzzer quando a temperatura cai para 10°C.
Alternância entre exibir temperatura e umidade no display com base no estado do botão.

Controle dos LEDs e Buzzer:
Funções controlarLeds e controlarBuzzer usadas para controlar LEDs e o buzzer conforme as mudanças de temperatura.

Funções Auxiliares:
piscaLuz: Piscar rápido de um LED para indicar alterações de temperatura.

Resumo:
O código configura um sistema que utiliza um sensor DHT11 para medir temperatura e umidade, mostrando esses valores em um display OLED. Também controla LEDs e emite sons através de um buzzer de acordo com as mudanças de temperatura. Um botão permite alternar entre exibir temperatura e umidade no display. O programa foi desenvolvido para fins educacionais, integrando uma aula de robótica em uma escola.

Materiais Necessários para o Projeto:
Arduino Uno R3 + Cabo USB
Display OLED 128×64 0.96″ I2C – Azul/Amarelo
Módulo Sensor De Umidade e Temperatura DHT11
Led Push Button (Chave Táctil) 6x6x6mm
Resistor 330R 1/4W (1 Unidades)
Resistor 220R 1/4W (2 Unidades)
Jumpers – Macho/Macho – 25 Unidades
Mini Protoboard 170 pontos
LEDs (um azul e um vermelho) (2 Unidades)
Buzzer passivo (1 Unidades)




