# MYOB: the AI inside it, and the AI that connects to it

Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

MYOB has built AI into its small-business software under the name Iris by MYOB, and it has its own read-only connector for Claude and ChatGPT. [S1][S4]

Inside MYOB Business, Ask Iris answers plain-English questions about your numbers on Lite, Pro and AccountRight in the browser, and MYOB says that data is processed in Australia and isn't used to train AI models. [S3]

AI BAS helps you prepare your BAS through the quarter on Lite and Pro, but it's a paid add-on with a 12-month commitment, and it doesn't lodge for you. [S7][S8]

Smart Reconciliation and category suggestions match bank transactions for you, and some of the suggestions come from how other MYOB businesses coded similar transactions. [S12][S13]

The MYOB Connector lets Claude or ChatGPT read figures such as profit and loss, sales, receivables and payables. It can't change anything in MYOB, and the business owner has to allow it in My Account first. [S4][S6]

Once you connect, the figures you ask about go into the AI company's systems under its own terms, so MYOB tells you to turn off model training in Claude or ChatGPT. [S4]

There's no official MYOB link for Microsoft Copilot, Google Gemini, Zapier or Power Automate that we could find, so the documented fallback is exporting a report and uploading it, which copies your data out of MYOB. [S1][S32][S41][S55]

Building your own link through MYOB's API needs a paid developer membership, and MYOB's developer terms put firm limits on using its data with AI. [S47][S48]

MYOB's AI pages warn that the AI can get things wrong, and its terms make you responsible for checking AI output before you rely on it. [S1][S3][S8][S27]

## The tool, and the plans that matter

What AI you get depends on which MYOB product and plan you're on, so check yours first. [S2]

