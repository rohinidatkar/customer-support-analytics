# Customer Support Analytics

## Project overview
A customer support analytics project that structures ticket data by category, channel, priority and resolution status. It measures first-response and resolution performance, repeat contacts, unresolved backlog and illustrative SLA attainment, then visualises the main service trends.

## Business questions
- Which query categories generate the most tickets?
- How quickly does the support team respond and resolve cases?
- Which categories or channels have the longest handling times?
- What proportion of tickets are repeat contacts?
- Which priority/category combinations contribute most to unresolved backlog?
- Are tickets meeting the example response and resolution targets?

## Key analysis
- Ticket data generation and quality checks
- Ticket volume and resolution-status analysis
- First-response and resolution-time metrics
- Category, channel and priority comparisons
- Repeat-contact analysis by customer and issue category
- Unresolved backlog ageing
- Illustrative priority-based SLA monitoring
- Dashboard-style charts and practical recommendations

## Repository structure
```text
customer-support-analytics/
├── README.md
├── requirements.txt
└── notebooks/
    └── customer_support_analytics.ipynb
```

## Run locally
1. Clone this repository.
2. Create and activate a Python virtual environment (recommended).
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
5. Open `notebooks/customer_support_analytics.ipynb` and run all cells.

The notebook generates the sample ticket data and writes CSV outputs to an `outputs/` folder relative to the notebook's working directory.

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.

## Dataset
The notebook generates 1,600 synthetic support tickets across six categories, four channels and four priority levels. Customer IDs are synthetic.

## Important assumptions
- SLA targets are examples only; organisations define SLAs differently.
- Response/resolution durations are generated as elapsed hours, not business hours.
- Repeat contacts are approximated as multiple tickets from the same customer in the same category. A production solution should use a linked case/reopen identifier or validated matching logic.
- All data and findings are synthetic and illustrative.

## Suggested next steps
- Exclude weekends and public holidays from business-hour SLA calculations.
- Add agent/team ownership and workload analysis.
- Track reopened tickets and customer satisfaction (CSAT).
- Build a Power BI dashboard using the exported CSV files.
