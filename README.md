# Projeto FarmTech Solutions - Fase 5

Este projeto foi desenvolvido para a FarmTech Solutions, focado em fornecer soluções de Inteligência Artificial e Computação em Nuvem para uma fazenda de médio porte. O objetivo principal é prever o rendimento de safras e estruturar a hospedagem da solução na AWS.

## 👥 Equipe
* **Integrantes:**
    * Matheus de Souza Santos - RM566901
    * Ricardo José Amorin - RM567312
    * Klaus Lohany Barbosa de Oliveira - RM
    * Paulo Roberto Silva Amaral Ribeiro Junior - RM568413
      

---

## 🚀 Entrega 1: Machine Learning

A Entrega 1 consistiu na análise de uma base de dados agrícola (`crop_yield.csv`) contendo variáveis de solo, temperatura e precipitação para prever a produtividade.

### Metodologia
* **Exploração de Dados:** Análise de correlação entre umidade, temperatura e precipitação.
* **Modelagem:** Foram testados diversos modelos de regressão para prever o rendimento.
* **Melhor Modelo:** O modelo **Extra Trees Regressor** apresentou os melhores resultados de predição (R² de aproximadamente 0.99).

### 📺 Vídeo da Entrega 1
Assista à demonstração do modelo preditivo:
* **Link:** [https://youtu.be/3umQKPlmfq4](https://youtu.be/3umQKPlmfq4)

---

## ☁️ Entrega 2: Computação em Nuvem (AWS)

Para hospedar a API de Machine Learning e processar os dados dos sensores, realizamos uma estimativa de custos utilizando a calculadora da AWS para uma instância Linux.

### 💰 Comparativo de Custos (On-Demand - 100%)
Configuração da máquina: 2 CPUs, 1 GiB RAM, 5 Gigabit de rede e 50 GB de armazenamento (EBS).

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

### 📺 Vídeo da Entrega 2
Demonstração da comparação de recursos na calculadora AWS:
* **Link:** [https://youtu.be/zbzFp9JnF70](https://youtu.be/zbzFp9JnF70)

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python
* **Bibliotecas:** PyCaret, Pandas, Scikit-learn, Seaborn, Matplotlib
* **Cloud:** AWS (EC2, EBS, AWS Pricing Calculator)
