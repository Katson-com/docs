# Introduction to the Data Insights Agent

The Data Insights Agent is a powerful enhancement for CentralQ Chat that allows you to analyze your Microsoft Dynamics 365 Business Central data directly within the chat interface. Ask questions in natural language and receive both textual summaries and visual charts based on your live Business Central data.

<div style="padding:49.27% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1085683957?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="centralq-chat-data-insights-sales-trend-with-follow-up"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

## Key Capabilities

- **Natural Language Queries**: Ask questions about your data the way you think. No need to learn query languages or navigate complex reporting tools. Simply type your business question, like "What were our sales for item X 
last quarter?"
- **Data-Driven Insights**: Go beyond raw numbers. Receive meaningful summaries and visualizations (e.g., bar charts, 
line graphs, pie charts) generated from your real-time BC data. Understand trends, identify outliers, and gain actionable 
insights quickly.
- **Unified Experience**: Access both knowledge-based guidance and data analysis in one interface.
- **Secure Analysis**: Your data interactions are handled securely, with transparent code generation.
- **Business Central Integration**: The agent is designed to work smoothly with your Business Central environment, 
leveraging the specific APIs available to you.

## What can you ask?

You can ask the Data Insights Agent various questions about your Business Central data:

- "Show me the sales trend for item 'ABC' in Q1 this year."
- "What are my top 5 best-selling products by revenue last month?"
- "Compare actual vs. budgeted expenses for the 'Marketing' department."
- "List customers who haven't placed an order in the last 90 days."
- "What is the average payment period for invoices closed last month?"
- "Show inventory levels for products in the 'Finished Goods' category."

## How It Works

When you ask a data-related question:

1. **Intent Detection**: CentralQ Chat identifies that your query requires data analysis.
2. **Code Generation**: An advanced AI model generates Python code specifically designed to answer your question using 
your available Business Central APIs.
3. **Secure Execution**: This code is executed in a secure, sandboxed environment. It fetches the necessary data 
from your BC instance and performs the requested analysis (e.g., calculations, aggregations).
4. **Result Presentation**: The system interprets the analysis results.
5. **Display Insights**: You receive a natural language answer with visualizations in the chat window.

!!! tip
    You can view the AI's reasoning process and generated code by expanding the "Thoughts" section in each response.

## Next Steps

- ➡️ **[Getting Started](./getting-started.md)**: Learn how to enable and start using the Data Insights Agent.
- ✨ **[Key Features](./features.md)**: Discover the full range of capabilities.
- ⚙️ **[How It Works (Detailed)](./how-it-works.md)**: Dive deeper into the technical architecture.
- 🛡️ **[Security Considerations](./security.md)**: Understand the security measures in place.
- 📊 **[Examples & Use Cases](./examples.md)**: Explore practical examples of data analysis queries. 