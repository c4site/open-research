# Xero: the AI inside it, and the AI that connects to it

Researched 18 November 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Xero's built-in AI is called JAX. Xero uses that one name for a chat assistant you open from the navigation bar and for automation that runs in the background, such as bank matching. [S2] [S4]
- JAX chat comes with every Xero subscription at no extra charge for now. It can only see what your own Xero login can see. [S2]
- Automatic bank reconciliation by JAX is included from the Grow plan up. On Ignite it's a paid add-on called AI Automate. [S9]
- Smart Document Capture reads the receipts and invoices you send into Xero. You check the details before Xero creates anything. [S10]
- Four outside AI assistants now have official Xero connections: Claude, ChatGPT, Microsoft Copilot and Google Gemini. [S6] [S34] [S7] [S36]
- The Claude, ChatGPT and Copilot connections are read-only. They answer from live Xero data and link you back to Xero to make any change. [S6] [S65] [S7]
- The Gemini connection went live in October 2026. Xero's launch release said it could issue invoices after you confirm, but Xero's newer help article says Gemini can't change anything in Xero. [S36] [S91] [S90]
- Since October 2026 you can connect more than one Xero organisation to each of these assistants. Name the organisation in your question. [S91] [S90]
- Xero says data passed to Claude, Copilot and Gemini through these connections is used only for your session and isn't used to train their models. [S24] [S26] [S36]
- For anything else, Xero offers a developer route: its MCP server plus a custom connection at $10 a month. Xero stops selling new custom connections on 1 December 2026. [S52] [S51] [S54]
- Xero reports about 96% accuracy on the bank lines JAX reconciles by itself, so someone still needs to check the results. [S8]

## The tool, and the plans that matter

Xero is online accounting software. Each set of books is called an "organisation". In Australia it's sold as monthly plans priced in AUD, including GST. [S1] [S20]

These are the regular monthly prices on Xero's Australian pricing page as read on 18 November 2026. New Australian customers are offered 80% off for the first three months with a promo code. [S1]

| Plan | Price a month (AUD, incl. GST) | AI-related inclusions | Limits worth knowing |
|---|---|---|---|
| Ignite | $37 | "Smart document capture basic extraction". JAX bank matching isn't included; it's sold as the AI Automate add-on (the pricing page lists auto-reconcile on Ignite as "Optional" at $8 a month). | 20 invoices, 5 bills, payroll for 1 person, 30-day cash flow forecast |
| Grow | $78 | Smart document capture basic extraction. JAX categorises and matches high-confidence bank transactions. | Payroll for 2, 60-day forecast |
| Comprehensive | $107 | Full Smart document capture. JAX bank matching. "Budget with smart suggestions" (3 budgets). | Payroll for 5, 90-day forecast, multiple currencies |
| Ultimate 10 / 20 / 50 / 100 | $143 / $180 / $250 / $300 | As Comprehensive, plus "Analyse KPIs and ratios" and "Benchmark against the industry". | Payroll for 10 / 20 / 50 / 100, 180-day forecast |
| Ultra | $500 | As Ultimate, plus Syft Advanced for multi-entity consolidation, forecasting and budgeting. | Payroll for 10, priority support, targeted data restore |

Sources for the table: [S1] [S9] [S13] [S28]

- The Ignite invoice limit counts invoices that connected apps create too: "Transactions initiated by app partners may automatically contribute to your invoice limit." [S1]
- Ultra launched in Australia on 7 July 2026 at $500 a month including GST. [S28]
- Ultra's Syft Advanced tools use a separate Syft login. [S12]

**Tools for accountants and bookkeepers**

- **Xero Partner Hub** is free with the Xero partner program. Xero says it brings together work that used to be split across Xero HQ, Xero Practice Manager, Tax and Workpapers. [S14]
- Practices that used only Xero HQ were scheduled to move to Partner Hub in early 2026. [S40]
- Xero's Australian release notes say Partner Hub went live to all practices in September 2026. [S91]
- Xero's help centre (Xero Central) still uses "Xero HQ" in some article names, so expect to see both names. [S42]
- Partner Hub includes JAX chat, which Xero labels as beta. [S14]
- **Tax & Workpapers** is an optional Partner Hub tier. It's free for Bronze, Silver, Gold and Platinum partners. Otherwise it costs $71.50 to $163.90 a month. [S14]
- On the Xero Tax page, that's $71.50 a month for one user, $108.90 for up to three, and $163.90 for four or more, including GST. Xero Sign by Adobe Acrobat Sign costs extra. [S15]
- **Practice Management** (jobs, time and billing) is free for Silver partners and above. It's $163.90 a month for Bronze partners and new practices. [S14]
- **Xero Tax** prefills activity statements from ATO data. The Xero Tax page doesn't describe this or anything else as AI. [S15]
- **Xero Practice Manager**: we found no AI features described in the sources we could read. The Partner Hub page describes Practice Management as jobs, time and billing. [S14]
- **Hubdoc** is still sold as a separate document capture product, with a free trial and a Xero integration. Its home page describes automatic extraction of details such as supplier names and due dates, but doesn't use the word AI. [S59]
- Xero Central has Hubdoc articles updated as recently as November 2026, including one on turning off Hubdoc's data extraction. [S42]

## AI built in

### JAX chat ("JAX, your AI finance partner")

**What it does**

- Answers questions about your own figures in plain English, with charts and tables. [S2]
- Answers "how do I do this in Xero" questions from Xero's help content. [S2]
- Does general business research. Xero's examples include van lease rates in Melbourne and the minimum wage in Victoria. [S2]
- Coaches you through conversations, such as negotiating payment terms with a customer. [S2]
- Handles admin such as creating invoices and quotes. Xero's example is an invoice for a contact based on the last quote you sent them. [S2]
- Xero Central says JAX can also approve and send invoices and quotes, and answer questions about files you upload to it. It can only do what your own Xero role allows. [S76]
- Xero calls JAX a "superagent" that coordinates several AI agents behind the scenes. [S21]
- Xero says a control system called JAX Assure reduces made-up answers compared with tools that rely only on large language models. [S21]
- Its business research uses web research Xero developed with OpenAI. [S21]
- An image on Xero's AI philosophy page shows JAX asking for confirmation before it sends an invoice. [S16]
- Xero calls its approach "Accountable Intelligence". JAX shows its work with visible audit trails, and people "remain fully accountable for the final outcomes". [S31]

**Where to find it**

- Open JAX from the navigation bar inside Xero and ask a question. [S2]
- Xero Central says you can also use JAX in the Xero Accounting app. You can start a new chat to keep topics apart and reopen past chats from your chat history. [S45]

**Plans and cost**

- Xero says JAX chat is available to all Xero subscribers and users. [S2]
- Xero Central is narrower. It says JAX is for the subscriber and users with the administrator or standard user role, and it labels JAX a beta. [S76]
- There's currently "no additional charge to Xero subscribers". Xero reserves the right to change the terms, including pricing. [S2]

**On by default, and who controls it**

- JAX chat is there for everyone, but it only does something when a person opens it and asks a question. [S2]
- To stop particular people using it, Xero says to change their Xero roles and permissions. [S2]
- JAX chat follows the same access rules as the rest of Xero, so people only see data they're already allowed to see. [S2]
- We didn't find a single switch that turns JAX chat off for a whole organisation. The FAQ only describes leaving it unopened or changing roles. [S2]

**Your data**

- Xero says "JAX chat doesn't use your data to train the LLMs it uses". [S2]
- Xero names AWS, Microsoft Azure, GCP and OpenAI as its large language model providers. Xero says they process what you type, which may include personal data, and don't keep it to train their models. [S2]
- Xero's sub-processor list names Anthropic and OpenAI for "Conversational artificial intelligence services", both located in the United States. [S18]
- Xero's March 2026 Anthropic announcement says Claude's reasoning powers parts of JAX's work. The JAX FAQ doesn't name Anthropic. [S23] [S2]
- Xero's AI page says JAX is "Grounded in 20 years of Australian small business data". It doesn't explain how that sits with the no-training statement for JAX chat. [S4] [S2]
- Xero's privacy notice says data may be processed in countries including Australia, New Zealand and the United States. [S19]

**In Australia**

- The Australian JAX page says JAX chat is available to all subscribers and users. [S2]
- In March 2025 Xero said JAX could also be reached by SMS in Australia, and by WhatsApp and email forwarding. The current Australian JAX page mentions only the navigation bar, so we couldn't confirm those channels still work. [S22] [S2]

### Automatic bank reconciliation, powered by JAX

**What it does**

- JAX categorises and matches new bank statement lines. It reconciles a line by itself only when it's highly confident. [S9]
- When it isn't confident, it suggests a match and leaves the line for you to reconcile. [S9]
- Every auto-reconciled line shows one of four methods. "Match" means it matched an existing Xero document. "Rule" means one of your bank rules applied. [S8]
- "Memory" means it followed how you reconciled similar lines before. "Prediction" means it followed how other Xero users reconciled similar lines. [S8]
- Xero says it auto-reconciles over 60% of the lines it sees, with about 96% accuracy on those. Xero measures accuracy as the share of lines users didn't correct, averaged over April to July 2026. [S8]
- Xero's AI in accounting page gives the accuracy as 97%, without saying how that's measured. [S4]
- Since October 2026 it can suggest a match for a Stripe payment that covers several invoices, and reconcile it automatically. [S91]
- Once it's on, JAX looks at new statement lines as they arrive. It doesn't go back over old ones. [S44]

**Where to find it**

