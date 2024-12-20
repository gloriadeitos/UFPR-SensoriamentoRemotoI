# UFPR-SensoriamentoRemotoI <br> Engenharia Cartográfica e de Agrimensura
#### Aluna: Glória Maria Deitos Gomes da Silva - Segundo semestre 2024

---
**11 de Outubro de 2024**<br>
**Exercicio No. 04 : Assinatura espectral**<br>
link: https://docs.ufpr.br/~centeno/m_sr1/exercicios/exe04/index.html <br>

---
<h4>PARTE 1:</h4>

<p align="justify">Um conjunto de sete curvas espectrais foram representadas e armazenadas como arquivos gráficos. Porém a pessoa encarregada de gerar estas figuras esqueceu de associar o nome do arquivo ao alvo correspondente a cada curva.
Visualize as curvas espectrais escolhidas. Existem sete curvas espectrais, ou seja, a representação gráfica da relação reflectância vs. comprimento de onda de sete objetos diferentes. Analise estas curvas e determine a que objeto cada uma delas pertence.
Ao visualizar cada curva analise sua variação e tente determinar a qual objeto ela pertence. Preencha a tabela abaixo, com base nas suas conclusões. Note que algumas curvas podem pertencer ao mesmo objeto e alguns objetos listados não foram incluídos no conjunto de curvas.</p>

<h5>MODELO:</h5>
<table>
    <tr>
        <th>Objeto</th>
        <th>Comprimento de Onda (µm) - eixo X</th>
        <th>Refletância - eixo Y</th>
    </tr>
    <tr style="background-color: #ADD8E6;"> <!-- Água pura -->
        <td>Água pura</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #B0E0E6;"> <!-- Água turva -->
        <td>Água turva</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #98FB98;"> <!-- Água com matéria orgânica -->
        <td>Água com matéria orgânica</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #D2B48C;"> <!-- Solo seco -->
        <td>Solo seco</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #8FBC8F;"> <!-- Solo úmido -->
        <td>Solo úmido</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #FFD700;"> <!-- Solo com baixo teor de argila -->
        <td>Solo com baixo teor de argila</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #98FB98;"> <!-- Vegetação sadia -->
        <td>Vegetação sadia</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #ADFF2F;"> <!-- Vegetação com baixo teor de clorofila -->
        <td>Vegetação com baixo teor de clorofila</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: #7FFF00;"> <!-- Vegetação com baixo teor de umidade -->
        <td>Vegetação com baixo teor de umidade</td>
        <td></td>
        <td></td>
    </tr>
</table>

<h4>CURVAS A SEREM ANALISADAS:</h4>

![01](https://github.com/user-attachments/assets/ec902918-ec88-4ea1-a061-16ee35dc447b)
![02](https://github.com/user-attachments/assets/41c0642f-e1bb-43eb-b1f8-9372f7c35d77)
![03](https://github.com/user-attachments/assets/b266169c-5909-4f25-b059-c684094ef91d)
![04](https://github.com/user-attachments/assets/d023579c-40d0-463a-98ce-e9cf3652b73f)
![05](https://github.com/user-attachments/assets/4cd65ad9-56bb-41b8-98e4-5e17979c6af9)
![06](https://github.com/user-attachments/assets/064dfed3-ed36-4d6e-bc3b-3fc3e7710f86)
![07](https://github.com/user-attachments/assets/9126c5fb-9071-48c5-87f9-41112ba2a638)


<h4>RESPOSTA CORRETA:</h4>

![resposta-correta](https://github.com/user-attachments/assets/f0dc7a60-aeae-4cad-b643-c47de15360f7)

---
<h4>PARTE 2:</h4>
<p align="justify">Os valores digitais de diferentes coberturas da superfície terrestre foram lidos em um recorte de uma imagem digital Landsat, com 7 bandas espectrais. As bandas são:

<b>Banda 1 :</b> azul <br>
<b>Banda 2:</b> verde <br>
<b>Banda 3:</b> vermelho <br>
<b>Banda 4:</b> infra-vermelho próximo <br>
<b>Banda 5:</b> Infra-vermelho médio <br></p>

<p align="justify">
Regiões ocupadas por água, vegetação, solo exposto e areia foram selecionadas. A média dos valores digitais para cada região foi calculada e é mostrada na tabela abaixo. Os valores variam entre 0 e 255 (máximo). Com base na tabela dos valores digitais lidos identifique o tipo de cobertura mais provável para cada região lida. 
</p>



### Tabela 1: Matriz de Confusão - Random Forest (RF)

| Classe                | Floresta | Restinga | Manguezal | Transição | Áreas Urbanas | Agricultura/Pecuária | Água | Restante (Outras) | Total |
|-----------------------|----------|----------|-----------|-----------|---------------|----------------------|------|-------------------|-------|
| **Floresta**           | 0        | 56322    | 26        | 0         | 0             | 0                    | 376  | 0                 | 56324 |
| **Restinga**           | 0        | 8        | 954       | 0         | 0             | 0                    | 0    | 0                 | 962   |
| **Manguezal**          | 0        | 0        | 78        | 0         | 1             | 0                    | 0    | 0                 | 79    |
| **Transição**          | 0        | 0        | 2         | 3475      | 0             | 0                    | 0    | 0                 | 3477  |
| **Áreas Urbanas**      | 0        | 0        | 0         | 12        | 254           | 0                    | 0    | 0                 | 266   |
| **Agricultura/Pecuária** | 0        | 0        | 0         | 0         | 0             | 6873                 | 0    | 0                 | 6873  |
| **Água**               | 0        | 1467     | 7         | 0         | 1             | 0                    | 6873 | 0                 | 7348  |
| **Restante (Outras)**  | 0        | 0        | 0         | 0         | 13            | 0                    | 29   | 0                 | 42    |
| **Total**              | 0        | 56322    | 78        | 3475      | 254           | 6873                 | 0    | 8508              | 8508  |

---

### Tabela 2: Matriz de Confusão - Distância de Mahalanobis (MDist)

| Classe                | Floresta | Restinga | Manguezal | Transição | Áreas Urbanas | Agricultura/Pecuária | Água | Restante (Outras) | Total |
|-----------------------|----------|----------|-----------|-----------|---------------|----------------------|------|-------------------|-------|
| **Floresta**           | 0        | 45977    | 3796      | 0         | 58            | 0                    | 6893 | 0                 | 45977 |
| **Restinga**           | 0        | 2        | 952       | 1         | 7             | 0                    | 0    | 0                 | 962   |
| **Manguezal**          | 0        | 0        | 57        | 24        | 0             | 0                    | 0    | 0                 | 81    |
| **Transição**          | 0        | 0        | 0         | 3363      | 0             | 0                    | 112  | 0                 | 3475  |
| **Áreas Urbanas**      | 0        | 0        | 0         | 56        | 195           | 0                    | 0    | 49                | 300   |
| **Agricultura/Pecuária** | 0        | 0        | 0         | 0         | 0             | 8014                 | 0    | 0                 | 8014  |
| **Água**               | 0        | 251      | 21        | 0         | 62            | 0                    | 8014 | 0                 | 8350  |
| **Restante (Outras)**  | 0        | 0        | 0         | 0         | 0             | 0                    | 42   | 0                 | 42    |
| **Total**              | 0        | 45977    | 3796      | 3363      | 3363          | 8014                 | 6893 | 8508              | 8508  |


<h4>RESPOSTA CORRETA:</h4>

![resposta-correta-2](https://github.com/user-attachments/assets/0c7e7fa0-50e6-4f1c-8899-f61d6a4fae04)

