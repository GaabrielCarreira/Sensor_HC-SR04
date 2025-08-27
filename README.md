# Sensor_HC-SR04
O HC-SR04 é um sensor ultrassônico muito utilizado em projetos de eletrônica e robótica para medir distâncias de forma simples e precisa. Ele funciona emitindo ondas sonoras de alta frequência (ultrassom) através do pino Trigger e medindo o tempo que essas ondas levam para retornar ao sensor após refletirem em um objeto, através do pino Echo.

A partir desse tempo de resposta, é possível calcular a distância entre o sensor e o obstáculo detectado. Esse recurso é bastante útil em sistemas de automação, robôs desviadores de obstáculos, medidores de nível e diversas outras aplicações práticas.

No passo a passo a seguir, veremos como o HC-SR04 opera, quais são suas conexões e como interpretar os sinais para obter a distância com precisão;

![introducao1](https://github.com/user-attachments/assets/1d2269fe-74a9-4b56-a299-290b4d753b1c)

# Passo 1:
Conecte sua Placa ESP em sua Protoboard, de maneira que sobre uma linha para você conectar os jumpers;

![foto1 1](https://github.com/user-attachments/assets/8a16af97-6b90-434f-803a-8fa4dce433c7)

# Passo 2:
Agora conecte seu sensor HC-SR04 em algum espaço da Protoboard (o sensor deve ficar com os "olhos" para fora da placa, para que não identifique os fios e dê uma distância equivocada), deve sobrar espaço para conectar os jumper na placa, dando ligação com o sensor;

![foto2 2](https://github.com/user-attachments/assets/d01ced89-47a8-4f12-9de5-aaa623b9bbef)

# Passo 3:
Conecte seu Jumper Preto ao GND da placa e ao o GND do sensor, se tiver feito como a gente, será o primeiro pino do sensor da esquerda para a direita;

![foto3 1](https://github.com/user-attachments/assets/0fcbb3d0-6ede-49bf-8788-1df829e4b4f9)

Existe outra maneira de fazer a ligação do GND, se seu interesse for ligar outros sensores ou LED's você pode optar por fazer uma ligação usando a linha negativa da protoboard, dessa forma:

![foto4](https://github.com/user-attachments/assets/42e3ec12-fe98-4601-85bb-ba201ed2a79c)

# Passo 4:
Conecte outro Jumper com uma cor que seja chamativa como Verde, Azul, em um pino digital da placa de sua preferência, escolhemos o pino 13, e ligue diretamente na placa, no pino "ECHO", que como foi dito anteriormente, vai medir o tempo que suas ondas levam para retornar ao sensor após refletirem em um objeto, ou seja, a informação vai entrar;

![foto5](https://github.com/user-attachments/assets/49911ff4-f857-4d4c-99b0-06a11277addf)
![foto5 1](https://github.com/user-attachments/assets/c10a550f-e6dd-4ef7-9ce9-a2cf09aba876)

# Passo 5:
Agora com outro jumper, (uma boa prática, é utilizar uma cor chamativa também, mas diferente da que você usou anteriormente, não cometa o mesmo erros que nós) conecte no pino "TRIGER", que é o responsável por emitir ondas sonoras de alta frequência (ultrassom), e conecte em um pino digital da placa, utilizamos a porta 12, dessa forma:

![foto6](https://github.com/user-attachments/assets/d1e6191e-706f-449f-b79d-e9ab2bf3a211)
![foto6 1](https://github.com/user-attachments/assets/7b5909d7-f4ae-4b2e-bfd0-486da3aeeeaa)

# Passo 6:

Para finalizar as conexões, conecte um cabo vermelho no pino VCC do sensor, e na placa no pino VIN, que representa os 5 volts;

![foto7](https://github.com/user-attachments/assets/d0c5ae36-2d86-4bd0-b95c-d65544d4ef11)
![foto7 1](https://github.com/user-attachments/assets/d6a69bc1-aed9-474b-960b-fb8f2eed5e3e)

# Passo 7:
Conecte o USB à sua placa, e ao seu computador;

![foto9](https://github.com/user-attachments/assets/9761a23c-ed69-44a9-a269-e3b6aaf8f966)

# Passo 8: 
Baixe a biblioteca "EasyUltrassonic" para a facilitar a programação, e escreva o seguinte código (está de uma forma bem simplificada, substitua o que for necessário, como número das portas, etc.":

<img width="466" height="442" alt="codigo" src="https://github.com/user-attachments/assets/e59f5eca-8244-48c6-96d9-77587f7ed02c" />

Se tudo ocorrer bem você obeterá esse resultado, um sensor medindo a distância corretamente:

<img width="324" height="343" alt="resultado" src="https://github.com/user-attachments/assets/aff75c3c-8c35-4d7d-a79d-8af8b128c5bd" />

Espero que tenha entendido e gostado, muito obrigado pela atenção!




