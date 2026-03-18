# Projeto FarmTech Solutions - Fase 5

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap (1).png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<p align="center">
Faculdade de Informática e Administração Paulista - FIAP

</p>

Este projeto foi desenvolvido para a FarmTech Solutions, focado em fornecer soluções de Inteligência Artificial e Computação em Nuvem para uma fazenda de médio porte. O objetivo principal é prever o rendimento de safras e estruturar a hospedagem da solução na AWS.

## 👥 Equipe
* **Integrantes:**
    * Matheus de Souza Santos - RM566901
    * Ricardo José Amorin - RM567312
    * Klaus Lohany Barbosa de Oliveira - RM 566994
    * Paulo Roberto Silva Amaral Ribeiro Junior - RM568413
    * Victor Oliveira Fedeli Tate - RM566823    

---

## 🚀 Entrega 1: Machine Learning

A Entrega 1 consistiu na análise de uma base de dados agrícola (`crop_yield.csv`) contendo variáveis de solo, temperatura e precipitação para prever a produtividade.

### Metodologia
* **Exploração de Dados:** Análise de correlação entre umidade, temperatura e precipitação.
* **Modelagem:** Foram testados diversos modelos de regressão para prever o rendimento.
* **Melhor Modelo:** O modelo **Extra Trees Regressor** apresentou os melhores resultados de predição (R² de aproximadamente 0.99).

### Codigo no Google Colab
* **Link Colab** [https://colab.research.google.com/github/Matheus-Santos-AI/FarmTech-na-Era-da-Cloud-Computing/blob/main/Cap_1_FarmTech_na_Era_da_Cloud_Computing.ipynb]
  
### 📺 Vídeo demonstrativo da Entrega 1
Assista à demonstração do modelo preditivo:
* **Link:** [https://youtu.be/3umQKPlmfq4](https://youtu.be/3umQKPlmfq4)

---

## ☁️ Entrega 2: Computação em Nuvem (AWS)

Para hospedar a API de Machine Learning e processar os dados dos sensores, realizamos uma estimativa de custos utilizando a calculadora da AWS para uma instância Linux.

### 💰 Comparativo de Custos (On-Demand - 100%)
Configuração da máquina: 2 CPUs, 1 GiB RAM, 5 Gigabit de rede e 50 GB de armazenamento (EBS).

### Arquivo Orçamentario Gerado
[![PDF](https://img.shields.io/badge/Download-Orçamento_AWS-red?style=for-the-badge&logo=adobe-acrobat-reader&logoColor=white)](./Orçamento%20AWS%20sp%20-%20usa.pdf)


| Região | Custo Mensal (USD) | Custo Anual (USD) |
| :--- | :--- | :--- |
| **São Paulo (sa-east-1)** | $10.01 |$ 120.12 |
| **Norte da Virgínia (us-east-1)** | $5.53 |$ 66.36 |

*Dados baseados na exportação da calculadora AWS em 17/03/2026.*

### ⚖️ Justificativa de Escolha
Embora a região da Virgínia do Norte seja significativamente mais barata ($5.53 vs$ 10.01 mensais), a escolha estratégica para este projeto é a região de **São Paulo (South America)**.

**Motivos:**
1. **Latência:** O acesso rápido aos dados dos sensores é um requisito crítico. A proximidade geográfica reduz o tempo de resposta (RTT) da API.
2. **Conformidade Legal:** Existem restrições legais mencionadas para o armazenamento de dados no exterior. Utilizar a região de São Paulo garante que os dados permaneçam em território nacional, atendendo à LGPD e outras normas locais.

### 📺 Vídeo demosntrativo da Entrega 2
Demonstração da comparação de recursos na calculadora AWS:
* **Link:** [https://youtu.be/zbzFp9JnF70](https://youtu.be/zbzFp9JnF70)

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python
* **Bibliotecas:** PyCaret, Pandas, Scikit-learn, Seaborn, Matplotlib
* **Cloud:** AWS (EC2, EBS, AWS Pricing Calculator)
