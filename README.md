# Fundamental of Database Design & Information Systems
## KT0103 & KT0104 - Class Activity 2: Types of Information Systems & IT Landscapes
## SuperMart SA - Enterprise Analysis
### Date: 19/10/2026

### 1. Transaction Processing System (TPS)
Daily operational transactions that must be recorded reliably:

**At Checkout Counters:**
- Point-of-Sale sales transactions (item scanned, quantity, price, VAT)
- Payment processing (cash, card, EFT, loyalty points)
- Receipt generation and barcode printing
- Returns and refunds processing

**At Inventory Warehouse:**
- Stock receipts from suppliers (Goods Received Note)
- Stock issue to store shelves (stock movement)
- Stock counts and adjustments (physical vs system stock)
- Low-stock alerts and reorder requests

TPS is critical because it is the source of all data. If TPS fails, SuperMart cannot sell or track stock.

### 2. Management Information Systems (MIS) & Decision Support Systems (DSS)

**MIS for Store Management (Weekly Sales Tracking):**
MIS takes raw TPS data and creates routine reports. Example: Every Monday, the MIS generates a report showing:
- Total sales per department (Grocery, Electronics, Clothing)
- Sales vs target, comparison to last week and same week last year
- Best and worst selling products, cashier performance.
Management uses this to monitor performance, not to make complex decisions.

**DSS for Decision Making (Promotion during sales drop):**
When MIS shows a sudden 20% drop in sales, the DSS helps management decide what to do. DSS is interactive and analytical.
- It can run What-If analysis: "What if we give 15% discount on grocery? What will profit be?"
- It can analyze historical data: "Did promotions work last time sales dropped in winter?"
- It combines external data: competitor prices, weather, payday dates.
Then it recommends: Run promotion on high-margin items this weekend.

Difference: MIS tells you WHAT happened, DSS helps you decide WHAT TO DO.

### 3. Executive Support Systems (ESS)

The CEO does not need daily checkout details. ESS provides high-level, strategic, mostly graphical information for long-term decisions.

**Examples for SuperMart CEO:**
1. **Static & Summarized Reports:** Yearly profit across all 50 branches in South Africa, overall market share.
2. **Competitor Data:** Benchmarking against Shoprite, Pick n Pay, Woolworths - pricing, new stores opened.
3. **Long-term Trend Forecasts:** 5-year forecast on consumer shift to online shopping, impact of inflation on spending, need to invest in e-commerce or close underperforming branches.
ESS data comes from MIS/DSS plus external sources (Stats SA, market research).

### 4. Knowledge Work Systems (KWS) & Office Automation Systems (OAS)

**KWS Example at SuperMart SA:**
Used by specialized knowledge workers. Example: A Data Analyst using Power BI or Python to create new customer segmentation models, or Graphic Designers using Adobe Illustrator to design new packaging and store layouts. KWS helps create NEW knowledge.

**OAS Example at SuperMart SA:**
Used by all staff for daily admin to increase efficiency.
- Microsoft Outlook for emails and meetings
- Microsoft Excel for daily rosters and admin schedules
- Microsoft Teams for communication between Head Office and branches
- Electronic document filing system for invoices.

### 5. IT Landscape & Legacy Systems

**Why connecting old legacy systems to new cloud apps increases complexity:**
SuperMart has used old systems for 15 years (e.g., old DOS-based POS, old payroll on local servers). New apps are cloud-based (e.g., Shopify Online, SAP S/4HANA Cloud).
1. **Incompatibility:** Legacy systems use old data formats and no APIs, while cloud apps use modern APIs. You need custom middleware/converters.
2. **Data Silos & Duplication:** Same product exists with different codes in old and new systems, causing errors.
3. **Security Risks:** Old systems have no modern encryption, connecting them to internet opens holes.
4. **Maintenance Cost:** You need staff who know both old and new tech.

**Two ways SuperMart SA can save costs using an IT Landscape Diagram:**

An IT Landscape Diagram is a visual map showing all applications, servers, how they connect, and their lifecycle.

**1. End-of-Life Asset Tracking:**
The diagram shows which systems are outdated and no longer supported by vendor (e.g., Windows Server 2012). SuperMart can see that it pays R50k/year supporting an old POS that vendor no longer updates. By retiring it and moving to one standard cloud POS, they save maintenance, license, and power costs and reduce risk.

**2. Standardization & Reducing Duplication:**
The diagram may show SuperMart uses 3 different inventory systems in 3 regions. IT can see this duplication and standardize to 1 single system for all branches. This saves on 2 extra licenses, training costs (staff learn one system only), and integration costs.
