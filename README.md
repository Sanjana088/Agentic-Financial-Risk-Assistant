
# Agentic Financial Risk Assistant

An AI-powered financial assistant that leverages **Agentic AI, Retrieval-Augmented Generation (RAG), and Text-to-SQL** to analyze portfolio risk and generate personalized investment strategies.

This project demonstrates how modern AI systems can move beyond simple Q&A and act as a **decision-making layer over financial data systems**.

---

##  Key Features

*  **Agent-based architecture** using LangChain
*  **Portfolio risk analysis** and investment planning
*  **RAG-to-SQL pipeline** for querying structured financial data
*  **Memory-enabled interactions** using vector database (ChromaDB)
*  **Dynamic tool orchestration** (risk, portfolio, planning)
*  **End-to-end system** with Flask API and web interface

---

##   Architecture

![Architecture](architecture.png)

> The system dynamically decomposes user queries, selects relevant tools, retrieves financial data, and generates structured insights.

---

## Demo

### Example Query

> “I want to invest for buying a house”

### System Workflow

* Retrieves user portfolio data
* Evaluates risk exposure
* Identifies diversification gaps
* Generates tailored investment plan

### Output

* Risk score
* Suggested asset allocation
* Investment strategy recommendation

---

##  Tech Stack

* **Language**: Python
* **Backend**: Flask
* **AI Framework**: LangChain
* **LLM**: OpenAI
* **RAG System**: Vanna (Text-to-SQL)
* **Vector DB**: ChromaDB
* **Cloud**: Microsoft Fabric (Lakehouse + Data Warehouse)
* **Database**: SQL Server

---

## Run Locally (Demo Mode)

> Simplified mode without database setup

### 1. Clone the repository

```bash
git clone https://github.com/Sanjana088/Agentic-Financial-Risk-Assistant.git
cd Agentic-Financial-Risk-Assistant
```

### 2. Create virtual environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Create `.env` file

```text
OPENAI_API_KEY=your_api_key
OPENAI_MODEL=gpt-4o-mini
DEMO_MODE=true
```

### 5. Run application

```bash
python app.py
```

### 6. Open in browser

```text
http://127.0.0.1:7001/
```

---

## Full System (Advanced Setup)

Includes:

* Microsoft Fabric Lakehouse
* Azure authentication
* Real financial dataset

### Steps:

1. Configure Fabric credentials
2. Generate token:

```bash
python connection.py
```

3. Add credentials in `.env`
4. Train RAG system:

```bash
python FinancialGoals/RAGToSQL/TrainRAG.py
```

---

##  Database Overview

The system models a full wealth management pipeline:

* Clients
* Portfolios
* Assets
* Financial Goals
* Risk Metrics
* Historical Projections

Supports:

* Portfolio analysis
* Risk evaluation
* Financial planning

---

##  Why This Project Matters

Traditional financial tools are static and manual.

This system simulates how real-world financial advisors operate:

* Understanding user intent
* Retrieving relevant data
* Adapting strategies dynamically

It demonstrates how **Agentic AI can automate decision workflows**, not just answer questions.

---

## Future Improvements

* Real-time market data integration
* Advanced risk models (VaR, GARCH)
* Cloud deployment (Azure / AWS)
* Interactive dashboard visualizations

---

