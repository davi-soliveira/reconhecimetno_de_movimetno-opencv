# Contador de Polichinelos com OpenCV e MediaPipe
![Status do Projeto](https://img.shields.io/badge/Status-Concluído-brightgreen)

## 📖 Descrição do Projeto

Este projeto é um contador de polichinelos que utiliza as bibliotecas **OpenCV** e **MediaPipe** para detectar e contar automaticamente o número de polichinelos realizados em um vídeo. O programa rastreia os pontos do corpo em tempo real e utiliza cálculos de distância para identificar os movimentos característicos do exercício.

---

## ⚙️ Tecnologias Utilizadas

- **OpenCV**: Uma biblioteca de visão computacional que permite a manipulação de imagens e vídeos, além de realizar operações de detecção e reconhecimento.
- **MediaPipe**: Uma biblioteca desenvolvida pelo Google que fornece soluções de aprendizado de máquina para a detecção de pontos-chave do corpo humano, permitindo o rastreamento de movimentos em tempo real.

---

## 📋 Funcionalidades

1. **Carregamento de Vídeo**: O programa carrega um vídeo (`polichinelos.mp4`) para análise.
2. **Rastreamento Corporal**: Utiliza o modelo de pose do MediaPipe para identificar e rastrear pontos-chave do corpo, como mãos e pés.
3. **Cálculo de Distâncias**: Calcula a distância entre as mãos e os pés para identificar se um polichinelo foi realizado.
4. **Contagem de Polichinelos**: Incrementa um contador sempre que um polichinelo é detectado com base nas distâncias calculadas.
5. **Exibição Visual**: Mostra o número de polichinelos realizados em uma caixa azul no canto superior esquerdo do vídeo.

---

## 🛠️ Como Funciona

1. **Inicialização**: O vídeo é carregado e as bibliotecas OpenCV e MediaPipe são inicializadas.
2. **Processamento de Frames**: Em um loop, cada frame do vídeo é processado:
   - O frame é convertido para o formato RGB.
   - Os pontos-chave do corpo são detectados.
   - As distâncias entre as mãos e os pés são calculadas.
3. **Detecção de Polichinelos**: Um polichinelo é detectado quando:
   - As mãos estão a uma distância de 150 pixels ou menos.
   - Os pés estão a uma distância de 150 pixels ou mais.
4. **Contagem e Exibição**: O contador é atualizado e o número de polichinelos é exibido no vídeo.

---

## 📥 Requisitos

Para executar este projeto, você precisará das seguintes bibliotecas:

````bash
pip install opencv-python mediapipe
````
## 📸 Exemplo de Uso

1. **Clone o repositório** e navegue até o diretório do projeto:
   ```bash
   git clone <url-do-repositorio>
   cd <nome-do-diretorio>


---


# Jumping Jack Counter with OpenCV and MediaPipe

## 📖 Project Description

This project is a jumping jack counter that uses the **OpenCV** and **MediaPipe** libraries to automatically detect and count the number of jumping jacks performed in a video. The program tracks body keypoints in real-time and uses distance calculations to identify the characteristic movements of the exercise.

---

## ⚙️ Technologies Used

- **OpenCV**: A computer vision library that allows for image and video manipulation, as well as detection and recognition operations.
- **MediaPipe**: A library developed by Google that provides machine learning solutions for detecting human body keypoints, enabling real-time movement tracking.

---

## 📋 Features

1. **Video Loading**: The program loads a video (`polichinelos.mp4`) for analysis.
2. **Body Tracking**: Uses the MediaPipe pose model to identify and track keypoints of the body, such as hands and feet.
3. **Distance Calculation**: Calculates the distance between hands and feet to identify if a jumping jack has been performed.
4. **Jumping Jack Counting**: Increments a counter whenever a jumping jack is detected based on the calculated distances.
5. **Visual Display**: Shows the number of jumping jacks performed in a blue box in the upper left corner of the video.

---

## 🛠️ How It Works

1. **Initialization**: The video is loaded, and the OpenCV and MediaPipe libraries are initialized.
2. **Frame Processing**: In a loop, each frame of the video is processed:
   - The frame is converted to RGB format.
   - Body keypoints are detected.
   - Distances between hands and feet are calculated.
3. **Jumping Jack Detection**: A jumping jack is detected when:
   - The hands are within 150 pixels or less.
   - The feet are 150 pixels or more apart.
4. **Counting and Display**: The counter is updated, and the number of jumping jacks is displayed on the video.

---

## 📥 Requirements

To run this project, you will need the following libraries:

```bash
pip install opencv-python mediapipe
Clone o repositório e navegue até o diretório do projeto.
Execute o script Python que contém o código do contador de polichinelos.
O vídeo será processado e o número de polichinelos será exibido em tempo real.
```