- Subscribers and advisers turn it on for each bank account from that account's settings. [S8]
- Xero Central's Australian steps: in the **Accounting** menu select **Bank accounts**, click the account, select the **Reconcile** tab and click **Auto-reconcile**. Under **Auto-reconcile settings**, tick **Turn on Auto Bank Reconciliation**, then click **Save**. [S44]
- To turn it off, clear that checkbox and click **Save**. To change every bank account at once, click the arrow next to **Save** and choose **Save for all accounts**. [S44]
- You review results on the **Reconciled** page. You can change an account code or tax rate in the row without starting over. [S9] [S32]
- **Remove & redo** reverses a line. **Settings history** shows the latest change to the setting, who made it and when. [S8]
- Xero keeps an audit trail in the History and Notes report. The GST Audit report shows the transactions behind your activity statement. [S9]
- Xero suggests starting with one account that has established rules and consistent transactions. [S8]

**Plans and cost**

- Xero's Australian page says: "Available on Grow plan and above. Optional add on for the Ignite plan." [S9]
- The Ignite add-on is called AI Automate. Xero Central says it costs a fixed monthly price. [S9] [S44]
- Xero's Australian pricing page lists auto-reconcile on Ignite as "Optional" at "$8 per month". It doesn't use the name AI Automate or say whether GST is included in that add-on. [S1]
- The pricing page's comparison table also lists auto-reconcile on Ultra. [S1]
- Xero's Australian campaign page for this feature has some contradictory lines, including US plan names. Check your own subscription settings before relying on it. [S8]

**On by default, and who controls it**

- Xero describes it as something you turn on account by account. We found no statement that it's on by default. [S8] [S9]
- Xero Central's Australian article says you must be the subscriber or have the administrator user role to turn it on or off, and only one person per organisation needs to do it. Xero's campaign page says advisers instead. [S44] [S8]

**Your data**

- Xero says it doesn't use customer data to train its Auto Bank Reconciliation models unless the data is anonymised or Xero has permission. [S8]
- Xero also says it may use data about how you use the feature to improve its products. [S8]
- The "Prediction" method draws on how other Xero users reconciled similar transactions. [S8]

**In Australia**

- Xero's Australian pages describe the feature and its plan inclusions. [S9] [S1]
- Xero Central has an Australia and New Zealand version of the how-to article updated 3 November 2026, and an "About" article updated 7 October 2026. [S42]

### Smart Document Capture (in Documents, formerly Files)

**What it does**

- Reads receipts, invoices and rental statements, then extracts the details into Xero. [S10]
- You double-check and approve the details before Xero creates a record. [S10]
- It compares extracted data with your bank records and highlights likely matches for you to accept or reject. [S10]
- It warns you if you upload the same document twice. [S10]
- On 18 September 2026 Xero renamed Files to Documents and said Smart Document Capture is now "powered by JAX". Xero says it learns patterns over time. [S35]
- From October 2026, bills you email to your Xero organisation get more details filled in on the draft bill. [S91]

**Where to find it**

- Documents now sits in the **Accounting** menu. It moved there from the organisation name menu. [S35]
- To get documents in, photograph them with the Xero Accounting app or send them to your Xero email address. You can also drag and drop files in the browser. [S10]
- Auto-matching can be turned on or off at any time. [S35]

**Plans and cost**

- Ignite and Grow include "Smart document capture basic extraction". Comprehensive and above include "Smart document capture". [S1]
- The pages we read don't explain what "basic extraction" leaves out. Xero's product page says the feature comes at no extra charge on all small business plans. [S1] [S10]

**On by default, and who controls it**

- The pages we read don't say whether it's on by default. [S10] [S35]
- User permissions can limit a team member to uploading and viewing only, so they can't see other financial data. [S35]

**Your data**

- The pages we read don't say whether your uploaded documents are used to train Xero's models. [S10] [S35]
- Xero says capture is highly accurate when documents are clear and in standard formats, and that you should check the details before records are created. [S10]

**In Australia**

- Xero's Australian product page and pricing page both describe it. [S10] [S1]
- Xero first rolled it out to UK customers in March 2026, with other markets to follow. [S37]
- Xero plans tax number validation for the UK and Australia. [S35]

### Analytics, forecasts and benchmarks (Analytics powered by Syft)

**What it does**

- Dashboards and a cash flow manager with "what if" scenarios. [S38]
- AI-generated suggestions and summaries that explain your numbers. [S38]
- Business health scorecards that combine performance metrics with outside data such as website traffic. [S38]
- Industry Benchmarks, launched 29 June 2026, compare your ratios with businesses in your industry and country. Each ratio is labelled leading, lagging or in line, with AI-generated suggestions. [S39]
- Cash flow forecasts run 30, 60, 90 or 180 days ahead depending on your plan. [S1]
- Xero's AI page groups cash flow answers and scenario modelling under a heading called "AI Insights". [S4]

**Where to find it**

- The pages we read don't give a menu path for analytics inside Xero. [S11] [S38]

**Plans and cost**

- Xero says core analytics are included in all business plans at no cost. [S11]
- "Analyse KPIs and ratios" and "Benchmark against the industry" are on Ultimate and Ultra. [S1]
- Syft Advanced, with consolidation and advanced forecasting and budgeting, comes only with Ultra at $500 a month. [S1] [S28]

**On by default, and who controls it**

- Not stated in the pages we read. [S11] [S38]

**Your data**

- Industry Benchmarks are built from "anonymized and aggregated data" from Xero small business customers worldwide. [S39]
- Xero's terms allow it to use anonymised statistical data from your use of Xero for its own purposes. [S20]

**In Australia**

- Xero's Australian analytics and pricing pages describe these features. [S11] [S1]
- Xero Central's Australian "Analytics pricing plans" article sets out which analytics features each plan gets. Its cash flow table gives Grow a 30-day forecast, while Xero's pricing page says 60 days. [S82] [S1]
- Xero Central's short-term cash flow article says cash predictions need at least three months of reconciled transactions. [S83]

### Budget with smart suggestions

- **What it does:** Xero lists budget suggestions among JAX's capabilities. [S3]
- Xero's 11 November 2026 blog on its new Budgets says "Smart suggestions guide you through common changes", such as boosting sales or growing your team. It doesn't mention AI or JAX, or say how the suggestions are made. [S92]
- **Where to find it:** Xero's blog says to go to **Reporting** to open New Budgets, then select **Start planning** at the top left of a budget. Xero Central's "About Budgets in Early access" says Xero creates a first budget from last year's actuals. [S92] [S77]
- **Plans and cost:** Comprehensive (3 budgets) and above. [S1]
- **On by default, and who controls it:** Not stated. [S1] [S3]
- **Your data:** No feature-specific statement found. [S1] [S3]
- **In Australia:** Listed on the Australian pricing page. [S1]

### JAX in Xero Partner Hub (beta, for accountants and bookkeepers)

- **What it does:** Ask JAX for insights across your clients, or for a summary of one client before a meeting. It also gives quick answers on the Partner Hub homepage. [S14]
- Client insights help you spot which Xero clients might benefit from support or advice. [S14]
- **Where to find it:** The Partner Hub homepage. [S14]
- **Plans and cost:** Partner Hub is free with the Xero partner program. [S14]
- **On by default, and who controls it:** Xero says "JAX chat is currently in beta". [S14] Xero's terms say beta services are used at your own risk. [S20]
- **Your data:** The Partner Hub page has no specific data statement. [S14]
- **In Australia:** Described on the Australian Partner Hub page. Xero Central's "About JAX for accountants and bookkeepers (beta)" was updated 8 September 2026. [S14] [S42]

### XeroForce (early access)

- **What it does:** Lets you build custom AI agents by describing them in plain English. Agents can link Xero with other apps. They can run on a schedule or wait for an event such as an email reply. [S25]
- Xero says every agent action is logged with an audit trail. [S25]
- **Where to find it:** In May 2026 it was an invite-only alpha. By August 2026 Xero called it early access, with general release "later this year". [S25] [S41]
- On 12 November 2026 Xero still described XeroForce as in beta. [S93]
- **Plans and cost:** Not stated. [S25]
- **On by default, and who controls it:** Not stated. [S25]
- **Your data:** The announcement has no data-use statement. [S25]
- **In Australia:** The XeroForce announcement doesn't say. Xforce, a beta service where Xero engineers help accounting firms build AI workflows with XeroForce, has one Australian design partner, Liston Newton Advisory. [S25] [S93]

## Outside AI that connects

A quick translation of the jargon. An **API** is the door Xero opens so other software can read or change your books. **MCP** (Model Context Protocol) is a standard way for an AI assistant to use outside tools. Xero's own FAQ describes it as a way to connect an AI model to an external data source. [S54]

Claude calls its links "connectors". ChatGPT calls them "plugins". Microsoft calls them "agents" and Google calls them "connected apps". In each case you sign in with your Xero login and approve access. [S6] [S61] [S68] [S71] [S72]

### Claude and Xero

**Official?**

- Yes. The "Xero connector in Claude" is made by Xero Limited and listed in Anthropic's connector directory, added April 2026. [S84] [S87]
- Xero announced it as live on 13 May 2026 for users with an active Xero subscription. [S24]
- Xero is also one of the integrations in Anthropic's "Claude for Small Business", announced 15 September 2026. [S62] [S34]

**In one line**

Claude can read your Xero figures and answer questions about them. It can't change anything in Xero. [S84] [S87]

**Before you start**

