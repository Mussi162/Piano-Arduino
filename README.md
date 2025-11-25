# Piano-Arduino
Um projeto que implementa um piano eletronico com 7 teclas com as seguintes notas (Dó, Ré, Mi, Fá, Sol, Lá Si)

🔗Link do Projeto: https://www.tinkercad.com/things/0wS3MYCJzsX-piano


Descrição do Projeto
Cada botão do nosso piano corresponde as notas musicais específica para melodias simples. 
O sistema tem feedback serial para monitoramento das notas que são reproduzidas.
---

<img width="539" height="421" alt="image" src="https://github.com/user-attachments/assets/8afcc43a-8574-4b11-95b0-f96254381119" />

---

🛠 Ferramentário utilizado:

* 1x Arduino Uno ou similar
* 1x Alto-falante ou buzzer (8Ω)
* 7x Botões push-button
* 7x Resistores de 10kΩ (pull-down)
* 1x Resistor de 220Ω (para o buzzer)
* Protoboard e fios jumper

---

Lógica do Sistema:

O sistema faz a leitura contínua das entradas, monitorando o estado dos sete botões.
A detectação dos botões é feita por maio de uma estrutura sequencial garantindo que somente a primeira tecla pressionada seja processada.
Quando o botão é precionado, o som é emitido pela função tone(), que emite a frequência correspondente a nota pressionada.
Caso nenhuma nota seja pressionada, a função noTone() interrompe qualquer som ativo garantindo o silêncio até o próximo botão precionado.