**Small-business plans in Australia** (prices are the "after offer period" figures shown on MYOB's pages on 15 October 2026; intro discounts were also showing) [S2][S25]

| Plan | What it is | Price after the intro offer | AI features MYOB lists for it |
|---|---|---|---|
| Solo by MYOB | A phone app for sole traders and freelancers, one user, no web version [S26] | $99/year [S2] | Category Suggestions [S2] |
| MYOB Business Lite | For sole traders and small businesses, payroll for up to 2 employees [S22] | $315/year [S2] | Ask Iris, Category Suggestions, Smart Invoice Reminders. AI BAS is "Available as an additional purchase" [S2] |
| MYOB Business Pro | Payroll for unlimited employees at an extra $3/month each [S23] | $70/month [S2] | Ask Iris, AI Business Insights (beta), Smart Reconciliation (beta), Category Suggestions, Smart Invoice Reminders. AI BAS is an extra purchase [S2] |
| AccountRight Plus | Needs a Windows computer for setup and some features; unlimited payroll included [S24] | $165/month [S2] | The same list as Pro, without AI BAS [S2] |
| AccountRight Premier | For multiple locations, jobs or currencies; Windows needed for setup and some features [S25] | $210/month [S25] | The product page mentions AI category suggestions [S25]. Premier isn't in the pricing page's AI comparison table [S2] |
| Payroll Only | A payroll-only plan [S2] | $15/month [S2] | None listed [S2] |

- The pricing page doesn't say whether these prices include GST. [S2]
- MYOB says it will change the prices of Payroll Only and the per-user Payroll premium feature from 1 November 2026, without showing the new prices. [S2]
- AccountRight Plus and Premier now sit under "MYOB Business" on MYOB's support site. [S63]

**Other MYOB products this guide covers**

- **MYOB Assist**, a phone app for quotes, invoices and receipt capture, included at no extra cost with Lite, Pro and AccountRight. [S17] It replaced the older MYOB Invoice and MYOB Capture apps. [S17][S18]
- **MYOB Acumatica**, MYOB's cloud ERP for mid-sized businesses. [S40][S56]
- **For accountants and bookkeepers:** MYOB Practice in the cloud (including Practice Compliance, Practice Management, Practice Tax, Practice BAS, Client Accounting and Nimbus Document Manager), plus the desktop products Accountants Office (AO) and Accountants Enterprise (AE). [S61]

**Where MYOB keeps your data**

- MYOB says its cloud storage is "hosted in Australia by Microsoft Azure and Amazon Web Services". [S29]
- MYOB says its information security management system is certified each year to ISO 27001. [S29]
- MYOB's privacy policy (August 2026) says related companies and third parties may be overseas, "including in New Zealand, the Philippines and the United States". [S28]
- The privacy policy doesn't mention artificial intelligence, machine learning or AI training. [S28]

## AI built in

MYOB groups most of its small-business AI under the name Iris by MYOB, which it calls the "intelligence engine built into your accounting software". [S1] It says availability "varies by feature and plan". [S1] MYOB says it designs these features in line with the Australian Government's Guidance for AI Adoption, with human oversight and transparency among its principles. [S1] You can see the data behind a suggestion, and override or ignore it. [S1]

MYOB's terms of use (June 2026) say it will tell you when a feature relies on AI, and that you're responsible for checking AI-generated information before relying on it. [S27] Beta features are used "at your own risk" under the same terms. [S27]

### Ask Iris (previously called AI Assistant)

**What it does.** A chat inside MYOB Business where you ask questions in plain English. [S3] It gives read-only answers about income, expenses, cash flow, profit and outstanding invoices, using your MYOB data. [S3] It also answers how-to questions about MYOB Business and general accounting terms. [S3] It handles follow-up questions and keeps your chat history. [S3] The help page says "Ask Iris only reads your data" and can't change your file, settings or business data. [S3]

**Where to find it.** In MYOB Business, click **Ask Iris** at the top of the screen. [S3] Use the **New chat** icon to start again and the **Chat history** icon to go back to an earlier chat. [S3]

**Plans and cost.** Available on MYOB Business Lite, Pro and AccountRight in the browser. [S3] The pricing page ticks it for Lite, Pro and AccountRight Plus. Solo doesn't have it. [S2] No extra charge is listed; it appears as a plan feature. [S2] The help page labels it "(Beta)" [S3], while MYOB's AI page says it's available now. [S1]

**On by default, and who controls it.** The docs we read don't say whether it's on by default or can be switched off. [S3] They don't mention any user-role limits either. [S3]

**Your data.** "Ask Iris doesn't use your business data to train AI models." [S3] "Your data is processed in Australia, kept within Australian systems", and MYOB says it isn't shared with third parties. [S3] The page doesn't say how long chats are kept. [S3] It warns "Ask Iris can make mistakes" and tells you to check important figures in your MYOB file before acting. [S3]

**In Australia.** Yes, and MYOB says Ask Iris data is processed in Australia. [S3]

### AI BAS (beta, paid add-on)

**What it does.** It works away during the quarter, as transactions come in. [S7] It:
- flags missing documents and possible GST issues [S8]
- suggests GST codes and categories, with an explanation for each [S8]
- suggests matches between uploaded documents and bank transactions [S8]

It shows a BAS readiness percentage that rises as you clear tasks. [S8] When you approve a suggestion, it updates your books. [S8] For employers, it also prepares PAYG withholding (labels W1 and W2). [S7][S8][S10] It covers simple quarterly BAS and cash-based scenarios (labels G1, 1A and 1B), with support due to expand. [S8] It produces a BAS decision report and a CSV of BAS-related transactions to share with your adviser. [S7][S8]

**What it doesn't do.** "AI BAS doesn't lodge with the ATO." [S8] You or your BAS agent lodge through your usual channel. [S8] MYOB says it "is not a registered tax agent" and you remain responsible for accuracy when you lodge. [S8]

**Where to find it.** **Accounting** menu > **AI BAS**. [S8] Its checklist has sections for **Missing documents**, **GST review**, **Categorise** and **Manual updates required**, each opened with **Review**. [S8] Suggestions have **Accept**, **Reject** and **Edit** buttons. [S8] When you're done, click **Save report**, and it moves to **Past BAS reports**. [S8]

**Plans and cost.**
- MYOB Business Lite or Pro only, for GST-registered Australian businesses. [S7][S8] It isn't offered on AccountRight or Solo in the pricing table. [S2]
- "AI BAS is a Premium Feature", an extra charge on top of your subscription. [S8] It's a 12-month subscription with an annual commitment, billed monthly in advance. [S8][S9] MYOB's terms describe it as a rolling 12-month term. [S27]
- On 15 October 2026 the AI BAS page showed it at $25 a month, labelled beta. [S7] From year two the page shows prices by BAS transactions per BAS period: [S7]

| BAS transactions per period | Non-employing | Employing |
|---|---|---|
| 1 to 100 [S7] | $25/month | $30/month |
| 101 to 750 [S7] | $40/month | $45/month |
| 750+ [S7] | $70/month | $75/month |

- The help page says the exact amount is shown in My Account before you confirm. [S8] MYOB was also advertising a bundle that discounts Lite or Pro for 12 months when bought with AI BAS, with bundle totals marked "(inc. GST)". [S7]
- Only the Primary Contact or Billing Contact on the MYOB account can add or cancel it. [S8][S9] Cancelling needs 10 days' notice by phone (1300 940 281), and you're billed for the rest of the 12-month commitment. [S8]
- Existing beta users: "You can continue using AI BAS, without any additional cost, for a limited time." [S8] After that they need to add it as a Premium Feature. [S8]

**On by default, and who controls it.** It's off until the Primary or Billing Contact adds it, either from **Accounting** > **AI BAS** or in My Account under **Manage my product** > **Manage my subscription** > **Add AI BAS**. [S8] Nothing in your books changes until you approve: "Your books will only update with your approval." [S7]

**Your data.** AI BAS "uses your MYOB data and AI models". [S8] It learns from your accepts, rejects and edits. [S7] The pages don't name the AI model provider or say where processing happens. [S7][S8] They also don't say whether your data trains models. [S7][S8] The help page warns "AI may omit or generate incorrect information". [S8]

**In Australia.** Australian businesses only. [S7][S8]

### Smart Reconciliation (beta)

**What it does.** MYOB matches bank feed transactions to your records as they arrive, so there's less to do at reconciliation time. [S12][S13] It works in this order: [S13]
- automatches to existing records using amount, date and contact name [S13]
- your bank rules [S13]
- AI category matches based on how you've matched similar transactions in your file [S13]
- suggested records that might match [S13]
- AI predictions, drawn from "how similar transactions have been matched across other MYOB businesses" [S13]
- manual matching by you [S13]

Each match shows a method label: **Logic**, **Rule**, **History**, **Prediction** or **Manual**. [S12] AI category matching works on a confidence score: [S12][S13]
- 90% or more: matched automatically [S12][S13]
- 70% to 90%: shown as a suggestion [S12][S13]
- below 70%: you match it yourself [S12][S13]

AI category matching only covers recent transactions, dated within 30 days of today and in the current financial year or later. [S13] It also skips anything dated before your lock date. [S13]

**Where to find it.** **Banking** > **Bank transactions**, with tabs **All**, **Not matched**, **Matched** and **Reconcile**. [S12] Expand a transaction and click **Accept**, or select several and click **Accept suggestions**. [S12] To reconcile, confirm the **Statement end date** and **Bank balance**, then click **Finalise** once the **Difference** is $0.00. [S12] If your page doesn't look like MYOB's examples, you don't have these features yet. [S12][S13]

**Plans and cost.** Ticked for Pro and AccountRight Plus, with a beta label. Lite and Solo don't have it. [S2] No extra charge is listed. [S2]

**On by default, and who controls it.** The help page says "Automatching settings are switched on by default" and, a line later, "You just need to switch on some settings to start." [S13] Check your own settings. To stop matching to records, deselect **Match to MYOB records** on the **Bank rules** page under the **Banking** menu. [S13] Category matching has its own setting on the same page. [S13] MYOB's FAQ says AI doesn't make final decisions; you finalise the reconciliation yourself. [S12] The pages don't say which user roles can change these settings. [S12][S13]

**Your data.** History matching learns from your own file. [S13] Predictions use patterns from other MYOB businesses, and MYOB says this happens "without exposing your business data to other customers". [S12] The pages don't say where the AI runs or which provider is used. [S12][S13]

**In Australia.** These are Australian help pages. [S12][S13] They don't say whether "other MYOB businesses" includes New Zealand businesses. [S12][S13]

### Category Suggestions

**What it does.** When you connect a bank account, AI suggests how to categorise transactions and explains each suggestion. [S22][S23] On AccountRight it suggests matches for bills and expenses. [S24][S25] It's the same AI category matching and prediction described under Smart Reconciliation. [S13]

**Where to find it.** In bank transaction matching. [S13]

**Plans and cost.** Ticked for Solo, Lite, Pro and AccountRight Plus. [S2] No extra charge is listed. [S2]

**On by default, and who controls it.** Category matching is controlled on the **Bank rules** page. [S13] We found no Solo help article covering it. [S26]

**Your data.** Predictions draw on how other MYOB businesses matched similar transactions. [S13]

**In Australia.** Yes, on the Australian plans above. [S2]

### Smart Invoice Reminders

**What it does.** Sends reminder emails for unpaid invoices on a schedule you set, up to five reminders. [S14] You choose a tone for each: Friendly, Neutral, Firm or Urgent. [S14] In the Overdue view, "For each overdue invoice, MYOB can suggest the next step": **Send reminder**, **Contact customer** or **Watch and wait**, based on invoice age, history and activity. [S14] The Overdue view also shows days overdue and each customer's average days to pay. [S14]

**Where to find it.** In MYOB Business: Settings (gear icon) > **Sales settings** > **Reminders** tab > select **Send reminders to all customers**, edit each reminder, then **Save**. [S14] For one customer: **Contacts** > open the customer > **Invoice reminders** > **Send reminders to this customer**. [S14] Overdue suggestions: **Sales** menu > **Invoices** > **Overdue**. [S14] In AccountRight, use the **Sales** command centre > **Invoice Reminders**, which opens the browser settings. [S14]

**Plans and cost.** Ticked for Lite, Pro and AccountRight Plus. Solo doesn't have it. [S2] No extra charge is listed. [S2]

**On by default, and who controls it.** Reminders only go out after you switch them on. [S14] Once saved, they're emailed to customers automatically on the schedule. [S14] Turn them off by deselecting **Send reminders to all customers**, then **Confirm** and **Save**. [S14] They don't go out for invoices on Prepaid or Cash on delivery terms. [S14] The page doesn't say which user roles can change the settings. [S14]

**Your data.** The help page describes "intelligent insights and suggested actions" but doesn't explain what technology is used or how data is handled. [S14]

**In Australia.** Yes, on the Australian plans above. [S2]

**Note.** MYOB's March 2026 announcement said the feature would offer tone suggestions [S11]; the current help page has you pick the tone yourself. [S14]

### AI Business Insights (beta)

**What it does.** AI-written summaries and charts about your sales, customers, cash flow and spending, with "Your numbers" charts behind them. [S15][S16] Metrics include total income, average invoice value, cash runway, average time to get paid, net profit and profit margin. [S16] Insights refresh overnight [S16], at most once every 24 hours per ledger and only when there are meaningful changes. [S15] It doesn't replace your standard reports. [S16]

**Where to find it.** On the MYOB Business dashboard, look for the purple AI Business Insights banner and click **View Latest Insights**. [S16] Use **Check recent insights** for the feed, or **Your numbers** for the charts. [S16]

**Plans and cost.** Selected Pro and AccountRight browser customers in Australia and New Zealand, during beta. [S15] The pricing page ticks it for Pro and AccountRight Plus with a beta label. [S2] No extra charge is listed. [S2] You can ask MYOB support for early access. [S16]

**On by default, and who controls it.** Beta participants see a banner and in-product message. [S16] Only users with the **Administrator** or **Accountant/Bookkeeper** role can see the insights. [S15][S16] It needs an active bank feed. [S16]

**Your data.** It uses the financial data already in your MYOB file, including bank feed transactions and balances. [S15][S16] The first release doesn't use outside marketing or CRM data. [S15] The pages don't say whether the data trains models or where it's processed. [S15][S16] They don't mention third parties either. [S15][S16] MYOB says "AI can still get things wrong" and that the insights aren't financial advice. [S15]

**In Australia.** Yes, for selected customers. [S15]

### Reading bills and receipts (Uploads, In Tray and the MYOB Assist app)

**What it does.** When a bill or receipt reaches Uploads or the In Tray, MYOB pre-fills a bill or spend money transaction from it, with details such as supplier, dates, amounts and invoice number. [S20][S19] MYOB Assist "uses AI to read and process the captured receipts and bills". [S18] The Assist product page says AI pulls out the total, GST and date. [S17] MYOB's 2025 updates list "upgraded AI-powered OCR" for receipts and bills. [S21]

**Where to find it.**
- MYOB Business (browser): **Uploads** in the Purchases area. Click the ellipsis (**...**) on a document, then **Create bill**, **Create spend money transaction** or **Link to existing bill**. [S20]
- AccountRight desktop: **Purchases** command centre > **In Tray** (online company files only). [S20]
- Each company file has its own uploads email address, shown on the **Uploads** screen. [S20]
- In the MYOB Assist app, photograph the receipt or pick a saved photo, then crop it and add a note if you like. It goes to Uploads or the In Tray. [S19]

**Plans and cost.** MYOB Assist is included at no extra cost with Lite, Pro and AccountRight. [S17] Uploads take PDF, JPG, TIFF and PNG files up to 10 MB. [S20] No charge for uploads is mentioned. [S20]

**On by default, and who controls it.** Documents are read when you upload them, and you choose what to create. [S20] In AccountRight desktop, an administrator can remove In Tray access from a role (**Setup** > **User Access** > **Manage Roles**). [S20] The **Field** role gives staff the Assist app only, without access to MYOB Business. [S18][S31]

**Your data.** Deleted uploads are gone for good, so download a copy first if you need one. [S19][S20] The pages make no statement about AI training or processing location for document reading. [S17][S20]

**In Australia.** Yes. [S17][S20]

**Coming.** MYOB says Assist will add "agentic AI capabilities" over time, with no timeline. [S17]

### For practices: AI mapping in MYOB Practice Compliance

**What it does.** Client ledger data "intelligently maps to one standardised chart of accounts", so one workflow works across clients. [S60] Data comes in by live sync or CSV, and the page names MYOB and QuickBooks as sources, plus trial balance imports. [S60] It also surfaces "risk flags and client insights" inside the workflow. [S60]

**Where to find it.** In MYOB Practice, signed in at partner.myob.com. [S61]

**Plans and cost.** AI mapping and insights are included in Core Compliance and Pro Compliance. Starter Compliance doesn't include them. [S60] We didn't capture Practice Compliance prices.

**On by default, and who controls it.** Not stated. [S60]

**Your data.** The page doesn't say how the AI mapping handles data or where it's processed. [S60] It's also silent on training. [S60]

**In Australia.** Yes, on MYOB's Australian site. [S60]

**Other practice AI.** MYOB's accountants and bookkeepers page names no other AI features for practices. [S61] Advisers can review and adjust a client's AI BAS work with their usual MYOB access [S7], and the Accountant/Bookkeeper role can see AI Business Insights. [S16]

### MYOB Acumatica AI (larger businesses)

**What it does.** MYOB lists these features: [S56]
- **AI Assistant**, for plain-English questions about revenue, customers, invoices, inventory and performance [S56]
- **AI Automation**, for building AI-powered workflows (approvals, document processing, pricing, notifications) [S56]
- **AP Bill Entry**, which reads supplier bills and checks them against supplier records [S56]
- **Expense Management**, which captures expenses from receipts in the mobile app [S56]
- **Anomaly Detection**, which flags unusual transactions [S56]
- **Production Variance Anomaly Detection**, **Cross-Sell Assistant** and **Auto Complete** [S56]

In version 2026.1.1, "AI Studio" was renamed **AI Automation** and "Detection of Anomalies in Generic Inquiries" became **Anomaly Detection**. [S58] Journal entry anomaly detection marks entries Normal, Medium or Significant for you to review. [S59]

**Where to find it.** Switch on **AI Studio** and **Anomaly Detection** on the **Enable/Disable Features (CS100000)** form. [S58][S59] Journal anomalies appear in **Journal Entries Analysis (GL3010ML)**. [S59]

**Plans and cost.** Not stated on the pages we read. [S56][S58] AI Studio opened in early access in May 2026, with wider availability planned later in the year. [S57]

**On by default, and who controls it.** These features have to be enabled on the CS100000 form. [S58][S59] MYOB says the AI respects the user permissions and access controls already in place. [S56]

**Your data.**
- "Customer data is not used to train external AI models." [S56]
- "MYOB Acumatica stores customer data in Australia." [S56]
- Depending on the feature, data may be processed in Australia or on AI infrastructure run by providers including Anthropic, AWS and Microsoft, which MYOB says "cannot store it or use it to train their models". [S56]
- AI Automation runs on MYOB's managed infrastructure on AWS, with models through AWS Bedrock. [S56] MYOB says AI Studio processing runs in local data centres. [S57]
- Customers can also use their own preferred AI model. [S57]
- Journal entry anomaly detection sends the inquiry data to an external AI service, which the release note doesn't name. [S59]

**In Australia.** Data is stored in Australia. [S56]

## Outside AI that connects

In plain words, a connector lets a chat assistant such as Claude or ChatGPT look things up in another app while you're chatting. [S33] MYOB has built one, called the MYOB Connector, for Claude and ChatGPT. [S1][S4] It runs on an MCP server, which is the standard kind of plug that Claude's connectors use. [S6][S34] MYOB's sits at https://mcp.myob.com/mcp. [S6]

Before anyone can connect, the business owner has to allow it. The help page says "the business owner (the Owner user in the MYOB Business file) must allow access". [S4] After that, "a user who has access to the MYOB Business file and their own Claude or ChatGPT account" can connect. [S4]

### Claude and MYOB

**Official?** Yes. It's MYOB's own connector, listed in Anthropic's Connectors Directory as "MYOB", made by MYOB, with the "Anthropic verified" label. [S6] The listing says it was added in July 2026 and "This feature is currently in beta." [S6] MYOB announced it on 17 August 2026, with a phased rollout from August. [S5] Anthropic says verification means it tested the tools for quality, and it "isn't a security audit". [S35]

**What it can see and do.**
- Read-only. "The connection with MYOB is read-only." [S4] MYOB says it "can't create, edit or delete anything in your MYOB account". [S4]
- Anthropic's listing shows seven tools, all for getting information: business details, financial year dates, outstanding customer balances, outstanding payables, profit and loss, sales invoice totals, and standard payment terms. [S6]
- MYOB says you can ask about revenue and profit, expenses, receivables and overdue invoices, and cash position. [S4]
- It doesn't cover payroll, inventory or job tracking, year-end tax advice or lodgement, or MYOB help content. [S4]
- It can only reach what your own MYOB user permissions allow. [S4] Claude inherits each person's permissions from the connected service. [S33]
- Example questions from MYOB: "Do I have any overdue invoices?" and "What is my cash position?" [S4]

**What you need.**
- An active MYOB Business Pro, Lite or AccountRight subscription. [S4]
- Your own Claude account. [S4] Anthropic says web connectors are available for all users on Claude, Claude Desktop and Claude Mobile. [S33]
- Your MYOB username and password. [S4]
- The MYOB file's Owner user must first allow Claude in My Account. [S4]
- On Claude Team and Enterprise plans, an Owner or Primary Owner must enable the connector for the organisation before members can connect. [S33][S34] On Team plans, members without that permission see a **Request** button that goes to the Owners. [S34]
- Access is being rolled out gradually, so MYOB may not show up for you yet. [S4]

**Steps to connect** (MYOB help page, no date shown, read 15 October 2026) [S4]

First, the Owner user in MYOB:
1. Sign in to My Account (myaccount.myob.com). [S4]
2. If you have several MYOB businesses, choose the one to allow. [S4]
3. From the quick links on the right, click **Manage AI connections**. [S4]
4. Click **AI file access**. [S4]
5. Find the business and allow access for **Claude**, **ChatGPT** or both. [S4] Allowing access doesn't connect anything by itself. [S4]

Then anyone with access to that file, in Claude:
1. Go to the Connectors directory in your Claude account. [S4] (Anthropic's path is **Customize** > **Connectors**, then **+**.) [S33]
2. Search for MYOB, then click **Connect to Claude**. [S4]
3. If prompted, enter your MYOB username and password. [S4]
4. If you can see more than one MYOB Business file, choose the one to connect. [S4]
5. At the confirmation, click **Done**. [S4]

In a chat, you can switch connectors on or off for that conversation from the **+** menu > **Connectors**. [S33]

**To disconnect.**
1. In Claude, go to the Connectors directory and open MYOB. [S4]
2. Click **Disconnect**. [S4]

To switch to a different business file, disconnect and then connect the other one, which must also be allowed in My Account. [S4] The help page doesn't explain how the Owner withdraws access in My Account. [S4]

**Limits.**
- Beta, rolling out gradually. [S4][S6]
- One business file per connection, going by MYOB's switching instructions. [S4]
- In **Customize** > **Connectors**, each of the connector's tools can be set to **Always allow**, **Needs approval** or **Blocked**. On Team and Enterprise plans, Owners can restrict these for everyone. [S33]
- MYOB's sign-in protects your password: "Claude or ChatGPT doesn't see or store your MYOB password". [S4]
- Your chat is still covered by Claude's own privacy settings and terms. [S4] MYOB tells you to go to **Settings** > **Privacy** and turn off **Help improve our AI models**. [S4][S36] On Claude's Free, Pro and Max plans, if that setting is on, Anthropic says chats may be kept in de-identified form for up to five years in training pipelines. [S36][S37] Deleted chats are removed from Anthropic's back-end within 30 days. [S37]
- Claude's memory can hold older figures that aren't live MYOB data. [S4] Manage it in **Settings** > **Memory**. [S4]
- For anything the connector doesn't cover, the fallback is exporting a MYOB report and uploading the file to Claude, which accepts PDF, CSV and XLSX files. [S32][S38] Payroll reports carry employees' personal details, so think before uploading those. (Our note.)
- Anthropic says connected services process data on their own infrastructure under their own terms. [S33] Anthropic's advice for any connector it didn't build: "Only use connectors from developers you trust." [S6][S35]

### ChatGPT and MYOB

**Official?** Yes. MYOB says the same MYOB Connector is installed in ChatGPT as a plugin. [S1][S4][S5] OpenAI's plugin directory, which replaced its App Directory on 9 July 2026, lists **MYOB**, made by MYOB Australia Pty Ltd, version 1.0.0. The listing says "This feature is currently in beta." [S66][S71]

**What it can see and do.** MYOB describes the same read-only connector for both Claude and ChatGPT, with the same supported and unsupported topics as above. [S4] OpenAI's listing describes a read-only view of profit and loss, sales, receivables and payables. It says access is "read-only in this phase, with no write actions", and it doesn't list the individual tools. [S66]

**What you need.**
- An active MYOB Business Pro, Lite or AccountRight subscription. [S4] OpenAI's listing asks for an active MYOB Business subscription in Australia or New Zealand. [S66]
- Your own ChatGPT subscription. [S4] MYOB doesn't name a ChatGPT plan. [S4] OpenAI doesn't list plans for it either. It says using any plugin depends on your plan, workspace, role and region. [S67]
- In ChatGPT Business, apps start switched on. In Enterprise and Edu, new plugins and apps generally stay off until an admin reviews them. [S68]
- Your MYOB username and password. [S4]
- The MYOB file's Owner user must first allow ChatGPT in My Account (the same five steps as for Claude). [S4]

**Steps to connect** (MYOB help page, no date shown, read 15 October 2026) [S4]
1. In ChatGPT, open **Plugins**. [S4]
2. Search for MYOB, then click **Install plugin**. [S4] (OpenAI's general instructions describe opening the plugin's details and selecting the plus button, then approving its requested permissions.) [S39]
3. If prompted, enter your MYOB username and password. [S4]
4. If you can see more than one MYOB Business file, choose the one to connect. [S4]
5. At the confirmation, click **Done**. [S4]

**To disconnect.**
1. In ChatGPT, open **Plugins** and find MYOB. [S4]
2. Click the three dots at the top right and choose **Uninstall**. [S4]

OpenAI's own guide says "Separately connected MCP server integrations remain connected in ChatGPT until you disconnect them there." [S39] After uninstalling, check that no MYOB connection is left in ChatGPT. (This is our caution; MYOB's page doesn't mention it.)

OpenAI's help centre adds that uninstalling a plugin can disconnect every account connected through it, after a warning. To disconnect only the account, go to **Settings** > **Plugins** > MYOB > the account's **•••** menu (or **Connection**) > **Disconnect**. [S69]

**Limits.**
- ChatGPT doesn't use MYOB automatically. Select the MYOB plugin before each question; "If it isn't selected, ChatGPT defaults to a web search." [S4] MYOB warns you could get a plausible-looking answer that isn't based on your MYOB data. [S4]
- MYOB tells you to turn off **Improve the model for everyone** in **Settings** > **Data Controls**. [S4] OpenAI says that on Free, Go, Plus and Pro it may use information from apps to train its models while that setting is on. Business, Enterprise and Edu aren't used for training by default. [S70]
- OpenAI's listing says ChatGPT may share relevant chats and memories with MYOB, under MYOB's terms and privacy policy. [S66]
- Manage memory in **Settings** > **Personalization** > **Memory**. [S4] Deleting a chat may not delete memories made from it. [S4]
- When ChatGPT sends data through an MCP server, that service's terms and privacy policy apply. [S39]

### Other AI tools and MYOB's MCP server

**Official?** Only for Claude and ChatGPT. The My Account screen lets the Owner allow "Claude, ChatGPT or both", and MYOB documents no other AI tools. [S4]

**What it can see and do.** Not documented for other tools. [S4]

**What you need, steps, disconnecting.** Not documented. [S4]

**Limits.** Anthropic notes that any connector URL can be added to Claude as a custom connector. [S35] Because MYOB's permission screen only names Claude and ChatGPT, it appears other AI tools can't use MYOB's server. That's our inference; MYOB doesn't say.

### Microsoft Copilot and MYOB

**Official?** No. We found no MYOB connector for Microsoft 365 Copilot or the Copilot apps. [S40][S41]
- MYOB and Microsoft signed a five-year partnership on 8 April 2026. [S40] It's about MYOB building its own AI with Microsoft technology: Microsoft Foundry for customer-facing AI agents, Copilot Studio for MYOB's own staff, and Agent 365 for governance. [S40] The announcement doesn't describe any link between MYOB and Microsoft 365 Copilot. [S40]
- The first jointly built customer features were due "later in 2026". [S40]
- Microsoft's list of connectors for Power Automate, Power Apps and Logic Apps (updated 2 October 2026) has no MYOB connector. [S41]

**The documented alternative: export to Excel, then use Copilot in Excel.**
- What it can see and do: whatever is in the exported report. Copilot in Excel can summarise data, make charts and PivotTables, and answer questions about it. [S42] It can also edit the sheet, and opens in **Allow editing** mode by default. [S42] Any edits stay in the copy and never reach MYOB. (Our note.)
- What you need: a MYOB report you can open, desktop Excel 2010 or later for MYOB's Excel export [S32], and a Microsoft 365 setup that includes Copilot. Microsoft says Copilot may not be included in your subscription. [S42]
- Steps:
  1. In MYOB Business, open the report you want, such as Profit and Loss. [S32]
  2. Filter it or change columns if you need to. [S32]
  3. From the **Export** menu, choose **Excel**, then click **Export**. The file saves to your Downloads folder. [S32]
  4. Open the file in Excel and select the Copilot icon in the lower-right corner. [S42]
  5. Choose **Allow editing**, **Plan** or **Chat only**, and ask your question. [S42]
- In AccountRight desktop, export from **File** > **Export** as PDF, Excel, XPS, CSV or TSV. [S32]
- To disconnect: there's no live connection, only a copied file. Delete it when you're done if you don't need it. (Our note.)
- Limits: the copy is out of date as soon as it's made, and MYOB's access controls don't follow it. (Our inference.)

### Google Gemini and MYOB

**Official?** No. MYOB's AI pages name only Claude and ChatGPT. [S1][S4] We found no MYOB extension for Gemini.

**The documented alternative: export, then upload the file to Gemini.**
- What it can see and do: only what's in the file you upload. [S43]
- What you need: a Google account signed in to Gemini Apps. [S43] Gemini accepts spreadsheets and documents, up to 10 files per prompt and 100 MB per file. [S43]
- Steps:
  1. Export the report from MYOB as Excel or PDF (steps above). [S32]
  2. In Gemini on the web, type your prompt, click **Add files**, then **Upload files**. [S43]
  3. Choose the file and click **Submit**. [S43]
- To disconnect: there's no connection. Uploaded files count toward your Gemini Apps activity storage, and deleting that activity frees the space. [S43]
- Limits: Google's upload page doesn't say how uploaded files are used for model training. [S43]

### Your own app or automation and MYOB (the MYOB API)

**Official?** Yes, MYOB has a public API, called the MYOB Business API (also known as the AccountRight API). [S44] An API is how other software reads and writes data in MYOB, under rules MYOB sets. [S44][S47] Using it is a job for a developer, who has to register an app with MYOB first. [S44]

**What it can see and do.** Apps can read and write. For example, the sale invoice endpoint supports "GET | PUT | POST | DELETE", meaning read, update, create and delete. [S65] Access is split into granular scopes such as sme-sales, sme-purchases, sme-banking, sme-payroll and sme-general-ledger, and apps should request only the ones they need. [S45][S46]

**What you need.**
- Membership of MYOB's Developer Program. The cheapest listed tier is $110 a month, and the page says "Pricing includes GST". [S48] The page mentions no free API access. [S48]
- An app registered in my.MYOB to get an API key and secret. [S44]
- A file administrator to approve access: MYOB's consent flow "requires an admin to approve consent to a single ledger". [S46]
- The app also sends the company file's username and password in a header with each call. [S45]

**Steps to connect** (developer docs: Getting Started updated April 2023, Authentication March 2025, Granular Data Scopes November 2025)
1. Join the Developer Program by choosing a level and filling in the form. [S48]
2. Submit the API access registration form. MYOB sets up a my.MYOB login and invites you to a sandbox company file. [S44]
3. In my.MYOB, open the **Developer** tab and click **Register App**. Enter the app name and redirect URL, then click **Register App**. [S44]
4. Your API key and secret appear on screen. [S44]
5. Your app sends the user to MYOB's sign-in page, asking for the scopes it needs. [S45][S46]
6. A MYOB administrator approves the request for one company file. [S46]
7. The app swaps the returned code for an access token and starts making calls. [S45]

**To disconnect.** The developer docs we read don't describe how a business revokes an app's access. Either party can end the developer agreement with 30 days' notice, and MYOB may switch off credentials unused for 12 months. [S47]

**Limits, including MYOB's AI rules for developers** (Developer Program and Platform Terms, updated 12 March 2026) [S47]
- Developers must not use MYOB data to train or improve any AI model (clause 31). [S47]
- If an app uses an outside AI service, that service must be contractually barred from training on MYOB data (clause 32). [S47]
- Developers "must not operate, expose or offer any model‑context, agent‑orchestration or similar protocol server" that wraps MYOB's API as generic tools for outside AI agents (clause 34). [S47]
- Bulk or persistent export of MYOB data is restricted (clause 27). [S47]
- MYOB may monitor and rate-limit to catch "behaviour indicative of LLM‑related misuse" (clause 42). [S47]
- Data must not be stored or processed in a country that would breach MYOB's data residency requirements (clause 29). [S47] MYOB's security requirements treat Australia and New Zealand as low-risk and ask developers to contact MYOB before storing data elsewhere. [S49]

### Zapier, Make and Power Automate and MYOB

**Official?** No official MYOB integration that we could confirm on any of the three. [S41][S55]
- **Zapier:** Zapier's MYOB page, as shown in search results, says MYOB "has not yet built an integration on Zapier". [S55] The page itself returned "not found" when we loaded it directly. [S55]
- **Make:** We couldn't confirm either way. Make's MYOB page didn't load properly. (See gaps.)
- **Power Automate:** Microsoft's connector list has no MYOB connector. [S41]

**What it can see and do, what you need, steps.** Nothing official to document. Zapier suggests building your own connection with webhooks or code [S55], and with MYOB that would mean using the API, which needs Developer Program membership. [S48] That's our inference about how it would work.

**Limits.** A home-made automation that feeds MYOB data to an AI would fall under MYOB's developer terms above. [S47]

### Marketplace AI apps and MYOB

**Official?** These are third-party apps listed in MYOB's marketplace. A listing is a directory entry. MYOB says "The apps on this site are developed by third parties." [S51] It adds that it "can't guarantee that the apps are suitable for your business". [S52]

**What MYOB checks before listing.** It reviews the app's sign-in (OAuth) flow, company file access and the data flowing between the app and MYOB. [S50] MYOB describes its role as "a directory type service". [S50]

**Apps listed that describe themselves as using AI** (we checked a handful of the 350+ apps) [S51]
- **Dext** (Dext Software Limited): "AI-powered extraction" of receipts, invoices and expenses, plus "Dext AI Assist". Works with MYOB AccountRight, MYOB Business and MYOB Essentials. [S52]
- **Accounts Payable – AP Automation Solution for MYOB** (Dataline Group): "AI driven data extraction and validation" for supplier invoices. Works with AccountRight, MYOB Acumatica and MYOB EXO Business. [S53]
- **Lightyear**: purchasing and accounts payable with line-item extraction from scanned documents; it describes "intelligent automation". Works with AccountRight and MYOB Acumatica. [S54]

**What you need, steps, disconnecting.** Each app has its own sign-up and pricing, shown on its own site. [S52][S53][S54]

**Limits.** Under MYOB's terms, installing an outside app means you consent to it accessing your data "as required" to work with MYOB Business. [S27] MYOB's terms limit its liability for what an outside app does with your data. [S27]

## Jobs it's good for

**For a small business**

- **"How did last month go?" without building a report.** Ask Iris answers questions like "What was my total income last month?" inside MYOB, with data processed in Australia. [S3]
- **Checking who owes you from a chat you already use.** With the MYOB Connector, ask Claude or ChatGPT "Do I have any overdue invoices?" or "Who are my biggest customers by revenue?". [S4] The connector can't send anything, so any follow-up still goes out from MYOB. [S4]
- **Getting paid sooner.** Set up to five automatic reminders with the tone you want, and check the Overdue tab's suggested next step for each late payer. [S14]
- **Keeping on top of the bank feed.** On Pro or AccountRight Plus, Smart Reconciliation matches transactions as they arrive; you accept suggestions in bulk and finalise. [S2][S12]
- **BAS through the quarter.** If you're GST-registered on Lite or Pro with a simple quarterly cash BAS, AI BAS flags missing documents and GST codes as you go, then gives your BAS agent a decision report and CSV. [S7][S8] You or your agent still lodge. [S8]
- **Receipts on the road.** Staff photograph receipts in MYOB Assist, and MYOB pre-fills the bill or expense for you to check. [S18][S19][S20] Give them the Field role so they don't see your accounts. [S18][S31]
- **A monthly check-in with your accountant.** If you're in the AI Business Insights beta, its plain-English commentary and charts give you something to talk through. [S11][S15][S16]

**For accounting practices and bookkeepers**

- **One workflow across messy client ledgers.** Practice Compliance AI mapping standardises client data to one chart of accounts (Core and Pro Compliance). [S60]
- **Reviewing a client's AI BAS.** Advisers use their normal MYOB access to review and adjust, and get the BAS decision report and CSV. [S7][S8]
- **Seeing a client's AI insights.** The Accountant/Bookkeeper role can view AI Business Insights. [S16]
- **Asking Claude about a client file.** Only after the client's Owner user has allowed it in My Account. [S4] MYOB's wording suggests any user with file access, including an adviser, could then connect their own Claude or ChatGPT account. That's our reading; the page doesn't mention advisers by name. [S4]

**For larger businesses on MYOB Acumatica**

- **Supplier bills.** AP Bill Entry reads supplier bills and checks them against supplier records. [S56]
- **Spotting odd journal entries.** Anomaly Detection rates journal entries Normal, Medium or Significant for review. [S59]

## What to watch for

**Your data leaves MYOB when you use Claude or ChatGPT.**
- MYOB's promise that data is processed in Australia and not used for training is made for Ask Iris. [S3] The connector page says instead that your conversation is subject to Claude's or ChatGPT's own privacy settings and terms. [S4]
- Turn off model training: **Help improve our AI models** in Claude, **Improve the model for everyone** in ChatGPT. [S4][S36]
- Check memory settings in both, because memory can hold older figures. [S4]
- In ChatGPT, select the MYOB plugin each time, or you may get an answer from the web. [S4]

**Who can connect a file.**
- Once the Owner allows it, any user with access to the file and their own AI account can connect. [S4]
- The connector reaches whatever that user's MYOB permissions allow. [S4] MYOB's "Read only" access level still lets a user read, so it won't stop the connector reading. (Our inference from how MYOB describes access levels.) [S31]
- For practices: if an adviser connects a client's file, the adviser's own Claude or ChatGPT settings govern that client's figures. (Our inference.) [S4]
- MYOB doesn't document how the Owner withdraws AI access in My Account. [S4]

**Check the answers.**
- MYOB says you can ask the connector about cash position [S4], but none of the seven tools on Anthropic's listing is named for bank balances. [S6] We couldn't find how cash position is worked out, so check it against MYOB.
- Smart Reconciliation and category predictions can be wrong, and some predictions come from other businesses' coding. [S12][S13] Review the Matched tab before you finalise. [S12]
- AI BAS "may omit or generate incorrect information". [S8] MYOB isn't a registered tax agent, so you stay responsible for what you lodge. [S8]
- MYOB's terms say you must verify AI output before relying on it, and that MYOB makes no guarantee about its accuracy. [S27]

**Things that happen automatically.**
- Smart Invoice Reminders email every customer with reminders switched on, on schedule, once you save the settings. [S14] Check your list before turning it on.
- Automatching may already be on in your bank rules. [S13]

**Cost surprises.**
- AI BAS is a 12-month commitment with 10 days' notice to cancel, and you pay out the term. [S8] Beta users get it free only "for a limited time". [S8]
- From year two, AI BAS pricing moves with your BAS transaction count. [S7]
- Building your own AI link through the API starts at $110 a month for Developer Program membership. [S48]

**What MYOB's terms let it do with your data.**
- You give MYOB a licence to use your data "to develop and improve our products and services". [S27]
- You also give MYOB a permanent licence to use anonymised or aggregated data derived from your data. [S27]
- MYOB's privacy policy doesn't mention AI. [S28]

**Unofficial connections.**
- If someone offers a third-party MCP server or automation for MYOB, MYOB's developer terms bar developers from running MCP servers that wrap MYOB's API for outside AI agents. [S47] Ask the vendor how it complies before you connect your books, and ask MYOB.
- Marketplace apps are third-party products, and installing one lets it access your data. [S27][S51]

**Protect the MYOB login.**
- Connecting Claude or ChatGPT uses your MYOB username and password. [S4]
- MYOB recommends passkeys, or an authenticator app with SMS as backup, and says "Email 2FA is not recommended and will be phased out in 2027." [S30]

**Larger businesses.**
- In MYOB Acumatica, journal entry anomaly detection sends the inquiry data to an external AI service. [S59]

## Announced changes

| When | What | Source |
|---|---|---|
| 1 November 2026 | Prices change for MYOB Business Payroll Only and the per-user Payroll premium feature (new prices not shown). | [S2] |
| 2027 | Email two-factor authentication to be phased out. | [S30] |
| "For a limited time" (no date) | AI BAS beta users keep free access, then must add AI BAS as a paid Premium Feature. | [S8] |
| Through 2026 | AI BAS support to expand; employing businesses joined the beta from September 2026. | [S7][S10] |
| From August 2026 | Phased rollout of the MYOB Connector in Claude and ChatGPT. "Further integration capabilities are expected to follow". | [S5] |
| Later in 2026 | First jointly built MYOB and Microsoft customer features. | [S40] |
| No date | Wider access to AI Business Insights planned. | [S15] |
| No date | "Agentic AI capabilities" to come to MYOB Assist over time. | [S17] |
| May 2026, then later in 2026 | MYOB Acumatica AI Studio in early access from May, wider availability later in the year. | [S57] |
| Version 2026.1.1 | Acumatica's AI Studio renamed AI Automation; anomaly detection renamed and moved out of experimental features; the old GL Anomaly Detection is deprecated. | [S58][S59] |
| Already happened, plus "the near future" | AccountRight offline files phased out. PC Edition only shows online files from 17 June (year not stated). The temporary Server Edition will stop working "in the near future". | [S62][S63] |
| Already happened | MYOB Invoice and MYOB Capture apps replaced by MYOB Assist. | [S17][S18] |
| 12 March 2026 | New Developer Program terms, with AI and MCP limits. Earlier members bound from 13 April 2026. | [S47] |
| Pilot, no date | MYOB and Mastercard's agentic payments pilot "remains in testing". | [S64] |

## What we couldn't establish

- **OpenAI's side of the ChatGPT connection.** OpenAI doesn't list which ChatGPT plans can install the MYOB plugin, or the plugin's individual tools. [S66][S67] We found no retention period for data the plugin fetches.
- **Where Claude and ChatGPT process data for Australian users.** The pages we read don't say.
- **Switching MYOB's own AI off.** We found no documentation on whether Ask Iris, category suggestions or AI Business Insights can be turned off, or by whom.
- **Which AI models power Iris.** MYOB names Anthropic, AWS and Microsoft for Acumatica [S56], but no provider for MYOB Business features. Only Ask Iris has a stated processing location and training promise. [S3]
- **How long AI data is kept.** We found no retention periods for Ask Iris chats or AI BAS decisions. The connector page doesn't give one for connector activity either.
- **Revoking access from MYOB's side.** How the Owner withdraws AI file access in My Account, and what happens to a connection when a user loses file access.
- **Other AI tools on MYOB's MCP server.** Whether anything besides Claude and ChatGPT can use mcp.myob.com.
- **New Zealand customers and the connector.** MYOB's Australian help page doesn't say whether New Zealand subscriptions can use the MYOB Connector. [S4] OpenAI's listing for the ChatGPT plugin asks for a MYOB Business subscription in Australia or New Zealand. [S66] We couldn't confirm the same for Claude.
- **How "cash position" is answered** through the connector.
- **The API scope deadline.** An MYOB community forum post says the old "CompanyFile" API scope was removed on 1 September 2026, forcing integrations to move to granular scopes. MYOB's developer pages we could load don't state it, and MYOB's API support site blocked our reader. If an older integration stopped working in September, this is the likely lead, but it isn't confirmed here.
- **API rate limits.** Not on the public pages we read. [S44][S47]
- **Make.com.** Whether Make lists a MYOB app.
- **Microsoft's Copilot connector gallery.** We checked Microsoft's Power Platform connector list [S41] but not the Microsoft 365 Copilot connector gallery.
- **The full marketplace.** We checked a handful of the 350+ listed apps for AI features. [S51] The marketplace pages we loaded had no AI category or search filter we could use.
- **New Zealand data in predictions.** Whether "other MYOB businesses" in Smart Reconciliation includes New Zealand businesses.
- **AccountRight Premier and Solo AI.** Premier isn't in the pricing page's AI comparison [S2], and Solo's only AI item, Category Suggestions, has no Solo help article. [S2][S26]
- **Prices we didn't capture.** Practice Compliance, MYOB Acumatica AI features, and whether plan prices include GST.
- **Our search allowance ran out** near the end of this research, so we couldn't run a final sweep for Google or Microsoft announcements about MYOB, or for an official MYOB page on the API scope deadline.

## Sources

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | MYOB AI Accounting Software (Iris by MYOB) | MYOB | https://www.myob.com/au/ai-accounting | No date shown | 15 Oct 2026 |
| S2 | Plans and pricing | MYOB | https://www.myob.com/au/pricing | No date shown | 15 Oct 2026 |
| S3 | Understand your business with Ask Iris (Beta) | MYOB | https://www.myob.com/au/support/myob-business/get-help-support/ai-assistant | No date shown | 15 Oct 2026 |
| S4 | Connecting Claude or ChatGPT to MYOB | MYOB | https://www.myob.com/au/support/myob-business/product-account/connecting-myob | No date shown | 15 Oct 2026 |
| S5 | MYOB brings SME financial intelligence into Claude and ChatGPT | MYOB | https://www.myob.com/au/press-releases/myob-brings-sme-financial-intelligence-into-chatgpt-and-claude | 17 August 2026 | 15 Oct 2026 |
| S6 | MYOB (connector listing) | Anthropic | https://claude.com/connectors/myob | "Added July 2026" | 15 Oct 2026 |
| S7 | AI BAS | MYOB | https://www.myob.com/au/products/ai-bas-software | No date shown | 15 Oct 2026 |
| S8 | Get BAS-ready faster with AI BAS | MYOB | https://www.myob.com/au/support/myob-business/end-of-period/month-end-procedures/ai-bas | No date shown | 15 Oct 2026 |
| S9 | MYOB Premium Features | MYOB | https://www.myob.com/au/support/billing-and-account/myob-premium-features | No date shown | 15 Oct 2026 |
| S10 | MYOB expands AI BAS beta to employing businesses | MYOB | https://www.myob.com/au/press-releases/myob-expands-ai-bas-beta-to-employing-businesses | 15 September 2026 | 15 Oct 2026 |
| S11 | MYOB rolls out suite of AI products to power up SME productivity | MYOB | https://www.myob.com/au/press-releases/myob-rolls-out-suite-of-ai-products-to-power-up-sme-productivity | 2 March 2026 | 15 Oct 2026 |
| S12 | Review as you go for easier reconciliation | MYOB | https://www.myob.com/au/support/myob-business/banking/smart-reconciliation | No date shown | 15 Oct 2026 |
| S13 | Matching transactions with automatches and suggestions | MYOB | https://www.myob.com/au/support/myob-business/banking/automatches-and-suggestions | No date shown | 15 Oct 2026 |
| S14 | Send Smart Invoice Reminders | MYOB | https://www.myob.com/au/support/myob-business/sales/online-invoicing/setting-up-invoice-reminders | No date shown | 15 Oct 2026 |
| S15 | AI Business Insights | MYOB | https://www.myob.com/au/ai-accounting/business-insights | No date shown | 15 Oct 2026 |
| S16 | Business Insights, including AI Business Insights (Beta) | MYOB | https://www.myob.com/au/support/myob-business/accounting/financial-control/reviewing-financial-information/business-insights-overview | No date shown | 15 Oct 2026 |
| S17 | MYOB Assist | MYOB | https://www.myob.com/au/myob-apps/assist | No date shown | 15 Oct 2026 |
| S18 | Getting started with the MYOB Assist app | MYOB | https://www.myob.com/au/support/myobapp/getting-started-with-myob-assist | No date shown | 15 Oct 2026 |
| S19 | Capture an expense | MYOB | https://www.myob.com/au/support/myobapp/apphelp/capture | No date shown | 15 Oct 2026 |
| S20 | Working with uploaded documents | MYOB | https://www.myob.com/au/support/myob-business/purchases/working-with-in-tray-documents | No date shown | 15 Oct 2026 |
| S21 | What's new and what's next (product roadmap) | MYOB | https://www.myob.com/au/myob-product-roadmap | No date shown | 15 Oct 2026 |
| S22 | MYOB Business Lite | MYOB | https://www.myob.com/au/products/myob-business/lite | No date shown | 15 Oct 2026 |
| S23 | MYOB Business Pro | MYOB | https://www.myob.com/au/products/myob-business/pro | No date shown | 15 Oct 2026 |
| S24 | MYOB Business AccountRight Plus | MYOB | https://www.myob.com/au/products/myob-business/accountright-plus | No date shown | 15 Oct 2026 |
| S25 | MYOB Business AccountRight Premier | MYOB | https://www.myob.com/au/products/myob-business/accountright-premier | No date shown | 15 Oct 2026 |
| S26 | Solo by MYOB (product page) and Solo support home | MYOB | https://www.myob.com/au/products/solo and https://www.myob.com/au/support/solo | No date shown | 15 Oct 2026 |
| S27 | MYOB Business Terms of Use | MYOB | https://www.myob.com/au/legal/myob-business-terms | "Last updated: June 2026" | 15 Oct 2026 |
| S28 | Privacy Policy | MYOB | https://www.myob.com/au/legal/privacy-policy | "August 2026" | 15 Oct 2026 |
| S29 | Security Practices (Trust Centre) | MYOB | https://www.myob.com/au/legal/security-practices | No date shown | 15 Oct 2026 |
| S30 | Security at MYOB | MYOB | https://www.myob.com/au/support/security | No date shown | 15 Oct 2026 |
| S31 | Manage users (user access) | MYOB | https://www.myob.com/au/support/myob-business/business-settings/manage-users | No date shown | 15 Oct 2026 |
| S32 | Exporting reports | MYOB | https://www.myob.com/au/support/myob-business/reporting/exporting-reports | No date shown | 15 Oct 2026 |
| S33 | Use connectors to extend Claude's capabilities | Anthropic | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated over 2 weeks ago" (as at 15 Oct 2026) | 15 Oct 2026 |
| S34 | Connectors directory | Anthropic | https://claude.com/docs/connectors/directory | No date shown | 15 Oct 2026 |
| S35 | Connector verification | Anthropic | https://claude.com/docs/connectors/verification | No date shown | 15 Oct 2026 |
| S36 | How do I change my model improvement privacy settings? | Anthropic | https://privacy.claude.com/en/articles/12109829-how-do-i-change-my-model-improvement-privacy-settings | 3 August 2026 | 15 Oct 2026 |
| S37 | How long do you store my data? | Anthropic | https://privacy.claude.com/en/articles/10023548-how-long-do-you-store-my-data | 1 July 2026 | 15 Oct 2026 |
| S38 | Upload files to Claude | Anthropic | https://support.claude.com/en/articles/8241126-what-kinds-of-documents-can-i-upload-to-claude-ai | 23 July 2026 | 15 Oct 2026 |
| S39 | Plugins (ChatGPT Learn) | OpenAI | https://learn.chatgpt.com/docs/plugins | No date shown | 15 Oct 2026 |
| S40 | MYOB and Microsoft sign five-year strategic partnership | Microsoft (Source Asia) | https://news.microsoft.com/source/asia/2026/04/08/myob-and-microsoft-sign-five-year-strategic-partnership/ | 8 April 2026 | 15 Oct 2026 |
| S41 | List of all connectors (Azure Logic Apps, Power Automate, Power Apps) | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/connector-reference/ | 2 October 2026 (page metadata) | 15 Oct 2026 |
| S42 | Get started with Copilot in Excel | Microsoft Support | https://support.microsoft.com/en-us/office/get-started-with-copilot-in-excel-d7110502-0334-4b4f-a175-a73abdfc118a | No date shown | 15 Oct 2026 |
| S43 | Upload & analyze files in Gemini Apps | Google | https://support.google.com/gemini/answer/14903178 | No date shown | 15 Oct 2026 |
| S44 | MYOB Business API: Getting Started | MYOB Developer | https://developer.myob.com/api/myob-business-api/api-overview/getting-started/ | April 2023 | 15 Oct 2026 |
| S45 | MYOB Business API: Authentication | MYOB Developer | https://developer.myob.com/api/myob-business-api/api-overview/authentication/ | "Date Updated: Mar 2025" | 15 Oct 2026 |
| S46 | Granular Data Scopes | MYOB Developer | https://developer.myob.com/api/myob-business-api/api-overview/granular_data_scopes/ | Nov 2025 | 15 Oct 2026 |
| S47 | MYOB Developer Program and Platform Terms | MYOB Developer | https://developer.myob.com/program/terms-conditions/business-api-tandcs/ | "Last Updated 12 March 2026" | 15 Oct 2026 |
| S48 | What is the Developer Program | MYOB Developer | https://developer.myob.com/what-is-the-developer-program/ | No date shown | 15 Oct 2026 |
| S49 | MYOB Developer Security Requirements | MYOB Developer | https://developer.myob.com/program/security-requirements/ | No date shown | 15 Oct 2026 |
| S50 | MYOB App Marketplace (listing your app) | MYOB Developer | https://developer.myob.com/program/add-on-listing-on-myob-com/ | No date shown | 15 Oct 2026 |
| S51 | MYOB App Marketplace | MYOB | https://www.myob.com/au/apps | No date shown | 15 Oct 2026 |
| S52 | Dext (marketplace listing) | MYOB | https://www.myob.com/au/apps/dext | No date shown | 15 Oct 2026 |
| S53 | Accounts Payable – AP Automation Solution for MYOB (marketplace listing) | MYOB | https://www.myob.com/au/apps/accounts-payable-solution-for-myob | No date shown | 15 Oct 2026 |
| S54 | Lightyear (marketplace listing) | MYOB | https://www.myob.com/au/apps/lightyear | No date shown | 15 Oct 2026 |
| S55 | MYOB integrations | Zapier | https://zapier.com/apps/myob/integrations | No date shown. Returned "not found" when loaded directly; wording read from the search index | 15 Oct 2026 |
| S56 | AI tools for MYOB Acumatica | MYOB | https://www.myob.com/au/erp-software/solutions/ai-erp | No date shown | 15 Oct 2026 |
| S57 | MYOB Acumatica launches new AI Studio in collaboration with AWS | MYOB | https://www.myob.com/au/press-releases/myob-acumatica-launches-new-ai-studio-in-collaboration-with-aws | 28 April 2026 | 15 Oct 2026 |
| S58 | AI Studio: Renaming of AI Features (2026 R1 release notes) | MYOB | https://help.myob.com.au/advanced/Docs/Published/ReleaseNotes/RN_2026_R1_AI_Studio_Renaming_Features.html | Version 2026.1.1; no date shown | 15 Oct 2026 |
| S59 | Finance: Anomaly Detection for Journal Entries (2026 R1 release notes) | MYOB | https://help.myob.com.au/advanced/Docs/Published/ReleaseNotes/RN_2026_R1_Finance_AnomalyDetection_GI.html | Version 2026.1.1; no date shown | 15 Oct 2026 |
| S60 | Practice Compliance | MYOB | https://www.myob.com/au/accountants-and-bookkeepers/products/practice-compliance | No date shown | 15 Oct 2026 |
| S61 | Accountants and bookkeepers | MYOB | https://www.myob.com/au/accountants-and-bookkeepers | No date shown | 15 Oct 2026 |
| S62 | Move your company file online to keep working | MYOB | https://www.myob.com/au/support/myob-business/product-account/working-online/put-your-company-file-online | No date shown | 15 Oct 2026 |
| S63 | MYOB Support (home) | MYOB | https://www.myob.com/au/support | No date shown | 15 Oct 2026 |
| S64 | MYOB and Mastercard pilot agentic payments for SMEs | MYOB | https://www.myob.com/au/press-releases/myob-and-mastercard-pilot-agentic-payments-for-smes | 15 June 2026 | 15 Oct 2026 |
| S65 | Sale Invoice endpoint (MYOB Business API v2) | MYOB Developer | https://developer.myob.com/api/myob-business-api/v2/sale/invoice/ | Last updated January 2022 | 15 Oct 2026 |
| S66 | MYOB (ChatGPT plugin listing) | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_6a698d6712708191b639ff0f4d92446b | No date shown; version 1.0.0 | 15 Oct 2026 |
| S67 | Plugins in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001256-plugins-in-chatgpt | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S68 | Admin controls, security, and compliance for plugins and apps | OpenAI Help Center | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S69 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S70 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S71 | ChatGPT release notes | OpenAI Help Center | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
