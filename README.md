# Sensor-de-temperatura

Bibliotecas Importadas:

Adafruit_AM2320.h: Biblioteca para comunicação com o sensor de temperatura e umidade AM2320.
U8glib.h: Biblioteca para controle do display OLED SSD1306.
DHT.h: Biblioteca para interação com sensores de temperatura e umidade da família DHT.
Definições de Pinos e Constantes:

pino_muda: Pino conectado ao botão que alterna entre exibir temperatura e umidade.
pino_DHT: Pino ao qual o sensor DHT11 está conectado.
DHTTYPE: Tipo do sensor DHT (DHT11 neste caso).
ledAzulPin: Pino para controlar o LED azul.
ledVermelhoPin: Pino para controlar o LED vermelho.
buzzerPin: Pino para controlar o buzzer passivo.
Variáveis Globais:

temperatura: Armazena o valor da temperatura lido pelo sensor.
umidade: Armazena o valor da umidade lido pelo sensor.
guarda_estado: Controla se a tela exibe a temperatura ou umidade.
estado: Armazena o estado atual do botão.
previousMillis: Armazena o valor do tempo anterior para controlar a leitura periódica dos sensores.
interval: Intervalo de tempo entre as leituras dos sensores.
letreiroDelay: Atraso para a animação do letreiro.
letreiroStep: Quantidade de pixels que o letreiro se move a cada iteração.
letreiroPosition: Posição atual do letreiro no display.
temperaturaSubiu: Variável de controle para determinar se a temperatura subiu.
Funções:

drawLetreiro(text): Desenha o letreiro no display OLED com o texto especificado.
controlarLeds(temperatura): Controla os LEDs vermelho e azul com base na temperatura.
controlarBuzzer(novaTemperatura, temperaturaAnterior): Emite diferentes sons pelo buzzer quando a temperatura sobe ou desce.
piscaLuz(pinoLed): Faz a luz associada ao pino piscar por um curto período de tempo.
draw(): Função principal para desenhar os elementos no display OLED com base no estado atual.
Configuração Inicial (setup()):

Inicialização das portas dos pinos.
Inicialização dos sensores DHT.
Configuração do baud rate da comunicação serial.
Loop Principal (loop()):

Verifica se é necessário alternar entre a exibição de temperatura e umidade.
Realiza a leitura periódica dos sensores de temperatura e umidade.
Controla os LEDs e o buzzer de acordo com as condições estabelecidas.
Faz a animação do letreiro.
Atualiza o display OLED com base nas informações de temperatura e umidade.
O projeto utiliza o sensor DHT11 para medir a temperatura e a umidade do ambiente. O display OLED exibe a temperatura ou umidade, dependendo do estado do botão. Os LEDs e o buzzer são controlados para indicar a mudança na temperatura, com diferentes sons e piscadas de luz para diferentes situações. A animação do letreiro no topo do display acrescenta um toque visual ao projeto.

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
