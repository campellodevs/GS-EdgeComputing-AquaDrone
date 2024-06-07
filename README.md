# GS-EdgeComputing-AquaDrone
Grupo: AquaDrone Innovations
Projeto de Monitoramento Ambiental com ESP32

Este projeto utiliza um microcontrolador ESP32 para monitorar a qualidade do ar e as condições ambientais, exibindo os resultados em um display LCD. Ele utiliza um sensor de gás para medir a concentração de partículas por milhão (PPM) no ar, e um sensor de temperatura e umidade para monitorar as condições ambientais.

Requisitos:

- Microcontrolador ESP32
- Sensor de gás (MQ-135 ou similar)
- Sensor de temperatura e umidade (DHT22 ou similar)
- Display LCD I2C 16x2
- Bibliotecas necessárias: Wire.h, LiquidCrystal_I2C.h, DHT.h

Instruções de Uso:

1. Monte o circuito conforme o esquema de conexões.
2. Carregue o código fornecido para o ESP32 utilizando a IDE Arduino.
3. Conecte o ESP32 ao computador via USB para monitorar os resultados no Monitor Serial.

Conexões:

- Conecte o sensor de gás ao pino analógico 4 (PPM_PIN).
- Conecte o sensor de temperatura e umidade ao pino digital 5 (DHT_PIN).
- Conecte o display LCD I2C aos pinos SDA e SCL do ESP32.

Dependências:

- Este projeto depende das bibliotecas Wire.h, LiquidCrystal_I2C.h e DHT.h para o funcionamento correto. Certifique-se de tê-las instaladas na sua IDE Arduino.

Funcionamento:

- Ao ligar o ESP32, ele inicializará os sensores e o display LCD.
- O sensor de gás medirá a concentração de partículas por milhão (PPM) no ar.
- O sensor de temperatura e umidade medirá as condições ambientais.
- Os valores lidos pelos sensores serão exibidos no display LCD, mostrando a concentração de PPM na parte superior e alternando entre temperatura e umidade na parte inferior.
- Os valores também serão enviados para o Monitor Serial para monitoramento adicional.

Observações:

- Certifique-se de calibrar o sensor de gás de acordo com as especificações do fabricante para obter resultados precisos.
- Este projeto pode ser expandido adicionando mais sensores para monitorar outras variáveis ambientais, como luminosidade ou qualidade do ar.
- Ajuste os valores de delay conforme necessário para atender aos requisitos do seu projeto.

Este projeto oferece uma solução simples e eficaz para monitoramento ambiental, permitindo que os usuários acompanhem a qualidade do ar e as condições de temperatura e umidade em tempo real.

Isso é útil para entender melhor o ambiente natural e como as mudanças climáticas podem estar afetando ecossistemas específicos. Por exemplo, variações extremas de temperatura e umidade podem afetar o comportamento e a distribuição de animais e plantas.
Esse tipo de monitoramento ambiental fornece dados valiosos para pesquisadores e cientistas que estudam ecologia, conservação da natureza e mudanças climáticas. Os dados coletados podem ser usados para entender padrões de longo prazo e realizar estudos de monitoramento de longo prazo em áreas naturais.

Autores: Lucca Campello - RM:58455, Victorio Bastelli - RM:554723, Guilherme Moreira - RM:557290;
