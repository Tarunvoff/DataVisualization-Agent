# 📊 AI Data Visualization Agent

An intelligent, conversational AI agent that analyzes datasets and generates insightful visualizations through natural language interaction. Upload your data, ask questions in plain English, and get instant analytical insights with automatically generated Python code and visualizations.

## 🎯 Use Case

### Problem Statement
Many organizations struggle with data analysis because:
- **Technical Barrier**: Non-technical users can't write SQL queries or Python code
- **Time Consumption**: Creating visualizations and reports is time-consuming
- **Expertise Gap**: Insight extraction requires data science knowledge
- **Tool Complexity**: Multiple tools (databases, BI software, Python) increase friction

### Solution
The **AI Data Visualization Agent** bridges this gap by providing a natural language interface to data analysis:

```
User Question (English) → AI Agent → Python Code Generation → Code Execution → Visualizations & Insights
```

### Who Should Use This?

✅ **Business Analysts** - Explore datasets without SQL expertise  
✅ **Product Managers** - Quick data-driven insights for decision-making  
✅ **Researchers** - Analyze research data and generate publication-ready visuals  
✅ **Data Teams** - Prototype analyses before formal reporting  
✅ **Students** - Learn data analysis concepts interactively  
✅ **Non-Technical Users** - Access data insights through conversational AI  

### Real-World Scenarios

#### Scenario 1: Sales Analytics
**Situation**: A sales manager has quarterly sales data but wants insights about top-performing products.  
**Traditional Approach**: Request a report from IT → wait days → get static report  
**With AI Agent**: Upload CSV → Ask "What are the top 5 products by revenue this quarter?" → Get instant visualizations and insights

#### Scenario 2: Customer Behavior Analysis
**Situation**: An e-commerce team has customer transaction logs and wants to understand purchase patterns.  
**Traditional Approach**: Write SQL queries → Manual chart creation → Send report  
**With AI Agent**: Upload data → Ask "Show me customer segments by spending patterns" → Get automatic clustering visualizations

#### Scenario 3: Research Data Exploration
**Situation**: A researcher has survey responses and needs exploratory data analysis.  
**Traditional Approach**: Learn Python → Write analysis scripts → Debug → Create plots  
**With AI Agent**: Upload CSV → Ask "What correlations exist between age and satisfaction score?" → Get statistical analysis and plots

## 🚀 Key Features

### 1. **Natural Language Interface**
- Ask questions in plain English
- No coding required
- Multi-turn conversations for follow-up questions

### 2. **Intelligent Code Generation**
- LLM generates Python code based on your queries
- Code is automatically extracted and executed
- Handles data loading, analysis, and visualization

### 3. **Safe Code Execution**
- E2B sandbox environment for secure execution
- No risk of malicious code affecting your system
- Isolated runtime for each analysis

### 4. **Automatic Visualizations**
- Charts, plots, and graphs auto-generated
- Multiple visualization types (bar, scatter, line, histogram, etc.)
- Publication-ready quality

### 5. **Session Management**
- API key configuration for Together AI & E2B
- Model selection for LLM inference
- Dataset persistence during conversations

## 🛠️ How It Works

### Architecture Flow

```
1. USER UPLOADS DATASET
         ↓
2. FILE STORED IN E2B SANDBOX
         ↓
3. USER ASKS QUESTION (Natural Language)
         ↓
4. TOGETHER AI LLM GENERATES PYTHON CODE
         + Instruction: Use dataset at provided path
         + Instruction: Generate visualizations
         ↓
5. E2B EXECUTES CODE IN ISOLATED SANDBOX
         + Safe execution environment
         + Returns results and visualizations
         ↓
6. RESULTS DISPLAYED IN STREAMLIT UI
         + Charts rendered
         + Summary insights shown
         + Code execution logs visible
```

### Workflow Example

#### User Query
> "Analyze the sales data. Show me the monthly revenue trend and identify the best performing region."

