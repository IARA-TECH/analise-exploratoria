# Análise Exploratória

Projeto em **Python (Jupyter Notebook)** para realizar **análise exploratória de dados (EDA)** sobre indicadores e registros do ecossistema **IARA**.  
O notebook `main.ipynb` conecta-se a um banco de dados PostgreSQL (via `SQLAlchemy`), carrega dados da tabela **`abacus_survey`** e executa etapas de inspeção, limpeza e visualização interativa com **Plotly**.

---

## 📚 Sumário

- [💡 Sobre o Projeto](#-sobre-o-projeto)
- [⚙️ Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [🧩 Como Executar](#-como-executar)
- [📊 Análises Realizadas](#-análises-realizadas)
- [🔐 Variáveis de Ambiente](#-variáveis-de-ambiente)
- [👩‍💻 Autor](#-autor)

---

## 💡 Sobre o Projeto

A **Análise Exploratória IARA** tem como foco **entender padrões, detectar inconsistências e extrair insights** a partir de dados armazenados no ecossistema IARA.

Etapas principais realizadas no notebook:

- Conexão segura ao banco de dados via variáveis de ambiente.
- Importação da tabela `abacus_survey` diretamente do PostgreSQL.
- Inspeção e limpeza de dados (valores nulos, tipos incorretos, duplicatas).
- Estatísticas descritivas (médias, medianas, frequências).
- Visualizações interativas com **Plotly** (distribuições, correlações e tendências).
- Preparação de dataset para futuras análises e modelos de IA.

---

## ⚙️ Tecnologias Utilizadas

| Categoria | Tecnologias |
| --- | --- |
| **Linguagem** | Python 3.9+ |
| **Ambiente** | Jupyter Notebook |
| **Bibliotecas Principais** | `pandas`, `numpy`, `plotly.express`, `sqlalchemy`, `python-dotenv` |
| **Banco de Dados** | PostgreSQL (ou Supabase) |
| **Gerenciamento de Ambiente** | `.env` para credenciais seguras |

---

## 🧩 Como Executar

### 1. Clonar o repositório
```bash
git clone https://github.com/IARA-TECH/analise-exploratoria.git
cd analise-exploratoria

# Crie e ative o ambiente virtual
python -m venv venv
# Linux / macOS
source venv/bin/activate
# Windows (PowerShell)
venv\Scripts\Activate.ps1

# Instale dependências
pip install -r requirements.txt

# Inicie o Jupyter Notebook e abra o arquivo
jupyter notebook main.ipynb
```
---

## 📊 Análises Realizadas

O notebook main.ipynb realiza as seguintes etapas de EDA:

* Importação de dados via SQLAlchemy e .env.
* Visualização geral com .head(), .info(), .describe().
* Tratamento de dados: remoção de nulos, renomeação de colunas e ajustes de tipos.
* Visualizações interativas com plotly.express (histogramas, scatter plots, distribuições).
* Cálculos estatísticos e agrupamentos com pandas.
* Correlação entre variáveis e identificação de padrões gerais.

---
## 🔐 Variáveis de Ambiente

| Variável |Descrição                                                                                                                                  |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `DB_URL` | URL de conexão completa com o banco de dados PostgreSQL ou Supabase. Exemplo: `postgresql+psycopg2://user:password@localhost:5432/iara_db` |


---

## 👩‍💻 Autor

**IARA Tech**

Projeto interdisciplinar para análise de dados e insights estratégicos do ecossistema IARA.

📍 São Paulo, Brasil  
📧 iaratech.oficial@gmail.com  
🌐 https://github.com/IARA-TECH