| You need | Detail |
|---|---|
| A Claude account | Free or paid. Xero says "a Claude account (either free or paid)", and Claude's pricing page lists "Connect your apps and tools" on the Free plan. [S87] [S89] |
| A Xero subscription | An active one. Xero Central says the connector works on any Xero business pricing plan. [S87] [S43] |
| Your own Xero login | The connector follows your Xero permissions, so Claude sees what your login can see. [S87] |
| Cost | Xero says "the Xero connector is free to add". [S87] |
| An admin? | On a personal Claude plan, no. On Team and Enterprise, an Owner adds the connector for the organisation first, then each person connects their own Xero login. [S85] [S86] |
| Where it works | claude.ai and the Claude desktop app. Anthropic's help centre says installing connectors on a phone is in beta. [S86] Once connected, a connector is available on web, desktop and mobile. [S85] |
| Time | Xero says "Connecting takes only a few minutes". We haven't timed our own run. [S87] |

**Which path?**

- **On my own** (a personal Claude plan): follow the seven steps below. [S86]
- **A member of a Team or Enterprise plan:** if you see **Request**, or a note to ask an Owner, where the connect button should be, your organisation hasn't added Xero yet. Ask an Owner. [S85]
- **A Team or Enterprise Owner:** do the owner steps first. They're under the seven steps. [S85] [S86]