#### System Processing
1. **LLM Receives Context**: Dataset path + user query
2. **Code Generation**: LLM writes Python code using pandas/matplotlib
3. **Code Extraction**: System extracts Python from LLM response
4. **Sandbox Execution**: Code runs safely in E2B environment
5. **Result Display**: Visualizations and insights rendered in UI

## 💡 Use Case Benefits

### For Business Users
- 📈 Make data-driven decisions faster
- 🎯 No technical skills required
- ⏱️ Get insights in minutes, not days
- 💰 Reduce dependency on data teams

### For Data Teams
- 🔍 Quick prototyping and exploration
- 📊 Faster insights iteration
- 🤝 Better communication with stakeholders
- ⚡ Focus on complex analyses while AI handles exploratory work

### For Organizations
- 🏢 Democratize data access
- 📉 Reduce time-to-insight
- 🛡️ Safe, isolated code execution
- 🔄 Scale analysis without hiring more analysts

## 📋 Example Questions You Can Ask

- "What's the average order value by customer segment?"
- "Show me the top 10 products by sales volume this month"
- "Create a heatmap showing correlations between all numeric columns"
- "Identify outliers in this dataset"
- "Group customers by spending patterns and show distribution"
- "Create a funnel analysis for our conversion data"
- "What's the trend in monthly revenue over the past year?"
- "Show me the distribution of customer ages"

## 🔧 Technical Stack

| Component | Purpose |
|-----------|---------|
| **Streamlit** | User interface & web app framework |
| **Together AI** | Large Language Model for code generation |
| **E2B Sandbox** | Secure, isolated code execution environment |
| **Pandas** | Data manipulation and analysis |
| **Matplotlib** | Data visualization |
| **Python** | Core programming language |

## 📦 Installation & Setup

### Prerequisites
- Python 3.8+
- Together AI API key (free tier available)
- E2B API key (free tier available)

### Installation
```bash
pip install -r requirements.txt
```

### Run Application
```bash
streamlit run app.py
```

### Configuration
1. Get API keys:
   - Together AI: https://api.together.ai
   - E2B: https://e2b.dev

2. Input keys in the Streamlit sidebar
3. Select your preferred LLM model
4. Upload a CSV dataset
5. Start asking questions!

## 🎓 Perfect For

- 📊 **Data Exploration**: Understand your data quickly
- 🔬 **Research Analysis**: Analyze research data without coding
- 📈 **Business Intelligence**: Generate insights for reports
- 🧪 **Prototyping**: Test analysis ideas before formal implementation
- 👥 **Stakeholder Communication**: Create visuals for presentations
- 📚 **Learning**: Understand how AI generates and executes analysis code

## 🔒 Security & Safety

- **Isolated Execution**: Code runs in E2B sandbox, not on your machine
- **No Data Leakage**: Files stored only in sandbox during session
- **Safe LLM**: Trusted access to Together AI models
- **Controlled Operations**: Only data analysis operations allowed

## 📊 Supported Data Types

- CSV files (primary input)
- Numeric columns (for statistical analysis)
- Categorical columns (for grouping and segmentation)
- Time-series data (for trend analysis)
- Datasets up to memory limits of execution environment

## 🚀 Common Use Cases by Industry

### Finance
- Portfolio analysis
- Risk assessment
- Expense tracking
- Revenue forecasting

### E-Commerce
- Customer segmentation
- Sales trends
- Product performance
- Conversion analysis

### Healthcare
- Patient outcome analysis
- Treatment effectiveness
- Resource utilization
- Epidemiological studies

### Marketing
- Campaign performance
- Customer acquisition analysis
- Retention metrics
- Attribution analysis

### Education
- Student performance analysis
- Enrollment trends
- Graduation outcomes
- Course effectiveness

## 🎯 Getting Started

1. **Upload Your Data**: CSV files with your dataset
2. **Configure APIs**: Add Together AI and E2B keys
3. **Ask Questions**: Use natural language queries
4. **Get Insights**: Receive analysis and visualizations instantly
5. **Iterate**: Ask follow-up questions for deeper analysis

---

**Transform your data into actionable insights with the power of AI! 🤖📊**
