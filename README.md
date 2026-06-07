# Intelligent-compliance-analyzer.
The system acts as an intelligent layer between static, complex compliance documents (GDPR, SOC2, etc.) and the employees who need answers from them. Instead of manual searching, the AI uses RAG to fetch relevant context and provide precise, cited answers.

Interaction Step|   Sender Agent|         Receiver Agent|         Triggering Event|
Search Request      Compliance Analysis   Vector DB MCP           User input query
Risk Evaluation     Compliance Analysis   Risk Assessment         Retrieved context gathered
Data Fetch          Risk Assessment       BigQuery MCP            Need for historical context
Drafting            Compliance Analysis   Report Generation       All analysis complete