**Steps to connect** (Anthropic's connector docs, no date shown; Claude's Xero listing, added April 2026; Xero's Claude page, no date shown; Xero Central, updated 10 November 2026; all read 18 November 2026)

1. In Claude, go to **Customize > Connectors**. In the desktop app, **Customize** is in the sidebar. [S85]
2. Select **Discover**, type "Xero" in **Search connectors**, then select **Xero**. [S85] [S84]
3. Select **Connect to Claude**. Anthropic's docs use that name, and the public listing showed **Add to Claude** on 18 November 2026, so select whichever you see. [S85] [S84]
4. Sign in with your usual Xero login. [S87] [S43]
5. Choose the organisation you want Claude to read. If you have more than one, select each one you want. Then select **Allow**. [S87] [S43]
6. In a new chat, select **+** in the message box, then **Connectors**, and switch Xero on. [S85]
7. Ask a first question. If Claude asks to use a Xero tool, select **Allow once**. [S85] [S87]

For Claude for Small Business (Anthropic's plugin listing, not dated):

1. On the Small Business plugin listing, click **Install in Cowork**. [S63]
2. Connect the Xero connector as above if you haven't already. [S62] [S85]
3. Run a workflow such as **/monday-brief** or **/close-month**. It starts in approval mode, so Claude drafts and stages the work and waits for your OK. [S63]

**Owner steps, on Team and Enterprise**

1. Go to **Organization settings > Connectors**, click **Browse connectors**, select Xero and click **Add to your team**. [S86]
2. From the directory, the button reads **Connect for your team**. To try it on your own first, select the arrow beside it, then **Connect just for me**. [S85]
3. Under **Tool permissions**, choose **Always allow**, **Needs approval** or **Blocked** for each group of tools or for a single tool. Anthropic says these settings apply to everyone in the organisation. [S85] [S86]
4. Tell each person to connect their own Xero login. Nobody gets access automatically. [S86]

**Check it worked**

- Xero shows under **Your connectors** with the status **Connected**. [S85]
- Claude's answer links back to the Xero report, invoice or contact it used. Open one and compare a figure with the same report in Xero. That check is our advice, based on Xero's description of the links. [S87]

**If it doesn't work**

- **You see Request where the connect button should be.** Your organisation hasn't added Xero. Ask an Owner. [S85]
- **The connector's row shows Reconnect.** Claude has lost access to Xero. Select it and sign in again. [S85]
- **You need a different organisation.** Xero Central now says you can connect several organisations. To add one later, disconnect Xero in Claude, connect again and select every organisation you want, including the ones you already use. [S43]
- **Claude answers about the wrong organisation.** Name the organisation in your question. Xero Central says Claude then uses it for the rest of the chat until you name another. Xero's Claude page also says owners "can switch between business entities", and accountants and bookkeepers between clients. [S43] [S87]
- **The figures look out of date.** Xero Central says the visual summaries in an answer carry a time stamp for the data used. Select **Explore Xero Analytics** in the answer, click **Refresh now** in Xero, then ask again. [S43]
- Neither company describes what you see if the Xero sign-in fails, or what happens when your Xero role can't see some reports.

**What it can read**

- Anthropic's listing names 20 tools. [S84]
- Your financial position, cash position, and profit and loss. [S84]
- Your top customers by revenue. [S84]
- Your organisation's details and financial year, and which organisations are connected. [S84]
- Aged receivables (who owes you) and aged payables (who you owe). [S84]
- Invoices, an invoice summary, bills, and repeating invoices and bills. [S84]
- Contacts, tracking categories, purchase orders and the chart of accounts. [S84]
- Bank account transactions. [S84]
- A "1099 report summary". A 1099 is a US tax form, which suggests the tool set isn't tailored to Australia. That's our inference; Xero doesn't say. [S84]

**What it can change**

- Nothing. Anthropic's listing says "Claude connects with read-only access." [S84]
- Xero says Claude can't create, edit, approve, reconcile or pay anything in Xero. To act on something, you follow the link and make the change in Xero yourself. [S87]
- Xero calls it read-only "at launch", which suggests that may change. [S87]

**Does it ask first?**

- Claude can ask for your approval before it uses a tool. **Allow once** continues. **Always allow** skips the question for that tool from then on. You can change this later under the connector's **Tool permissions**. [S85]
- In Claude for Small Business, Anthropic says "Every workflow starts in approval mode." Claude drafts and stages the work, then waits for your approval before anything goes out. [S63]

**Your data**

- Anthropic's listing says "Any data retrieved is used only to respond to your questions and is never stored between sessions." [S84]
- Xero says "Your Xero data is never used to train AI", and that connector data "isn't combined across organizations". [S87]
- Xero also says "Your Claude plan and settings control conversation data use." [S87]
- Anthropic says raw content from connectors isn't used for training. On Claude's Free, Pro and Max plans, your chats are used if you've turned on **Model Improvement** in your privacy settings, and that includes anything you paste in. [S88]
- Anthropic says it doesn't train on business data by default on Team and Enterprise plans. [S62]

**To disconnect**

- **Just this chat:** select **+**, then **Connectors**, and switch Xero off. Claude stays signed in to Xero. [S85]
- **Disconnect:** go to **Customize > Connectors**, select Xero under **Your connectors**, and select **Disconnect**. Xero stays in your list showing **Connect**, so you can sign in again later. Xero Central adds that you click **Disconnect** a second time to confirm. [S85] [S43]
- **Remove it completely:** open the three-dot menu and select **Remove**. On Team and Enterprise plans, an Owner removes it for everyone from **Organization settings > Connectors**. [S85]
- **Just one organisation:** Xero Central says to disconnect Claude from the connected apps in that Xero organisation. [S43]
- **From Xero's side:** click the organisation name, select **Settings**, click **Connected apps**, then click **Disconnect** beside the app and confirm. This is Xero's general article for any connected app. It doesn't name Claude, ChatGPT, Copilot or Gemini. [S48]
- **What stays behind:** Xero says disconnecting stops new data going to the app, but data already sent may still be available. Neither company says what happens to Xero figures already in your Claude chats. [S48]

**A first safe thing to try**

- Ask "Who owes me money, and how overdue are they?" That uses the aged receivables tool, which only reads. [S84]
- Don't paste extra client details into the chat. Claude already reads what it needs from Xero, and pasted content counts toward training if Model Improvement is on. That's our advice. [S88]

**Limits**

- Read-only "at launch". [S87]
- Xero says the connector is "not a source of tax, compliance, or financial advice" and doesn't replace your accountant, bookkeeper or JAX. [S87]
- Xero Central says the connector gives data for one organisation at a time. If Claude adds figures across organisations, Xero doesn't check those totals. [S43]
- In Claude for Small Business, Xero appears in workflows such as the Monday weekly brief, Proposal Builder and Close the Month. [S62]
- Xero lists business pulse, overdue invoice chasing, cash flow snapshot, accounts payable preparation and month-end preparation among the workflows it supports there. [S34]
- Claude for Small Business is available on every paid Claude plan and runs in the Claude Cowork desktop app. [S62]

### ChatGPT and Xero

**Official?**

- Yes. The "Xero plugin in ChatGPT" is built by Xero Limited and powered by JAX. Xero said it was live on 16 September 2026. [S34] [S65]
- It works in ChatGPT's Chat and Work modes and in Codex. [S34]

**What it can see and do**

- Xero says it reads real-time profit and loss, balance sheet, invoices and bills, "and more". [S34]
- OpenAI's listing describes profit and loss, cash position, outstanding invoices and top customers, with links back to Xero. [S65]
- Xero Central's list goes further, covering bills and suppliers, repeating invoices and bills, contacts, and organisation details. Answers show interactive widgets that link through to Xero. [S46]
- The listing says ChatGPT connects with read-only access. [S65] [S66] Xero Central says ChatGPT can't change anything in your Xero organisation. [S46]
- Xero says you can build your own workflows that pull live Xero data. [S34]

**What you need**

- A Xero subscription. The sources we read don't name a required Xero plan. [S34] [S65] [S46]
- A ChatGPT account. OpenAI says availability depends on the plugin, your plan and your workspace settings, and some connections need admin approval. [S65]
- Xero Central asks for ChatGPT Plus, or access to ChatGPT Work, Codex or ChatGPT for Excel and Google Sheets. [S46]
- In ChatGPT Business, apps start switched on. In Enterprise and Edu, new plugins and apps generally stay off until an admin reviews them. [S81]

**Steps to connect** (OpenAI's plugin docs and Xero Central, all read 18 November 2026)

1. In ChatGPT on the web, desktop or mobile, open the **Plugins** tab and search for Xero. [S68] [S67]
2. Open the Xero plugin's details and select the plus button (OpenAI's help centre calls it **Install plugin**). [S68] [S67]
3. When asked, sign in with your Xero login. Select every Xero organisation you want ChatGPT to read, then click **Allow access**. [S46] [S67]
4. Start a new chat. Type **@** and pick Xero, or just ask and let ChatGPT choose. [S68]

Xero Central's own steps match. Open **Plugins**, search for Xero, select it and click **Install** or **Get started**, then sign in to Xero, select your organisations and click **Allow access**. [S46]

If you've connected more than one organisation, name the one you mean in your question. Xero says the plugin gives data for one organisation at a time and doesn't check totals ChatGPT adds up across them. [S91] [S46]

**To disconnect**

- Select **Uninstall plugin** where it's offered. OpenAI's help centre warns that uninstalling can disconnect all the accounts connected through the plugin. Its Learn docs add that a separately connected integration stays connected until you disconnect it. [S80] [S68]
- To disconnect just your Xero account: **Settings > Plugins** > Xero > the account's **•••** menu (or **Connection**) > **Disconnect**. [S80] Workspace admins can disable a plugin under **Workspace settings > Plugins**. [S67]
- Xero Central's ChatGPT article sends you to OpenAI's help to disconnect. To remove just one organisation, it says to disconnect ChatGPT from the connected apps in that Xero organisation. [S46] On the Xero side, use Xero's general steps under **Settings > Connected apps** (see Claude above). [S48]
- OpenAI says disconnecting doesn't delete your existing chats, saved files or memories. Review those separately. [S80]

**Limits**

- Read-only, per the listing. [S65]
- OpenAI's listing says retrieved data is used only to answer you and isn't stored between sessions. [S65]
- ChatGPT's listing also says ChatGPT may share relevant chats and memories with the Xero plugin, under Xero's terms and privacy policy. [S66]
- The same listing says ChatGPT respects your training settings for data from connected apps. [S66] On Free, Go, Plus and Pro, OpenAI may use information from apps to train its models if **Improve the model for everyone** is on. Business, Enterprise and Edu aren't used for training by default. [S79]
- OpenAI's docs say that when ChatGPT sends data through a plugin's server, that service's terms and privacy policy apply. [S68]

### Microsoft Copilot and Xero

**Official?**

- Yes. Xero calls it the "Xero agent in Microsoft 365 Copilot". It launched on 1 July 2026. [S7] [S47] [S26]
- Microsoft's own documentation now calls it Microsoft Copilot, while Xero still says Microsoft 365 Copilot, so you may see either name. [S69] [S47]

**What it can see and do**

- Profit and loss, cash position, receivables, payables, overdue invoices and top customers. Answers can cover a month, quarter, financial year or year-on-year. [S7]
- Xero says "Copilot is read-only at launch". Links open the report, invoice or customer record in Xero, where you make any change. [S7]
- Xero's launch release said it worked in Copilot Chat, Excel, Word and PowerPoint. [S26]
- Xero's 16 September 2026 blog lists Excel, Word, PowerPoint and Copilot Cowork as "coming soon". These two Xero sources conflict. [S34]
- Xero plans Outlook and Teams support "in the months ahead". [S27]

**What you need**

- A paid Microsoft 365 Business or Enterprise account, plus a Xero subscription. [S7] Xero Central says the agent works in Copilot chat and connects to any organisation on a Xero business pricing plan. [S47]
- Xero's Australian Copilot page is more specific. It asks for "a paid Microsoft 365 Copilot licence". [S94]
- Your IT admin may need to approve the agent. [S71] Xero Central says your Microsoft 365 administrator has to enable the Xero agent first. [S47]

**Steps to connect** (Xero Central, updated 10 November 2026; read 18 November 2026)

1. From your Microsoft 365 account, open Copilot chat. [S47]
2. Under **Agents**, find and open Xero. Or go to the Agent Store, find Xero and click **Add** or **Open**. If your admin hasn't enabled it, you'll see an option to request approval instead. [S47] [S71]
3. Ask a question about your Xero data. [S47]
4. Follow the prompts to sign in to Xero. Select every organisation you want Copilot to read, then click **Allow access**. [S47]
5. Ask about profit, cash, receivables or overdue invoices. If you've connected more than one organisation, name the one you mean. [S7] [S47]

For admins, the **Integrated apps** section of the Microsoft 365 admin center shows each agent's permissions, terms and privacy statement. Admins choose which agents are allowed. [S69] [S70]

**To disconnect**

- Xero's steps: in Copilot chat, open **Settings** (on the web, from the menu next to your name; in the desktop app, from the menu at the top right of a Xero chat). Click **Agents**, open Xero and click **Sign out**. [S47]
- Admins can block or remove agents in the Microsoft 365 admin center. [S70]
- To remove just one organisation, Xero Central says to disconnect Copilot from the connected apps in that Xero organisation. [S47]
- On the Xero side, use Xero's general steps under **Settings > Connected apps** (see Claude above). [S48]

**Limits**

- Read-only at launch. [S7]
- Xero says "Your Xero data is session-based and not used to train models." [S7]
- Xero's release says the data is never used to train Copilot's models. [S26]
- Microsoft says prompts, responses and Microsoft 365 data aren't used to train its foundation models. It also tells you to check each agent's own privacy statement and terms. [S69]
- When Copilot uses an agent, Microsoft sends it a query based on your prompt, your Copilot history and Microsoft 365 data you can access. [S69]
- Microsoft says customers outside the EU may have their queries processed in the US, the EU or other regions. [S69]

### Google Gemini and Xero

**Official?**

- Yes, announced 14 October 2026 as the "Xero connected app for Google Gemini". [S36]
- Xero's Australian release notes list it as live in October 2026. Google's own Connected Apps table now lists Xero. [S91] [S95]

**What it can see and do**

- Profit and loss, income and expenses, balance sheet and cash position. [S36]
- Overdue balances, payables, overdue bills, customer and supplier contacts, and charts such as aged receivables. [S36]
- It can draft invoice summaries and complete routine tasks. [S36]
- Xero's launch release said any change to financial data, such as issuing an invoice or sending a payment reminder, "requires explicit user confirmation" in Gemini first. [S36]
- Xero Central's help article, updated 4 November 2026, says Gemini "can't make changes to your Xero organisation". Anything that sends an email or changes a document happens in Google's apps, and you confirm it there. [S90]
- The two Xero pages disagree. The help article is the newer one and describes how to use the connection, so expect read-only answers. That's our reading. [S36] [S90]
- Gemini Spark, which Xero Central calls Google's agent mode for scheduled tasks, can run jobs such as a daily cash summary or overdue-invoice reminders drafted in Gmail for you to review and send. Xero's launch release had called this Gemini Tasks, "coming soon". [S90] [S36]

**What you need**

- Xero Central says any Xero business plan and a Google account with access to Gemini. Scheduled tasks in Gemini Spark also need a Google AI Pro or AI Ultra plan. [S90]
- Google's table lists the Xero app for personal Google accounts only, for people 18 or over, in English. [S95]
- Google's general article for work or school accounts says a Workspace admin must enable connected apps. With Xero listed as personal-only, a work or school Google account appears not to be able to use it for now. That's our inference. [S73] [S95]

**Steps to connect** (Xero Central, updated 4 November 2026, with Google's menu names; both read 18 November 2026)

1. Go to gemini.google.com. [S72]
2. In the sidebar, click **Customize** (click **More** first if you don't see it), then click **Connectors** at the top. Xero Central calls this page Connected Apps. [S72] [S90]
3. Find and open Xero, then click **Connect**. Google's general steps call this button **Add**, so select whichever you see. [S90] [S72]
4. Enter your Xero email and password if asked. Select every organisation you want to use with Gemini, then click **Allow**. [S90]
5. In a chat, include **@Xero** or "Xero" in your question. If you've connected more than one organisation, name the one you mean. [S90] [S72]

**To disconnect**

- In Gemini, go to **Customize > Connectors**, click **More options** next to the app, then **Disconnect**. [S72]
- Xero Central's version: open Xero there, click **Disconnect**, then **Disconnect** again to confirm. [S90]
- To remove just one organisation, Xero Central says to disconnect Gemini from the connected apps in that Xero organisation. [S90]
- On the Xero side, use Xero's general steps under **Settings > Connected apps** (see Claude above). [S48]

**Limits**

- Xero says data shared between the platforms is used only for your session. [S36]
- Xero says "Xero data is not used to train Google Gemini models." [S36]
- Xero Central says the connector gives data for one organisation at a time, and Xero doesn't check totals Gemini adds up across organisations. [S90]
- Google says connected app availability varies by location, language, device and Gemini app. Its table says Xero works wherever both Gemini Apps and Xero are supported, without listing countries. [S72] [S95]

### Xero's MCP server and API (the developer route)

**Official?**

- Yes. Xero publishes an open-source MCP server, "xero-mcp-server", on GitHub under the MIT licence. [S55]
- It's part of Xero's AI Toolkit, alongside an Agents Toolkit and a Prompt Library. [S54] [S57]
- Xero's own Claude page calls the MCP server "a developer tool for custom workflows and automations". [S6]
- Xero says MCP server usage grew tenfold between December 2025 and May 2026. [S41]
- The latest version is 0.0.18, published 10 November 2026. Xero's change notes say it fixes security vulnerabilities. The code was last changed on 9 November 2026 (UTC). [S56] [S55]

**What it can see and do**

- It has 51 tools. [S55]
- Read tools cover accounts, contacts, invoices, credit notes, items, manual journals, quotes, tax rates, payments, bank transactions, tracking categories, and reports such as profit and loss, balance sheet, trial balance and aged receivables and payables. [S55]
- Create and update tools cover invoices, quotes, contacts, credit notes, items, manual journals, bank transactions, payment records and tracking categories. [S55]
- It also has payroll tools, including one that deletes timesheets. The README says that for payroll queries "the region should be either NZ or UK", so they don't cover Australian payroll. [S55]

**What you need**

- Node.js 18 or later and an AI app that can run a local MCP server. [S55] [S54]
- Xero says "some development or programming experience is needed" for its Agentic Toolkit. Its MCP server testing used Claude Desktop and Cursor. [S54]
- A custom connection, which gives you a client ID and secret for one organisation. Developers juggling several organisations can use a bearer token from their own sign-in flow instead. [S55]
- Custom connections are only for organisations in Australia, New Zealand, the UK and the US. Each one connects to a single organisation. [S51] [S52]
- Each costs "$10/m AUD (inc GST)" as a recurring monthly charge to the organisation. They're free on the Xero Demo Company. [S52]
- From 1 December 2026 Xero won't let you create a new custom connection app or buy a new custom connection subscription. Connections created before then keep working as they do now. [S51]
- After that, a new setup appears to need the bearer-token option above, which means running your own Xero sign-in flow. Xero gives no step-by-step guide for doing that with the MCP server. That's our reading. [S55] [S51]

**Steps to connect** (Xero's developer pages, not dated; README last changed 9 November 2026. Steps 1 and 3 only work until 30 November 2026.)

1. On developer.xero.com, set up a custom connection and choose its permissions (scopes). Enter the email address of the Xero user who will authorise it. If you're building for your own business, that user is you. [S52] [S51]
2. That Xero user opens Xero's email and follows it to authorise the connection to their organisation. [S51] [S52]
3. Buy a custom connection subscription for the organisation, at $10 a month. [S52]
4. Install Node.js and add the Xero MCP server to your AI app's local settings. Keep the client ID and secret only in that local file on your own computer. Never paste them into a chat or a website. Xero's README warns against committing credentials anywhere. [S55]
5. Test against the Demo Company first. [S55] [S52]
6. Restart your AI app and ask something simple, such as a list of overdue invoices. Read every create or update request before you approve it. [S55]

**To disconnect**

- Xero Central's steps for disconnecting a connected app: click the organisation name, select **Settings**, click **Connected apps**, then click **Disconnect** beside the app. [S48]
- Editing a custom connection deactivates it until it's re-authorised. [S51]
- Xero lists custom connection subscriptions separately, under **App Store subscriptions** on the same screen. To cancel one, click its name there, then **Cancel subscription**. [S48]

**Limits**

- Custom connections created from 29 April 2026 use narrower "granular" permissions that don't include journals. Older connections can keep their broad permissions until September 2027. [S51] [S55]
- Xero's API limits are 60 calls a minute and five at once, plus a daily cap of 1,000 or 5,000 calls per organisation depending on the developer tier. [S50]
- Xero's developer terms forbid using data from its APIs to train, fine-tune, adapt or enhance AI models. [S53]
- The same terms say API data can't be passed to another third party without the user's consent. [S53]
- If you build your own app with standard Xero sign-in instead, developer tiers apply from 2 March 2026: Starter is free for up to 5 connections and Core is $35 a month (excluding tax) for up to 50. [S49]
- Custom connections stay on their existing commercial terms and are excluded from the new tiers. [S50]
- Anthropic's listing gives the hosted Xero endpoint as https://mcp.xero.com/mcp. ChatGPT's plugin listing shows the same address. We found no Xero documentation for using that endpoint with other AI apps. [S60] [S66]

### AI apps listed on the Xero App Store

- Xero's Australian App Store has a collection called "AI apps for bills and expenses". [S58]
- On 18 November 2026 it listed the same 15 apps as on 15 October: BillBjorn, BookWell, DOKKA, Dext, FINNEX AI Assistant, Fresho, Pulsify, Receipt Bot, Receiptor AI, Restoke, SimpleAI Books, Synced, WellyBox, fileAI and tofu. [S58]
- FINNEX's listing describes a "ChatGPT-style AI assistant" in Excel for bookkeeping, billing, invoicing and reporting in Xero. [S58]
- SimpleAI Books' listing describes an AI agent that categorises transactions and reconciles bank feeds. [S58]
- Receiptor AI's listing says it finds receipts and invoices in your email, WhatsApp and iMessage and files them in Xero. [S58]
- Two general automation tools also have listings on the Australian App Store. Zapier's listing describes "Zaps" that link Xero with your other apps. [S74]
- Make's listing describes it as a no-code platform for AI agents and automations that connects Xero data to the rest of your business. [S75]
- These descriptions are the vendors' own listing text. Xero's terms say it doesn't endorse or take responsibility for third-party products. [S58] [S74] [S75] [S20]
- Xero commits to sharing your data with ecosystem partners only with your express consent. [S17]

## Jobs it's good for

- **The Monday money check.** Ask JAX, Claude, ChatGPT, Copilot or Gemini who owes you and how overdue they are. Then follow the link into Xero to send reminders. [S2] [S60] [S65] [S7] [S90]
- **Cash before a big bill.** Ask for your cash position across bank accounts before you commit to a payment. [S60] [S7] [S36]
- **An invoice from last month's quote.** Ask JAX to create an invoice based on the last quote for that customer. Check it before it goes out. [S2] [S16]
- **Receipts on the go.** Photograph a receipt in the Xero Accounting app. Smart Document Capture reads it and you approve the details. Then accept or reject the bank match it suggests. [S10]
- **Bank reconciliation on one tidy account.** Turn on auto bank reconciliation for an account with steady transactions and good bank rules. Review the Reconciled page each week. [S8] [S9]
- **Month-end preparation.** Claude for Small Business has a Close the Month workflow that lists Xero as a connector and waits for your approval. Practices work one client organisation at a time. [S62] [S63] [S34]
- **Before a client meeting.** In Partner Hub, ask JAX (beta) to summarise the client. [S14]
- **Comparing with the industry.** On Ultimate or Ultra, compare ratios such as debtor days with businesses like yours. [S39] [S1]
- **"How do I" questions.** Ask JAX how to do something in Xero and get an answer from Xero's help content. [S2]
- **A small custom tool.** Someone with programming skills can use the MCP server to create or update records in bulk, tested first on the Demo Company. [S55] [S52]

## What to watch for

**The AI sees what the login sees**

- JAX chat follows Xero's normal roles, so people only see what they're already allowed to see. [S2]
- Anthropic says Claude inherits each person's permissions from the connected service. [S61]
- Microsoft says Copilot only shows data each person can already access. [S69]
- So the login you connect with sets the limit. An adviser's login will expose everything that adviser can see. That's our inference from the above.

**Read-only now, actions later**

- The Claude, ChatGPT and Copilot connections are described as read-only "at launch", which suggests write access may come. [S6] [S7] [S65]
- Xero's Gemini launch release said Gemini could issue invoices after you confirm. Xero Central now says Gemini can't change anything in Xero, though Gemini Spark can draft reminder emails in Gmail for you to send. [S36] [S90]
- JAX itself can approve and send invoices and quotes when your Xero role allows it. [S76]
- The MCP server can create and update records, and delete payroll timesheets in NZ and UK organisations. [S55]
- Claude for Small Business lets you switch a trusted workflow from approval mode to running on its own. [S63]

**Training and who keeps what**

- Xero says JAX chat doesn't train language models on your data. [S2]
- Xero says data passed to Claude, Copilot and Gemini is used only for your session and isn't used to train their models. [S24] [S26] [S36]
- Your chat history on the AI side still follows that company's own settings. On Claude's Free, Pro and Max plans that's the **Model Improvement** setting. [S64] In ChatGPT it's **Improve the model for everyone**. [S79]
- ChatGPT's listing says ChatGPT may share relevant chats and memories with the Xero plugin. [S66]
- Xero itself may use anonymised data. Bank matching predictions draw on other users' reconciliations, and benchmarks are built from anonymised, aggregated data. [S8] [S39] [S20]
- Xero's privacy notice, updated 26 October 2026, says it may use "AI/ML" to understand customer behaviour and improve its services. [S19]

**Where your data goes**

- Xero's AI providers (Anthropic and OpenAI) and its cloud hosts are listed as located in the United States. [S18]
- Xero's privacy notice says data may be processed in Australia, New Zealand and the United States. [S19]
- Microsoft says queries from outside the EU may be processed in the US, the EU or other regions. [S69]
- We found no option to keep AI processing inside Australia. [S2] [S18] [S19]

**Check the work**

- Xero's terms make you responsible for checking the accuracy of information you use from Xero. [S20]
- Xero reports about 96% accuracy on lines it auto-reconciles, so a small share still gets corrected. [S8]
- Xero says document capture is most accurate on clear, standard documents, and tells you to check before records are created. [S10]
- Microsoft says AI responses "aren't guaranteed to be 100% factual". [S69]
- JAX's research answers, such as minimum wage rates, draw on outside information. Check them against the official source. That's our advice, based on what JAX says it can answer. [S2] [S21]
- Xero Central says JAX's figures come from the account types in your chart of accounts. They can differ from your reports if you've customised report layouts or use report templates. [S78]
- JAX may not show your latest changes straight away. Xero Central says to refresh the data in Analytics and ask again. [S78]

**Not advice**

- Xero says the Claude connector is not a source of tax, compliance or financial advice. [S6]
- Xero's terms say its information "should not be seen as a substitute for professional advice". [S20]

**Cost surprises**

- Ignite allows 20 invoices, and invoices created by connected apps can count toward that. [S1]
- Xero's bank reconciliation page doesn't price the AI Automate add-on for Ignite. The pricing page lists auto-reconcile on Ignite at $8 a month. [S9] [S1]
- Each custom connection costs $10 a month, and Xero stops selling new ones from 1 December 2026. [S52] [S51]
- Apps you build with standard sign-in pay developer tier fees once you pass five connections. [S49]
- JAX chat has no extra charge "currently", and Xero reserves the right to change that. [S2]
- Claude for Small Business needs a paid Claude plan. [S62] The Copilot agent needs a paid Microsoft 365 Business or Enterprise account, and Xero's Australian Copilot page asks for a paid Microsoft 365 Copilot licence. [S7] [S94]
- Scheduled tasks with Xero in Gemini Spark need a Google AI Pro or AI Ultra plan. [S90]
- Syft Advanced comes only with Ultra at $500 a month. [S1]

**Who can switch things on and off**

- JAX chat: Xero roles and permissions. [S2]
- Auto bank reconciliation: the subscriber or a user with the administrator role, for one bank account or all of them at once. [S44]
- Claude Team and Enterprise: Owners add connectors and can set each tool to **Always allow**, **Needs approval** or **Blocked**. [S61]
- Microsoft Copilot: admins allow or block agents in the Microsoft 365 admin center. [S69] [S70]
- ChatGPT business workspaces: apps start switched on in Business, while new plugins and apps in Enterprise and Edu stay off until an admin reviews them. Admins can also disable a plugin. [S81] [S67]
- Gemini: Google lists the Xero app for personal Google accounts only. For work or school accounts, Google says the Workspace admin enables connected apps in general. [S95] [S73]

**Logins and AI browser agents**

- Xero's terms say to keep your login details safe and not let anyone else use them. [S20]
- Xero's developer terms ban bots and browser extensions that simulate user actions without Xero's authorisation. [S53]
- Our reading: use the official connections that ask you to approve access, and don't give an AI tool your Xero password. General information, not legal advice.

**Untrusted text**

- Anthropic's listing warns: "Only use connectors from developers you trust." [S60]
- Microsoft describes attacks where hidden instructions in content try to steer an AI, and says Copilot uses classifiers to block them. [S69]
- Supplier bills and emails can carry text like that. Keep a person in the loop before anything is changed. That's our inference.

**Beta features**

- JAX for practices is beta. [S14] Bill Protection and Cash Flow Actions were beta as of July 2026. [S30]
- Xero's terms say beta services are used at your own risk. [S20]

**Two meanings of JAX**

- JAX chat only acts when someone asks it something. [S2]
- JAX automation, such as bank reconciliation and document capture, runs in the background once it's on. [S4] [S9]
- Know which one you've switched on.

## Announced changes

Xero's JAX vision page carries a warning that "future product features may differ" and that Xero isn't obliged to deliver them. Treat every "coming soon" below the same way. [S5]

- **4 December 2025:** New Xero developer terms took effect for new developers. They ban using Xero API data to train AI models. [S53] [S50]
- **2 March 2026:** New developer pricing tiers took effect, and existing developers became bound by the new terms. [S49] [S50]
- **29 April 2026:** New custom connections switched to granular permissions without journal access. Broad permissions on older connections last until September 2027. [S51]
- **13 May 2026:** Xero announced the Claude integration as live. [S24]
- **14 May 2026:** XeroForce announced as an invite-only alpha, with general release "later this year". [S25] [S41]
- **1 July 2026:** Xero's Microsoft 365 integration launched. Outlook and Teams are planned "in the months ahead". [S26] [S27]
- **7 July 2026:** Ultra launched in Australia. Flexible user permissions were promised "shortly after launch". [S28]
- **8 July 2026 (Xerocon London):** Xero announced Bill Protection (beta), Cash Flow Actions (beta) and Payment Follow Ups (coming soon). Bill Protection checks bills before payment and flags things such as changed bank details or unfamiliar suppliers. [S29] [S30]
- At the same event, Xero labelled document chasing and the Partner Hub book health view "available from October". [S30]
- By November 2026, Xero Central said document requests sent by JAX were "only available to a small number of UK practices". [S96]
- It also said bank statement extraction and auto-created transactions are coming to Smart Document Capture. [S30]
- **20 August 2026 (Xerocon US):** Xero named a ChatGPT integration. It said automating split payments in bank reconciliation would come "in the coming months". [S33]
- **16 September 2026:** The ChatGPT plugin went live and Xero joined Claude for Small Business. [S34]
- Xero said switching between client organisations without reconnecting is coming, along with Excel, Word, PowerPoint and Copilot Cowork support. [S34]
- **18 September 2026:** Files was renamed Documents. Planned additions include supplier rules and a bespoke email address. Tax number validation is planned for the UK and Australia. [S35]
- **September 2026:** Xero Partner Hub went live to all practices, according to Xero's Australian release notes. [S91]
- **13 October 2026:** Xero's JAX release notes listed payment follow-ups as in early access. JAX builds a schedule to chase overdue invoices on your behalf, and you can review, edit and approve the follow-ups at any time. [S97]
- **14 October 2026:** The Gemini connected app was announced, with Gemini Tasks "coming soon". [S36]
- **October 2026:** Xero's Australian release notes list the Gemini connection, with scheduled tasks in Gemini Spark, and the option to connect several organisations to Claude, ChatGPT and Copilot. [S91]
- **27 October 2026:** Xero and Anthropic scheduled a webinar on Claude for Small Business. [S34]
- **11 November 2026:** Xero blogged about its new Budgets, with smart suggestions, under **Reporting**. [S92]
- **12 November 2026:** Xero announced Xforce, a beta service where its engineers help accounting firms build AI workflows. It still described XeroForce as in beta. [S93]
- **1 December 2026:** Xero stops letting anyone create a new custom connection app or buy a new custom connection subscription. Existing connections keep working. [S51]
- **15 and 16 February 2027:** Unused custom connection subscriptions must be connected to an app or cancelled by 15 February. Xero cancels the rest on 16 February, and a cancelled subscription can't be bought again. [S51]
- **Naming:** Microsoft 365 Copilot is now called Microsoft Copilot. [S69]
- **Naming:** Xero HQ is being folded into Xero Partner Hub. [S40] [S14]

## What we couldn't establish

- Xero Central pages show no last-updated date, so the Sources table gives each article's date from Xero Central's sitemap. [S42]
- **Which ChatGPT plans can use the Xero plugin, by OpenAI's account.** OpenAI's pages say it depends on the plugin, your plan and your workspace settings, without listing plans. Xero Central asks for ChatGPT Plus, or access to ChatGPT Work, Codex or ChatGPT for Excel and Google Sheets. [S65] [S67] [S46]
- **Australian availability, stated outright,** for the ChatGPT plugin, the Gemini connection and the Copilot agent. Xero's Australian release notes list all three, and Google's table says Xero works wherever Gemini Apps and Xero are both supported, which suggests they work here. That's our inference. No page names Australia. [S91] [S95] [S46] [S47]
- **Which Microsoft licence the Copilot agent needs.** Xero's Australian Copilot page asks for a paid Microsoft 365 Copilot licence. Xero Central and Xero's campaign page mention only a paid Microsoft 365 Business or Enterprise plan. [S94] [S47] [S7]
- **Excel, Word and PowerPoint support** for the Xero agent. Xero's July release says it was there at launch, but its September blog lists them as coming soon. Xero Central's article mentions only Copilot chat. [S26] [S34] [S47]
- **Whether Gemini can change anything in Xero.** Xero's 14 October release says it can issue invoices after you confirm. Xero Central's 4 November article says it can't change your Xero organisation. [S36] [S90]
- **The Microsoft Agent Store listing** for the Xero agent. It's only reachable from inside a signed-in Copilot account, so we relied on Xero's and Microsoft's help pages. [S47] [S71]
- **Whether the $8 AI Automate price includes GST.** Xero's pricing page says its prices include GST, but it lists the add-on separately and doesn't use the name AI Automate. [S1]
- **What "basic extraction" leaves out** compared with full Smart Document Capture. [S1]
- **JAX by SMS, WhatsApp or email in Australia.** This was described in March 2025 but isn't on the current Australian JAX page. [S22] [S2]
- **Payment follow-ups in Australia.** Xero's JAX release notes say payment follow-ups are in early access, and that features vary by plan and region. We couldn't confirm when they reach Australian customers generally. [S97]
- **How long JAX keeps chat history**, and in which country JAX processing happens. Xero Central says you can't delete or rename JAX chats. [S2] [S45]
- **Which models do what.** The JAX FAQ names AWS, Azure, GCP and OpenAI, but the sub-processor list also includes Anthropic. [S2] [S18]
- **Whether auto bank reconciliation is off by default.** The documentation only describes turning it on per account. [S8]
- **Who can buy a custom connection.** A search-engine copy of Xero's developer pages said users with the Standard, Advisor or Administrator role and the Connected Apps permission can buy and manage one. We couldn't confirm this on a page we read directly.
- **The hosted endpoint mcp.xero.com.** Claude's and ChatGPT's listings both show it. We couldn't confirm whether Xero supports it for other AI apps, or what limits apply. [S60] [S66]
- **What replaces custom connections for the MCP server** after 1 December 2026. Xero's FAQ doesn't say, and the README's bearer-token option has no step-by-step guide. [S51] [S55]
- **AI in Xero Practice Manager.** None found in the sources we read. [S14]
- **Hubdoc's future** alongside Smart Document Capture. No retirement notice was found. [S59]
- **Claude for Small Business in Australia.** Anthropic's announcement doesn't say whether it's offered here. [S62]
- We didn't rely on third-party claims. For example, one vendor said it found no Xero listing in ChatGPT on 7 October 2026, but Xero's and OpenAI's own pages say the plugin exists.

## Sources

All sources were read on 18 November 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Plans to suit your business (Australia) | Xero | https://www.xero.com/au/pricing-plans/ | No date shown (© 2026) | 18 Nov 2026 |
| S2 | JAX, your AI finance partner (Just Ask Xero) | Xero | https://www.xero.com/au/jax/ | No date shown | 18 Nov 2026 |
| S3 | JAX, your AI finance partner (features page) | Xero | https://www.xero.com/au/ai-in-accounting/jax/ | No date shown | 18 Nov 2026 |
| S4 | AI in accounting | Xero | https://www.xero.com/au/ai-in-accounting/ | No date shown | 18 Nov 2026 |
| S5 | JAX vision | Xero | https://www.xero.com/au/ai-in-accounting/jax-vision/ | No date shown | 18 Nov 2026 |
| S6 | Claude (Xero connector in Claude) | Xero | https://www.xero.com/au/ai-in-accounting/claude/ | No date shown | 18 Nov 2026 |
| S7 | Ask Copilot About Your Xero Finance Data | Xero | https://www.xero.com/au/campaign/copilot-connector/ | No date shown | 18 Nov 2026 |
| S8 | Auto Bank Reconciliation | Xero | https://www.xero.com/au/campaign/auto-bank-reconciliation/ | No date shown; figures are a rolling average for April to July 2026 | 18 Nov 2026 |
| S9 | Bank reconciliation | Xero | https://www.xero.com/au/accounting-software/reconcile-bank-transactions/ | No date shown | 18 Nov 2026 |
| S10 | Smart document capture (Files) | Xero | https://www.xero.com/au/accounting-software/store-files/ | No date shown | 18 Nov 2026 |
| S11 | Analytics | Xero | https://www.xero.com/au/accounting-software/analytics/ | No date shown | 18 Nov 2026 |
| S12 | Ultra plan | Xero | https://www.xero.com/au/pricing-plans/ultra/ | No date shown | 18 Nov 2026 |
| S13 | Ignite plan | Xero | https://www.xero.com/au/pricing-plans/ignite/ | No date shown | 18 Nov 2026 |
| S14 | Xero Partner Hub | Xero | https://www.xero.com/au/accountants-bookkeepers/partner-hub/ | No date shown | 18 Nov 2026 |
| S15 | Xero Tax | Xero | https://www.xero.com/au/xero-tax/ | No date shown | 18 Nov 2026 |
| S16 | AI product philosophy | Xero | https://www.xero.com/au/campaign/ai-product-philosophy/ | No date shown | 18 Nov 2026 |
| S17 | Responsible data use at Xero | Xero | https://www.xero.com/au/data/ | Commitments "updated in 2024" | 18 Nov 2026 |
| S18 | Xero sub-processors | Xero | https://www.xero.com/au/legal/xero-subprocessors/ | No date shown | 18 Nov 2026 |
| S19 | Privacy notice | Xero | https://www.xero.com/au/legal/privacy/ | Last updated 26 Oct 2026 | 18 Nov 2026 |
| S20 | Terms of use | Xero | https://www.xero.com/au/legal/terms/ | Last updated 26 Oct 2026 | 18 Nov 2026 |
| S21 | Xero's AI Financial Superagent 'JAX' Launches Powerful New Features | Xero (media release) | https://www.xero.com/au/media-releases/xeros-ai-financial-superagent-jax-launches-powerful-new-features/ | 3 Sep 2025 | 18 Nov 2026 |
| S22 | JAX beta expands | Xero Blog | https://blog.xero.com/au/product-updates/jax-beta-expands | Published 11 Mar 2025; updated 24 Mar 2025 | 18 Nov 2026 |
| S23 | Xero and Anthropic Collaborate to Bring AI-Powered Financial Intelligence to Millions of Small Businesses | Xero (media release) | https://www.xero.com/us/media-releases/xero-and-anthropic-collaborate/ | 27 Mar 2026 | 18 Nov 2026 |
| S24 | Xero Delivers Claude Integration to Advance AI-Powered Financial Intelligence | Xero (media release) | https://www.xero.com/au/media-releases/xero-delivers-claude-integration-to-advance-ai-powered-financial-intelligence/ | 13 May 2026 | 18 Nov 2026 |
| S25 | Xero Introduces XeroForce | Xero (media release) | https://www.xero.com/au/media-releases/xero-introduces-xeroforce/ | 14 May 2026 | 18 Nov 2026 |
| S26 | Xero Launches Integration with Microsoft 365 | Xero (media release) | https://www.xero.com/us/media-releases/xero-launches-integration-with-microsoft-365/ | 1 Jul 2026 | 18 Nov 2026 |
| S27 | Xero + Microsoft 365: Real-time financial intelligence, right where you work | Xero Blog | https://blog.xero.com/product-updates/xero-microsoft-365-integration/ | 2 Jul 2026 | 18 Nov 2026 |
| S28 | Xero targets Australia's medium-sized businesses with launch of Ultra | Xero (media release) | https://www.xero.com/au/media-releases/xero-targets-medium-businesses-with-ultra/ | 7 Jul 2026 | 18 Nov 2026 |
| S29 | Xero Announces New AI Innovations at Xerocon London | Xero (media release) | https://www.xero.com/au/media-releases/xero-announces-new-ai-innovations-xerocon-london/ | 9 Jul 2026 | 18 Nov 2026 |
| S30 | Xerocon London 2026: The Agentic Era Has Arrived for Small Business Finance | Xero Blog | https://blog.xero.com/product-updates/xerocon-london-2026-agentic-era-small-business-finance/ | 8 Jul 2026; updated 23 Jul 2026 | 18 Nov 2026 |
| S31 | Accountable Intelligence (JAX) | Xero Blog | https://blog.xero.com/news-events/accountable-intelligence-ai-jax/ | 17 Mar 2026 | 18 Nov 2026 |
| S32 | What's new in Auto Bank Reconciliation | Xero Blog | https://blog.xero.com/product-updates/auto-bank-rec-updates/ | 14 Aug 2026; updated 19 Aug 2026 | 18 Nov 2026 |
| S33 | Xero Announces New AI Innovations for Small Businesses and Accountants at Xerocon US | Xero (media release) | https://www.xero.com/us/media-releases/new-ai-innovations-xerocon-denver/ | 20 Aug 2026 | 18 Nov 2026 |
| S34 | Xero Wherever You Work: Real-Time Financial Intelligence in Claude for Small Business and ChatGPT | Xero Blog | https://blog.xero.com/product-updates/claude-for-small-business-chatgpt-ai-integrations-launch/ | 16 Sep 2026 | 18 Nov 2026 |
| S35 | Files is now called Documents | Xero Blog | https://blog.xero.com/product-updates/files-now-called-documents/ | 18 Sep 2026 | 18 Nov 2026 |
| S36 | Xero brings real-time financial intelligence to Google Gemini | Xero (media release) | https://www.xero.com/au/media-releases/xero-brings-real-time-financial-intelligence-to-google-gemini/ | 14 Oct 2026 | 18 Nov 2026 |
| S37 | Xero to bring AI-powered data capture and extraction into platform ahead of Making Tax Digital | Xero (media release) | https://www.xero.com/au/media-releases/major-transformation-to-document-management-capabilities/ | 18 Feb 2026 | 18 Nov 2026 |
| S38 | Xero introduces enterprise-grade analytics | Xero (media release) | https://www.xero.com/au/media-releases/xero-introduces-enterprise-grade-analytics/ | 15 Jan 2026 | 18 Nov 2026 |
| S39 | Xero Introduces Industry Benchmarking Intelligence for Small Businesses | Xero (media release) | https://www.xero.com/au/media-releases/xero-introduces-industry-benchmarking-intelligence-for-small-businesses/ | 29 Jun 2026 | 18 Nov 2026 |
| S40 | Introducing Xero Partner Hub | Xero Blog | https://blog.xero.com/product-updates/xero-partner-hub/ | 22 Sep 2025; updated 2 Jul 2026 | 18 Nov 2026 |
| S41 | Customizing their way: the rise of the builders | Xero Blog | https://blog.xero.com/product-updates/rise-of-the-builders-custom-apps-ai/ | 21 Aug 2026 | 18 Nov 2026 |
| S42 | Xero Central article sitemap (titles and last-modified dates) | Xero | https://central.xero.com/0/sitemap-webarticle-1.xml | Per-article dates, e.g. Claude article 10 Nov 2026 | 18 Nov 2026 |
| S43 | Connect Xero using the Xero connector in Claude | Xero Central | https://central.xero.com/0/article/Connect-Xero-using-the-Xero-connector-in-Claude | No date shown (sitemap: 10 Nov 2026) | 18 Nov 2026 |
| S44 | How to use automatic bank reconciliation (Australia and New Zealand) | Xero Central | https://central.xero.com/0/article/How-to-use-automatic-bank-reconciliation-NZ-AU | No date shown (sitemap: 3 Nov 2026) | 18 Nov 2026 |
| S45 | Use JAX (BETA), Australia | Xero Central | https://central.xero.com/0/article/Use-Just-Ask-Xero-JAX-AU | No date shown (sitemap: 24 Aug 2026) | 18 Nov 2026 |
| S46 | Connect Xero to ChatGPT | Xero Central | https://central.xero.com/0/article/Connect-Xero-using-the-Xero-plugin-in-ChatGPT | No date shown (sitemap: 10 Nov 2026) | 18 Nov 2026 |
| S47 | Use the Xero agent in Microsoft 365 Copilot | Xero Central | https://central.xero.com/0/article/Use-the-Xero-agent-in-Microsoft-365-Copilot | No date shown (sitemap: 10 Nov 2026) | 18 Nov 2026 |
| S48 | Update, cancel, disconnect or review connected apps | Xero Central | https://central.xero.com/0/article/Access-review-or-disconnect-app-connections | No date shown (sitemap: 9 Sep 2026) | 18 Nov 2026 |
| S49 | Pricing | Xero Developer | https://developer.xero.com/pricing | No date shown; effective dates 4 Dec 2025 and 2 Mar 2026 | 18 Nov 2026 |
| S50 | Pricing and Policy Updates FAQs | Xero Developer | https://developer.xero.com/faq/pricing-and-policy-updates | No date shown | 18 Nov 2026 |
| S51 | Custom Integration FAQs | Xero Developer | https://developer.xero.com/faq/custom-integration | No date shown | 18 Nov 2026 |
| S52 | Xero Custom Development (Custom Connections) | Xero Developer | https://developer.xero.com/custom-development | No date shown | 18 Nov 2026 |
| S53 | Developer Platform Terms and Conditions | Xero Developer | https://developer.xero.com/xero-developer-platform-terms-conditions | Last updated 4 Dec 2025 | 18 Nov 2026 |
| S54 | AI Toolkit FAQs | Xero Developer | https://developer.xero.com/faq/AI-Toolkit | No date shown | 18 Nov 2026 |
| S55 | xero-mcp-server (README) | Xero (XeroAPI on GitHub) | https://github.com/XeroAPI/xero-mcp-server | Last commit 9 Nov 2026 (UTC, from GitHub's commit list for this repo) | 18 Nov 2026 |
| S56 | @xeroapi/xero-mcp-server (package record) | npm registry | https://registry.npmjs.org/@xeroapi%2fxero-mcp-server | Version 0.0.18 published 10 Nov 2026 | 18 Nov 2026 |
| S57 | XeroAPI organisation repositories | Xero (XeroAPI on GitHub) | https://github.com/XeroAPI | Prompt Library last updated 7 Oct 2026; Agent Toolkit 8 Aug 2025 | 18 Nov 2026 |
| S58 | AI apps for bills and expenses | Xero App Store AU | https://apps.xero.com/au/collection/ai-apps-for-bills-expenses | No date shown | 18 Nov 2026 |
| S59 | Hubdoc home page | Hubdoc (a Xero company) | https://www.hubdoc.com/ | No date shown (© 2026) | 18 Nov 2026 |
| S60 | Xero Connector (the old address now redirects to the listing at S84) | Anthropic | https://claude.com/marketplace/connectors/xero | "Added April 2026" | 18 Nov 2026 |
| S61 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (18 Nov 2026) | 18 Nov 2026 |
| S62 | Claude for Small Business launches new workflows, integrations, and training programs | Anthropic | https://claude.com/resources/articles/claude-for-small-business-launches-new-workflows-integrations-and-training-programs | 15 Sep 2026 | 18 Nov 2026 |
| S63 | Small Business plugin | Anthropic | https://claude.com/marketplace/plugins/small-business | No date shown | 18 Nov 2026 |
| S64 | Is my data used for model training? | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | Updated 16 Mar 2026 | 18 Nov 2026 |
| S65 | Xero plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/xero/ | No date shown | 18 Nov 2026 |
| S66 | ChatGPT plugin listing: Xero | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_6a7ee05cee1881918dbfaba26fb555e1 | No date shown; version 1.0.3 | 18 Nov 2026 |
| S67 | Plugins in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001256-plugins-in-chatgpt | "Updated: yesterday" (17 Nov 2026) | 18 Nov 2026 |
| S68 | Plugins | OpenAI (ChatGPT docs) | https://learn.chatgpt.com/docs/plugins | No date shown | 18 Nov 2026 |
| S69 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/plan/microsoft-365-copilot-privacy | ms.date 9 Jul 2026 | 18 Nov 2026 |
| S70 | Agent installation in Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/manage/copilot-agent-install | ms.date 18 May 2026 | 18 Nov 2026 |
| S71 | Get more agents in the Microsoft 365 Copilot app | Microsoft Support | https://support.microsoft.com/en-us/topic/get-more-agents-in-the-microsoft-365-copilot-app-5986a0fb-ed6c-4eb7-82c0-e91e105276fb | No date shown | 18 Nov 2026 |
| S72 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 18 Nov 2026 |
| S73 | Use apps connected to Gemini with a work or school Google Account | Google Gemini Apps Help | https://support.google.com/gemini/answer/14959807?hl=en | No date shown | 18 Nov 2026 |
| S74 | Zapier (app listing) | Xero App Store AU | https://apps.xero.com/au/app/zapier | No date shown | 18 Nov 2026 |
| S75 | Make (app listing) | Xero App Store AU | https://apps.xero.com/au/app/make | No date shown | 18 Nov 2026 |
| S76 | About JAX (BETA), Australia | Xero Central | https://central.xero.com/0/article/About-Just-Ask-Xero-JAX-AU | No date shown (sitemap: 17 Aug 2026) | 18 Nov 2026 |
| S77 | About Budgets in Early access | Xero Central | https://central.xero.com/0/article/About-Budgets-in-Early-access | No date shown (sitemap: 9 Sep 2026) | 18 Nov 2026 |
| S78 | How JAX uses account types to calculate financial insights | Xero Central | https://central.xero.com/0/article/How-JAX-uses-account-types-to-calculate-financial-insights | No date shown (sitemap: 28 Apr 2026) | 18 Nov 2026 |
| S79 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: yesterday" (17 Nov 2026) | 18 Nov 2026 |
| S80 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: yesterday" (17 Nov 2026) | 18 Nov 2026 |
| S81 | Admin controls, security, and compliance for plugins and apps | OpenAI Help Center | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 13 days ago" (5 Nov 2026) | 18 Nov 2026 |
| S82 | Analytics pricing plans, Australia | Xero Central | https://central.xero.com/0/article/Analytics-powered-by-Syft-pricing-plans-AU | No date shown (sitemap: 4 Aug 2026) | 18 Nov 2026 |
| S83 | About short-term cash flow, Australia | Xero Central | https://central.xero.com/0/article/STCF-Cash-Predictions-AU | No date shown (sitemap: 29 Jul 2026) | 18 Nov 2026 |
| S84 | Xero (Claude's connector listing, read again) | Anthropic | https://claude.com/marketplace/connectors/xero | "Added April 2026" | 18 Nov 2026 |
| S85 | Get started with connectors | Anthropic (Claude docs) | https://claude.com/docs/connectors/getting-started | No date shown | 18 Nov 2026 |
| S86 | Use connectors to extend Claude's capabilities (read again) | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (18 Nov 2026) | 18 Nov 2026 |
| S87 | Claude (Xero connector in Claude, read again) | Xero | https://www.xero.com/au/ai-in-accounting/claude/ | No date shown (© 2026) | 18 Nov 2026 |
| S88 | Is my data used for model training? (read again) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | Updated 16 Mar 2026 | 18 Nov 2026 |
| S89 | Plans and pricing | Anthropic | https://claude.com/pricing | No date shown | 18 Nov 2026 |
| S90 | Connect Xero to Google Gemini | Xero Central | https://central.xero.com/0/article/Connect-Xero-to-Google-Gemini | No date shown (sitemap: 4 Nov 2026) | 18 Nov 2026 |
| S91 | Xero product releases (Australia) | Xero Central | https://central.xero.com/0/article/Xero-product-releases-AU | No date shown (sitemap: 13 Nov 2026); entries to November 2026 | 18 Nov 2026 |
| S92 | Build your budget from actuals you already trust in Xero | Xero Blog | https://blog.xero.com/product-updates/new-budgets/ | 11 Nov 2026 | 18 Nov 2026 |
| S93 | Xforce by Xero: Forward-Deployed Engineers & Partner Consultants to Help Accountants Put AI to Work | Xero (media release) | https://www.xero.com/au/media-releases/xforce-by-xero-forward-deployed-engineers-partner-consultants-help-accountants-put-ai-to-work/ | 12 Nov 2026 | 18 Nov 2026 |
| S94 | Xero in Microsoft 365 Copilot | Xero | https://www.xero.com/au/ai-in-accounting/copilot/ | No date shown (© 2026) | 18 Nov 2026 |
| S95 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654 | No date shown | 18 Nov 2026 |
| S96 | Request documents from clients with JAX (BETA) | Xero Central | https://central.xero.com/0/article/Request-documents-with-JAX-in-Books-health | No date shown (sitemap: 1 Nov 2026) | 18 Nov 2026 |
| S97 | JAX product releases (BETA) | Xero Central | https://central.xero.com/0/article/Release-notes-for-Just-Ask-Xero-JAX | "Last updated on 13 October 2026" | 18 Nov 2026 |
