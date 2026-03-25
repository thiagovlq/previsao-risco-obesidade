# Previsão e análise do risco de obesidade

## 📌 Visão Geral do Projeto
Este projeto foi desenvolvido para um ambiente hospitalar com o objetivo de auxiliar equipes médicas na previsão dos níveis de risco de obesidade. Utilizando machine learning, o sistema classifica pacientes com base em sua condição física e hábitos de vida.

## 📊 Contexto de Negócio
A obesidade é uma condição médica multifatorial. O objetivo desta ferramenta é fornecer uma abordagem orientada por dados para diagnóstico precoce e recomendações personalizadas de saúde.

## 🛠️ Stack Técnica
* **Linguagem:** Python 3.13  
* **Análise de Dados:** Pandas, NumPy, Matplotlib/Seaborn  
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)  
* **Deploy:** Streamlit  
* **Serialização do Modelo:** Joblib  

## 📈 Principais Resultados
* **Acurácia do Modelo:** 91.80% ✅  
* **Dataset:** 2.111 registros de obesidade do dataset UCI  
* **Categorias de Classificação:** 7 níveis de obesidade (Peso Insuficiente até Obesidade Tipo III)  
* **Principais Variáveis:** Peso, Altura, Monitoramento de Calorias, Frequência de atividade física  
* **Tipo de Modelo:** Random Forest (100 estimadores)  

## 🚀 Aplicativo Streamlit e Dashboard Power BI

Acesso o App pelo link abaixo:
https://previsao-risco-obesidade-thiago-vinicius.streamlit.app/

Acesso o Dash pelo link abaixo:
https://app.powerbi.com/view?r=eyJrIjoiNGUzMDk4ZjktZmE1MS00YmJlLWJiMGEtMDI0MmFiNjQ2YmY4IiwidCI6IjM3ZDlkN2ZlLWQ4ZWQtNGU2MS05OTNlLWUwMTcxMTlmZTFlZiJ9


### Início Rápido (Recomendado)
Dê um duplo clique em `run_app.bat` na pasta do GitHub e o app será iniciado automaticamente.

### Configuração Manual
```bash
# 1. Criar ambiente virtual
python -m venv venv

# 2. Ativar o ambiente
venv\Scripts\Activate

# 3. Instalar dependências
pip install -r requirements.txt

# 4. Navegar até o projeto
cd obesity-risk-prediction

# 5. Treinar o modelo
python app/train.py

# 6. Rodar o app
python -m streamlit run app/app.py
```

O app estará disponível em `http://localhost:8501`

## 📁 Estrutura do Projeto
```
obesity-risk-prediction/
├── app/
│   ├── app.py                    # Aplicação web em Streamlit
│   ├── train.py                  # Script de treinamento do modelo
│   └── model_pipeline.pkl        # Modelo treinado
├── data/
│   ├── Obesity.csv               # Dataset original
│   └── processed_obesity.csv     # Dataset processado
├── notebook/
│   └── model_pipeline.ipynb      # Notebook com análise
└── requirements.txt              # Dependências do Python
```

## 🔧 Dependências
Veja `requirements.txt` para a lista completa. Principais pacotes:
- scikit-learn==1.6.1  
- streamlit>=1.53.0  
- pandas>=1.4.0  
- numpy>=1.23  
- matplotlib & seaborn para visualização  
