the A2A flow as a sequence of events:

Step 1: Document Ingestion: The PDF Ingestion Agent watches for new documents. It extracts raw text, chunks it into smaller, meaningful segments, and uses an embedding model to convert text into vector representations.

Step 2: Storage: These vectors are pushed to the Vector Database MCP, which acts as the system's "long-term memory."

Step 3: Query Processing: When an employee asks a question in the Compliance Chat Assistant, the Compliance Analysis Agent receives it. It queries the Vector Database MCP to find the most relevant compliance clauses.

Step 4: Risk Evaluation: The Compliance Analysis Agent then triggers the Risk Assessment Agent. This agent analyzes the retrieved text for potential violations or gaps based on internal policy benchmarks (often pulled via BigQuery MCP).

Step 5: Reporting: Finally, the Report Generation Agent aggregates the retrieved facts and the risk assessment into a clean, human-readable summary.
