# AI Competitor Intelligence Agent Team

This project is a fully open-source **AI-powered competitor intelligence system** that I built to automate competitor discovery, website analysis, and market insight generation using a team of coordinated AI agents.

The application simulates a real-world market research workflow by combining semantic search, web crawling, and large language models into a single Streamlit app that produces structured competitor comparisons and strategic insights.

---

## Project Motivation

Manually researching competitors is slow, repetitive, and often incomplete. I built this project to explore how **multi-agent AI systems** can automate competitive intelligence tasks that are commonly done by product managers, analysts, and consultants.

The goal was to design a system where **multiple AI agents specialize in different roles**, collaborate with each other, and generate meaningful business insights from raw website data.

---

## What This Project Does

The application automatically:

* Finds competitors based on a company URL or description
* Crawls competitor websites
* Extracts structured business information
* Compares competitors across features, pricing, and positioning
* Identifies market gaps and opportunities
* Generates a comprehensive competitor analysis report

All results are presented through an interactive Streamlit interface.

---

## AI Agent Architecture

The system is built using a **multi-agent architecture**, where each agent has a clear responsibility.

### Research Agent

* Discovers and validates competitor companies
* Supports:

  * URL-based competitor discovery
  * Description-based company search
* Uses:

  * Perplexity AI (Sonar Pro) or
  * Exa AI semantic search

### Data Extraction Agent

* Crawls competitor websites using Firecrawl
* Extracts structured data such as:

  * Pricing models
  * Key features
  * Technology stack
  * Marketing focus
  * Customer feedback

### Market Analyst Agent

* Analyzes extracted competitor data
* Identifies:

  * Competitive positioning
  * Market gaps
  * Opportunities for differentiation
* Generates strategic recommendations

### Team Coordinator Agent

* Orchestrates communication between all agents
* Aggregates outputs into:

  * Comparison tables
  * Final market intelligence reports

---

## Key Features

* Multi-agent orchestration using **Agno (formerly Phidata)**
* Semantic competitor discovery
* Deep website crawling with structured extraction
* Automated competitor comparison tables
* Market gap analysis and strategic insights
* Streamlit-based interactive UI

---

## Tech Stack

* **Frontend:** Streamlit
* **Agent Framework:** Agno
* **Web Crawling:** Firecrawl
* **Search APIs:** Exa AI or Perplexity Sonar Pro
* **LLM:** OpenAI GPT-4o
* **Data Modeling:** Pydantic
* **Data Processing:** Pandas

---

## Prerequisites

* Python 3.10 or higher
* API keys for:

  * OpenAI
  * Firecrawl
  * Exa AI or Perplexity Sonar
* Basic Python programming knowledge
* VS Code or PyCharm recommended

---

## Installation

Navigate to the project directory:

```bash
cd ai_agent_tutorials/ai_competitor_intelligence_agent_team
```

Install required dependencies:

```bash
pip install -r requirements.txt
```

---

## API Keys Setup

The app securely collects API keys using the Streamlit sidebar at runtime.

Required:

* OpenAI API Key
* Firecrawl API Key
* Either Exa API Key or Perplexity Sonar API Key

---

## Running the Application

From the project folder, run:

```bash
streamlit run competitor_agent_team.py
```

The app will be available at:

```
http://localhost:8501
```

---

## How the Workflow Operates

1. User enters a company URL or description
2. Research Agent discovers relevant competitors
3. Data Extraction Agent crawls competitor websites
4. Market Analyst evaluates competitive positioning
5. Team Coordinator generates:

   * Comparison tables
   * Market gap analysis
   * Strategic recommendations

---

## Outputs

* Competitor comparison tables
* Pricing and feature analysis
* Market opportunity insights
* Strategic competitor intelligence reports

---

## Error Handling

* API key validation
* Graceful handling of failed crawls or searches
* Clear error messages displayed in the UI

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Designing multi-agent AI systems
* Orchestrating AI agents with specialized roles
* Using semantic search APIs
* Web crawling and structured data extraction
* Applying LLMs for business analysis
* Building production-style Streamlit apps

---

## Credits

This project was inspired by the **Awesome LLM Apps** open-source repository and the competitor intelligence tutorial by **Shubham Saboo and Gargi Gupta**, which I used as a reference while implementing and extending the system myself.

---

## License

This project is open-source. Please refer to the main repository for license details.

---

## Contributions

Feedback, suggestions, and improvements are welcome. Feel free to open an issue or submit a pull request.
