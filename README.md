Predição e Análise de Risco de Obesidade
📌 Visão Geral do Projeto

Este projeto foi desenvolvido para um ambiente hospitalar com o objetivo de auxiliar equipes médicas na previsão dos níveis de risco de obesidade. Utilizando técnicas de Machine Learning, o sistema classifica pacientes com base em suas condições físicas e hábitos de vida.

📊 Contexto de Negócio

A obesidade é uma condição médica multifatorial. O objetivo desta ferramenta é fornecer uma abordagem orientada a dados (data-driven) para diagnóstico precoce e recomendações de saúde personalizadas.

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.13
Análise de Dados: Pandas, NumPy, Matplotlib/Seaborn
Machine Learning: Scikit-Learn (Random Forest Classifier)
Deploy: Streamlit
Serialização do Modelo: Joblib
📈 Principais Resultados
Acurácia do Modelo: 91,80% ✅
Base de Dados: 2.111 registros de obesidade (dataset UCI)
Categorias de Classificação: 7 níveis de obesidade (de Peso Insuficiente até Obesidade Tipo III)
Principais Variáveis: Peso, Altura, Monitoramento de Calorias, Frequência de Atividade Física
Modelo Utilizado: Random Forest (100 estimadores)
🚀 Como Executar
Início Rápido (Recomendado)

Dê um duplo clique no arquivo run_app.bat na pasta do GitHub e a aplicação será iniciada automaticamente.

Execução Manual
# 1. Criar ambiente virtual
python -m venv venv

# 2. Ativar o ambiente
venv\Scripts\activate

# 3. Instalar dependências
pip install -r requirements.txt

# 4. Acessar o diretório do projeto
cd obesity-risk-prediction

# 5. Treinar o modelo
python app/train.py

# 6. Executar a aplicação
python -m streamlit run app/app.py

A aplicação estará disponível em: http://localhost:8501

📁 Estrutura do Projeto
obesity-risk-prediction/
├── app/
│   ├── app.py                    # Aplicação web em Streamlit
│   ├── train.py                  # Script de treinamento do modelo
│   └── model_pipeline.pkl        # Modelo de ML treinado
├── data/
│   ├── Obesity.csv               # Base de dados original
│   └── processed_obesity.csv     # Base tratada
├── notebook/
│   └── model_pipeline.ipynb      # Notebook com análises
└── requirements.txt              # Dependências do projeto
🔧 Dependências

Veja o arquivo requirements.txt para a lista completa. Principais pacotes:

scikit-learn==1.6.1
streamlit>=1.53.0
pandas>=1.4.0
numpy>=1.23
matplotlib e seaborn para visualização