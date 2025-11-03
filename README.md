# Implementação do K-Means em C++ (Algoritmos 1)

Este repositório contém o código-fonte de uma implementação do algoritmo de clusterização K-Means, desenvolvido em C++ como trabalho final para a disciplina de Algoritmos 1. O objetivo é agrupar os dados do dataset Iris em um número $k$ de clusters, com base em suas características.

---

## 🇧🇷 Versão em Português

### Visão Geral do Projeto

O código implementa os passos fundamentais do algoritmo K-Means:

* **Leitura de Dados:** Processa o arquivo `iris.txt`, extraindo as 4 dimensões (atributos) de cada ponto.
* **Interatividade:** Solicita ao usuário o número de clusters ($k$) e o número de iterações desejado.
* **Inicialização:** Os $k$ centróides iniciais são escolhidos aleatoriamente a partir dos pontos de dados existentes.
* **Clusterização:** Executa iterativamente dois passos:
    1.  **Atribuição:** Associa cada ponto ao centróide mais próximo, usando a Distância Euclidiana.
    2.  **Atualização:** Recalcula a posição de cada centróide como a média de todos os pontos atribuídos a ele.
* **Resultado:** Exibe a qual cluster cada ponto foi associado e a porcentagem de pontos em cada cluster.

### Como Compilar e Executar

Certifique-se de que o arquivo `iris.txt` está no mesmo diretório que o executável.

1.  **Compile o código (ex: com g++):**
    ```bash
    g++ seu_arquivo.cpp -o kmeans
    ```
    *(Substitua `seu_arquivo.cpp` pelo nome do seu arquivo C++)*

2.  **Execute o programa:**
    ```bash
    ./kmeans
    ```

3.  **Siga as instruções:**
    Insira o número de grupos (clusters) e o número de iterações quando solicitado.

---

## 🇬🇧 English Version

### Project Overview

This code implements the fundamental steps of the K-Means algorithm:

* **Data Parsing:** Processes the `iris.txt` file, extracting the 4 dimensions (features) for each data point.
* **Interactivity:** Prompts the user for the desired number of clusters ($k$) and the number of iterations.
* **Initialization:** The initial $k$ centroids are chosen randomly from the existing data points.
* **Clustering:** Iteratively performs two steps:
    1.  **Assignment:** Assigns each point to the nearest centroid using Euclidean Distance.
    2.  **Update:** Recalculates each centroid's position as the mean of all points assigned to it.
* **Result:** Displays the final cluster assignment for each point and the percentage of points in each cluster.

### How to Compile and Run

Ensure the `iris.txt` file is in the same directory as the executable.

1.  **Compile the code (e.g., with g++):**
    ```bash
    g++ your_file.cpp -o kmeans
    ```
    *(Replace `your_file.cpp` with your C++ file name)*

2.  **Run the program:**
    ```bash
    ./kmeans
    ```

3.  **Follow the prompts:**
    Enter the number of groups (clusters) and the number of iterations when requested.
