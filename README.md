#  Sensor de Proximidade com ESP32 e HC-SR04

##  Descrição

Este projeto utiliza o sensor ultrassônico HC-SR04 conectado a um ESP32 para medir a distância entre o sensor e um objeto. O sistema funciona enviando ondas ultrassônicas e calculando o tempo que o sinal leva para retornar após atingir um obstáculo.

Com base nessa medição, o ESP32 pode identificar quando um objeto está próximo e acionar um LED como indicador visual de proximidade.

---

##  Componentes Utilizados

- 1x ESP32  
- 1x Sensor ultrassônico HC-SR04  
- 1x LED  
- 1x Resistor  
- 1x Protoboard  
- Jumpers (cabos de conexão)

---

##  Funcionamento

O sensor HC-SR04 mede distâncias utilizando ondas ultrassônicas. O ESP32 envia um pulso elétrico para o pino **TRIG** do sensor, que emite uma onda ultrassônica. Quando essa onda encontra um objeto, ela é refletida de volta ao sensor.

O pino **ECHO** retorna ao ESP32 o tempo que o sinal levou para ir até o objeto e voltar. A partir desse tempo, o microcontrolador calcula a distância até o objeto.

Se a distância medida estiver abaixo de um valor definido no programa, o ESP32 aciona o LED, indicando que há um objeto próximo ao sensor.

---

##  Autor

Luana M. Lopes Bomfim
