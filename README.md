# Projeto_Final
Projeto Final Bi Master - Business Intelligence Master
#### Aluno: [Silvana de Jesus Silva](https://github.com/Silvana-js)
#### Orientadora: [Manoela Kohler](https://github.com/manoelakohler)
---
Data:

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

https://github.com/Silvana-js/Projeto_Final.git

---

### Resumo

O tema saúde mental tem crescido nos últimos anos, principalmente agora em virtude da pandemia relacionada à COVID-19.

Tanto o mundo científico quanto o empresarial está cada vez mais está preocupado com esse tema e infelizmente estamos passando pelo pior momento da pandemia no Brasil até agora.

Pensando nisso, o objetivo desse trabalho é auxiliar na identificação se o paciente será diagnosticado com alguma condição de saúde mental. 

Utilizamos uma base do Kaggle (https://www.kaggle.com/ron2112/mental-health-data) de Fevereiro de 2021 para iniciarmos esse estudo, embora os dados estejam em inglês,  os conceitos básicos são os mesmos, os mesmos tipos de sintomas são sentidos em qualquer lugar do mundo.

### Introdução

O trabalho envolveu a análise de 8 modelos diferentes com o apoio da ferramenta o RapidMiner 9.9, em todos eles foram considerados as etapas: análise exploratória de dados, missing values e reavaliação dos atributos pelo peso.

### Fundamentação Teórica

A mineração de dados pode ser considerada como uma parte do processo de Descoberta de Conhecimento em Banco de Dados (KDD – Knowledge Discovery in Databases).

Dentro do universo da mineração de dados temos 5 classes de problemas:

Previsão, Classificação, Regressão, Agrupamento e Associação.
    
Destacamos que no caso desse trabalho foi feita análise através do método supervisionado - classificação, onde o rótulo é categórico.

### Modelagem

Primeiramente foi feita a análise dos dados para entender quais atributos manter no modelo, em seguida transformei os atributos nominais para numéricos com o operador 
Nominal to Numerical, além disso foi verificado quais atributos apresentaram missing values e com isso a funcionalidade de Replace Missing Values do RapidMiner foi utilizada.

Para entender a relevância de cada atributo em relação ao rótulo a ser classificado, as funcionalidades Weight by Information Gain e Select by Weights do RapidMiner foram consideradas para que somente os atributos com pesos relevantes fossem considerados.  

O balanceamento dos dados e processo para gerar as duas bases tratadas, nesse ponto fiz um processo no RapidMiner para gerar as duas bases, a de treino e a de teste.

Diferentes modelos foram testados usando os seguintes algoritmos de classificação: Decision Tree, Deep Learning, KNN, Naive Bayes, SVM, Random Forest, Random Tree e Neural Net.

Decision Tree

![image](https://user-images.githubusercontent.com/83094048/119270579-c60a7600-bbd3-11eb-9197-03e1e9683fc5.png)

Deep Learning

![image](https://user-images.githubusercontent.com/83094048/119270649-1a155a80-bbd4-11eb-8b34-7bca1a31cd00.png)

KNN

![image](https://user-images.githubusercontent.com/83094048/119270748-88f2b380-bbd4-11eb-815d-3a3a21b58a4b.png)

Naive Bayes

![image](https://user-images.githubusercontent.com/83094048/119270781-b17aad80-bbd4-11eb-9935-6965cff9f3cf.png)

Neural Net

![image](https://user-images.githubusercontent.com/83094048/119270858-31087c80-bbd5-11eb-8bc5-f3085b926165.png)

Random Forest

![image](https://user-images.githubusercontent.com/83094048/119270922-82b10700-bbd5-11eb-8e5b-6ed6c48566c2.png)

Random Tree

![image](https://user-images.githubusercontent.com/83094048/119271041-197dc380-bbd6-11eb-872b-d21736a48af8.png)

SVM

![image](https://user-images.githubusercontent.com/83094048/119271091-695c8a80-bbd6-11eb-8da8-8255699d8c79.png)

### Resultados

Índices de acurácia e kappa encontrados nos modelos:

1) Deep Learning 99.91% / 0.999
2) Neural Net 93.81% / 0.923
3) K-NN 86.05% / 0.824
4) SVM 84.79% / 
5) Decision Tree 80.30% /
6) Random Forest 79.34% /
7) Random Tree 70.62% /
8) Naive Bayes 68.18% /

### Conclusão

O modelo com a melhor acurácia foi o Deep Learning com 99.39% e o pior foi Naive Bayes com 68.18%.

### Considerações finais

Gostaria de agradecer a todos os professores do curso e em especial à professora Manoela Kohler pelas aulas e orientação nesse trabalho.

---

Matrícula: 192.671.163

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
