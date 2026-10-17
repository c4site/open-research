# LEAP: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- LEAP's AI is built into the practice management software. Matter AI answers questions from the documents, emails and notes saved in a matter. LawY does legal research and can send an answer to a lawyer to check. [S2] [S3]
- LEAP says Matter AI, LawY, AI Prompts, Generator and AutoTime come with every LEAP subscription at no extra cost. AI Paralegal is the exception: it bills its work to your clients and LEAP takes a cut. [S1] [S5]
- Matter AI lets you choose the model for each task. LEAP's help centre lists two GPT 5.4 models and two Claude 4.6 models. [S34]
- LEAP stores Australian firms' data in AWS Sydney. When Matter AI is used, LEAP's Trust Center says relevant matter data goes to its supplier Corto's infrastructure in the United States for processing. [S9] [S12]
- LEAP's contract says it won't use your matter data to train or improve its AI services. Its security page says client data isn't used to train third-party foundation models without your explicit consent. [S14] [S9]
- LEAP's help centre says you can't switch LawY or Matter AI off for a particular user. [S35]
- We found no official connection between LEAP and ChatGPT, Claude, Microsoft Copilot or Google Gemini. [S54] [S56] [S58] [S61]
- LawY has its own connector for Claude and ChatGPT. It needs a paid LawY account, and nothing we read says it reaches the matters in LEAP. [S26]
- LEAP documents a Zapier integration that can create records in LEAP, and offers an API through its developer console. Its terms otherwise ban automated access to LEAP. [S45] [S51] [S14]

## The tool, and the plans that matter

LEAP is legal practice management software from an Australian company founded in Sydney in 1992. It covers matters, documents, email, time recording, billing and trust accounting in one system. [S13]

LEAP's page written for AI assistants says it's for Australian law firms and conveyancing practices with 1 to 300 users, from sole practitioners to the smaller end of enterprise. [S13]

LEAP doesn't publish prices. It's sold per user per month for a set term, and LEAP says pricing depends on firm size, jurisdiction and requirements. [S13]

| Product | Who it's for | AI included | Price |
|---|---|---|---|
| LEAP | Small and mid-sized firms | Matter AI, LawY, AI Prompts, Generator and AutoTime, at no extra cost | Not published; per user per month |
| LEAP Enterprise | Mid-sized and larger firms | The same legal AI, plus an Open API and integrations including Zapier | Not published |
| AI Paralegal (family law) | Firms that bill its work to clients | Sources and files disclosure documents, drafts first documents | Revenue share or a cost per item, depending on billing basis |
| LawY on its own (outside LEAP) | Anyone who buys it directly | Full LawY suite, including its own connector for Claude and ChatGPT | $89 per user per month plus local tax |

Sources for the table: [S1] [S13] [S50] [S5] [S43] [S22] [S26]

- LEAP Enterprise is LEAP configured for mid-sized and larger firms. LEAP says it combines enterprise accounting with "the innovative productivity tools and Legal AI already trusted in LEAP practice management". [S13] [S66]
- LawY says LEAP users get LawY's research feature with their LEAP subscription. LawY's pricing page sells the full suite as a separate subscription. [S25] [S22]
- LawY's pricing page doesn't say which currency the $89 is in. [S22]

## AI built in

### Matter AI

**What it does**

- Reads the documents, emails and attachments saved in a LEAP matter, including scanned PDFs and handwritten notes, and answers questions with references to the files it used. [S2] [S34]
- Summarises documents or folders, compares documents for inconsistencies, drafts emails and documents, and answers questions about the matter's financial transactions. [S2] [S34]
- Turns an answer into a first draft in Word, PDF, Excel or PowerPoint and saves it to the matter. [S2]
- The All tab combines matter facts with LawY legal research and shows its reasoning step by step. [S2] [S34]
- Matter Summary builds a summary of the whole matter with inline references, and adds a chronology for some matter types. [S37]
- Matter AI chat can send a response to Word or Outlook. [S34]

**Where to find it**

- Open a matter, go to the **Details & Correspondence** tab and click **Matter AI Chat** in the **LEAP AI** ribbon. [S34]
- You can also right-click a document and choose **Matter AI - New Document Chat** (on the web: **LEAP AI > Matter AI - New Document Chat**). [S34]
- Pick the model from the dropdown below **Ask me anything**: **GPT 5.4 - Instant**, **GPT 5.4 - Thinking**, **Claude 4.6 Sonnet** or **Claude 4.6 Opus**. [S34]
- **Document Status** shows which documents have loaded, failed or been excluded. You can exclude a document from future answers. [S2] [S34]

**Which plans have it**

- Included in every LEAP subscription at no extra cost, including Matter AI for Word and the model selector. [S2]
- Corto's terms for Matter AI say Corto "retains the right to charge fees" and would tell you first. [S18]

**What happens to your data**

- LEAP's terms list "Matter AI powered by Corto" as a third-party product, with its own terms shown in the Matter AI window. [S15]
- LEAP's legal page names "Corto Matter AI" among the suppliers whose terms apply on top of LEAP's own. [S17]
- Corto's published Matter AI terms, current from 20 March 2026, say it "uses third-party artificial intelligence services, including OpenAI's large-scale language-generation model and others". [S18]
- The first time someone uses Matter AI or Matter Summary, the firm has to accept Corto's terms and privacy policy. [S37]
- LEAP's Trust Center says matter data stays in your regional AWS location, but "When Matter AI is used, relevant matter data is sent to Corto's infrastructure in the United States for processing". [S12]
- Corto's security page says it's hosted on AWS in the Oregon region (us-west-2). It says client data isn't used to train or tune AI models. [S20]
- LEAP's Word add-in article says the first time you use Matter AI "it will ingest the documents within all your LEAP matters". [S36]
- Matter AI chat history is visible only to the person who wrote it. Colleagues opening the same matter can't see it. [S34]
- Feedback you give with the thumbs buttons is reviewed by LEAP's team. [S34]

**In Australia**

- Described on LEAP's Australian site and in its Australian help centre. [S2] [S34]
- The processing location for Matter AI is the United States, per LEAP's Trust Center. [S12]

### LawY (legal research, with lawyer verification)

**What it does**

- Answers legal questions with numbered citations to case law and legislation, tailored to the jurisdiction and matter type. [S3] [S35]
- Drafts letters, precedent orders and court documents, and can summarise, translate or remove personal information from text. [S3] [S35]
- **Deep Research** gives a longer analysis. You can apply the matter's facts or send it to a lawyer to verify. [S35]
- **Automatic Deep Research** re-checks your questions in the background and emails a memo, filed to the matter, when the deeper research changes or adds to the answer. [S3] [S30]
- Verification goes to a panel of 300+ Australian lawyers with at least five years' post-qualification experience. LEAP says most are returned in one to three business days. [S3]

**Where to find it**

- In a matter, go to **Details & Correspondence** and select **LawY** in the **LEAP AI** ribbon. [S35]
- In a browser, go to app.lawy.ai, select **Sign in**, then **Sign in with LEAP**, choose your region and use your LEAP login. [S35] [S27]
- The first time you open it, you may be asked to consent to permissions: **Allow as admin** for the whole firm, or **Allow** for yourself only. [S35]
- To turn off Automatic Deep Research, open the LawY settings, go to **Preferences** and switch it off. It's on by default. [S35]
- LawY isn't available in the LEAP mobile app. [S35]

**Which plans have it**

- Included in all LEAP subscriptions at no extra cost, including verification. [S35] [S3]
- Verification is only offered on Deep Research answers. [S35]
- Some LawY features are only for standalone LawY subscribers. Attaching matter documents in Research is one. [S31]

**What happens to your data**

- LEAP says LawY doesn't extract information from your matters. You decide what to share. [S3]
- LEAP's Trust Center says LawY is "powered by sub-processor Corto". [S12]
- LawY's security page says it uses models from OpenAI and Google Gemini under zero data retention arrangements, and that prompts are scrubbed of personal information. [S21] [S29]
- LawY's security page also says "LawY does not use your conversations or documents to train AI models". Its About page says the same of your questions. [S21] [S33]
- LawY's terms, though, let LawY and its providers use your inputs and outputs "to develop and improve the services", including "the design, training and development process for machine learning models". [S23]
- Only verified answers are added to LawY's knowledge base, with personal details replaced by placeholders. [S3] [S35]
- LawY's privacy policy says your name and queries are visible to other people in your firm who use LawY through the firm's LEAP account. [S24]
- LawY doesn't currently let you delete or clear conversation history. [S35]
- LawY says its service is hosted and operated in Australia, Canada, the United States, the United Kingdom and New Zealand. [S24]

**In Australia**

- LEAP's help centre says LawY covers all matter types and all jurisdictions in Australia. [S35] [S28]
- Automatic Deep Research launched first for LEAP Australia users on Australian matter types. [S30]

### AI Prompts, Matter AI for Word and Generator

**What it does**

- AI Prompts are lawyer-written instructions that draft documents such as affidavits, statutory declarations and briefs to counsel from the matter's contents. LEAP says there are over 200. [S2] [S36]
- Matter AI for Word is a Word add-in with a chat mode and a prompt mode. [S36]
- Generator finds and drafts documents from your precedents, past correspondence, By Lawyers precedents and LawY answers. [S41]

**Where to find it**

- In a matter, click **Forms & Precedents**, then search the **Browse** tab for "prompt". Prompts open in Word with the add-in on the right. [S4] [S36]
- If the add-in is missing, in Word go to **File > Account > Get Add-ins**, search for **Matter AI** and click **Add**. [S36]
- Generator sits in the **Generator** tab of **Forms & Precedents**, or under **LEAP AI** in the Actions pane on the web. [S41]
- Microsoft's Marketplace lists the Matter AI add-in from LEAP Legal Software. It "Can read and make changes to your document" and "Can send data over the Internet". [S53]

**Which plans have it**

- No extra fee. Prompts and Matter AI are part of the LEAP subscription. [S36]
- Prompts are only available for certain matter types. [S36]

**What happens to your data**

- The first time you use Generator, you choose whether to include matter context, which may include personal information. You can change this in the settings cog. [S41]
- The Word add-in article says Matter AI "does not yet read audio, visual, or video files". [S36]

**In Australia**

- Described in LEAP's Australian help centre. [S36]

### Pathways (next-step suggestions, tasks and an agent)

**What it does**

- Reads a matter's fields, cards, critical dates, tasks and fees, then suggests prioritised next steps with a completion estimate. [S38] [S7]
- Pathways Tasks gives a board of tasks across all matters. Firm admins get a whole-firm view. [S38]
- Pathways Agent can draft documents, do research and prepare file notes. [S38]

**Where to find it**

- Open a matter, go to **Details & Correspondence** and click **Pathways** in the **LEAP AI** section of the ribbon. [S38]
- For each suggestion you choose **Add**, **Mark as Done** or **Dismiss**. [S38]
- Each person can turn **Enable Pathways Agent** on or off in **My Settings**. Firm settings need LEAP Firm Admin access. [S38]

**Which plans have it**

- LEAP's Pathways page and help article don't mention any extra charge. [S7] [S38]

**What happens to your data**

- When enough users dismiss the same suggestion for the same reason, LEAP updates the underlying guide "as more firms use Pathways". [S38]

**In Australia**

- LEAP says Pathways covers all matter types in every jurisdiction and applies state and territory requirements. [S7]

### LEAP Risk and Matter Issues

- **What it does:** LEAP Risk lists risks typical for the matter type and uses Matter AI to summarise the evidence for and against each one. Matter Issues ranks issues in a family law file and suggests actions. [S40] [S39]
- **Where to find it:** The **LEAP Risk** icon in the **LEAP AI** tab, and **Matter Issues** in the LEAP ribbon. [S40] [S39]
- **Which plans have it:** LEAP Risk is switched on automatically for certain family law, estates, property and personal injury matter types. Matter Issues covers seven family law matter types. [S40] [S39]
- **What happens to your data:** Both run through Matter AI, so the Matter AI data handling above applies. That's our inference from how LEAP describes them. [S40] [S39]
- **In Australia:** Both are described in LEAP's Australian help centre. [S40] [S39]

### AI Paralegal (family law)

**What it does**

- Names, files and indexes financial disclosure documents, and drafts the financial disclosure schedule, balance sheet and Application for Consent Orders. [S5]
- Contacts your client by text message and email with a secure link, works through each category of document with them, and chases missing items for about four weeks. [S42]
- Can share disclosure with the other side by secure link. Anyone at the other firm with the same email domain can open it once they have the link. [S42]

**Where to find it**

- Click **AI Paralegal** in the matter ribbon. Firm settings sit under **LEAP Main Menu > Settings > Apps > AI Paralegal Settings**. [S42] [S43]

**Which plans have it**

- LEAP's product page says your firm keeps 70% of the revenue the AI Paralegal generates and LEAP receives 30%. [S5]
- The billing article says time-based work is billed at a charge-out rate you set, and the **Cost to you** screen shows LEAP's cost per item. [S43]
- None of the pages we read publish the per-item costs. [S5] [S43]

**What happens to your data**

- Tax returns and notices of assessment are obtained "through our specialist accounting firm". [S42]
- Every view of a shared link is logged with the viewer's email address and time. [S42]

**In Australia**

- Available on family law matter types. [S42]

### AutoTime and Ruffle

- **AutoTime** records time spent drafting, emailing and on calendar work in the background. LEAP's Outlook page calls it AI-powered time recording. [S6] [S8]
- **Ruffle** extracts transactions from bank statements for family law work. When a merchant isn't in its database, it "use[s] AI to attempt categorisation". [S44]
- Ruffle's help article says AI processing runs on a "no retention" basis and the output isn't used for training. [S44]
- LEAP reports that in its testing 98% of transactions were extracted without error and 0.2% had a wrong amount. [S44]
- Both are included in the LEAP subscription. [S1] [S44]

### AI apps in the LEAP Marketplace

- The Australian LEAP Marketplace listed 48 apps on 17 October 2026. [S48]
- AI-related apps include **Chronology**, **LEAP Chronology**, **LitigationMap** (which suggests court orders using Matter AI) and **Court Forms +** (which has an AI chat). [S48]
- Third-party listings include **AI Paralegal Conveyancing** by InfoTrack and **Settify Connect**, which describes using AI to gather client details. [S48]
- None of the listings name ChatGPT, Claude, Copilot or Gemini. [S48]

## Outside AI that connects

In plain words, a connector lets a chat assistant such as Claude or ChatGPT look things up in another app, and sometimes make changes there. Anthropic lists each one in its Connectors directory with a Verified or Community label. [S55]

LEAP's own AI uses OpenAI and Anthropic models inside LEAP. Using them doesn't link LEAP to your own ChatGPT or Claude account. [S2] [S34]

### Claude and LEAP

**Official?**

- No official connection found. LEAP isn't among the connectors on Anthropic's public directory page. [S54]
- A search of LEAP's Australian help centre for "Claude" found only articles about Matter AI's model choices. [S64] [S34]

**What it can see and do**

- Nothing official. [S54]
- LawY's separate connector can reach matters and documents held in a paid LawY account. See "LawY's own connector" below. [S26]

**What you need, steps, disconnecting**

- Not applicable. [S54]

**Limits**

- LEAP's terms say you must not use LEAP "via mechanical, programmatic, robotic, scripted or any other automated means" or scrape it, except as the agreement expressly permits. [S14]
- Our reading: that rules out home-made connectors and AI browser agents working in LEAP. This isn't legal advice.

### ChatGPT and LEAP

**Official?**

- No official connection found. LEAP isn't on OpenAI's public plugin page, including its Legal category. [S56]

**What it can see and do**

- Nothing official. [S56]

**What you need, steps, disconnecting**

- Not applicable. [S56]

**Limits**

- Matter AI's GPT models run inside LEAP under Corto's terms. Using them doesn't connect your own ChatGPT account. [S18] [S34]
- The automated-access ban in LEAP's terms applies here too. [S14]

### Microsoft Copilot and LEAP

**Official?**

- No official connection found. LEAP isn't among Microsoft's federated Copilot connectors, last updated 16 October 2026. [S58]
- A search of LEAP's Australian help centre for "Copilot" returned no results. [S47]

**What LEAP does offer in Microsoft 365**

- LEAP for Outlook, LEAP for Word and the Matter AI add-in are listed on Microsoft's Marketplace. None of LEAP's listings is a Copilot agent. [S65] [S53]
- Linking your Microsoft 365 account with LEAP lets you share invoices from your own work email and manage appointments and tasks. [S8]
- The LEAP Connector for Power BI reads LEAP data through LEAP's API gateway. It needs a LEAP Admin account and a Power BI Pro or Premium licence. [S46]

**Limits**

- Microsoft's connector list includes "Leap (Independent Publisher)". It belongs to an image and music generator at tryleap.ai, which has nothing to do with LEAP Legal Software. [S59] [S60]

### Google Gemini and LEAP

**Official?**

- No official connection found. LEAP isn't on Google's list of Connected Apps for Gemini. [S61]

**What it can see and do**

- Nothing official. [S61]

**Limits**

- LawY uses Google Gemini models behind the scenes. That's inside LawY, and it isn't a connection to your Gemini app. [S21]

### LawY's own connector (a separate LawY subscription)

**Official?**

- Yes, for LawY. LawY's help centre describes "LawY Connected Agents", a connector that links "your firm's matters and documents" in LawY to agents such as ChatGPT and Claude. [S26]
- We didn't find LawY on Anthropic's or OpenAI's public directory pages, though LawY's article says to find it there. [S54] [S56] [S26]

**What it can see and do**

- Lists matters, searches and reads documents, creates new documents and updates existing ones. It can also create folders and move documents if your access allows. [S26]
- It "cannot delete anything". Updates are refused if the document changed since the agent read it. [S26]
- Every action is recorded in the **Activity log** in LawY's **Connected Agents** panel. [S26]

**What you need**

- A paid LawY account with Connected Agents switched on, and access set up by a LawY Firm Administrator. [S26]
- A Claude or ChatGPT account. [S26]
- Nothing we read says this connector reaches matters stored in LEAP. LawY's LEAP integration is described as research only. [S22] [S25]

**Steps to connect** (LawY help centre, updated 15 October 2026)

1. In Claude, go to **Settings → Connectors** (or browse the connector directory) and find **LawY**. Anthropic's own page now calls this **Customize > Connectors**. [S26] [S55]
2. Choose **Connect** and sign in to LawY in the browser window that opens. [S26]
3. Approve the connection, then try "List my LawY matters." [S26]
4. In ChatGPT, LawY's article says to open **Settings → Apps & Connectors**. OpenAI's current help page uses **Settings > Plugins**. [S26] [S57]

**To disconnect**

- In LawY's **Connected Agents** panel, which suspends access straight away, or in the AI app's connector settings. [S26]
- A firm administrator can block the connector for the whole firm. [S26]

**Limits**

- When it's switched on, "all matters and operations are enabled by default". Administrators can then restrict matters, documents and operations. [S26]

### Zapier and LEAP (actions only)

**Official?**

- Yes. LEAP's help centre documents the **LEAP (Legal)** app in Zapier. [S45]
- LEAP Enterprise's integrations page also names Zapier. [S50]

**What it can see and do**

- Actions only: **Search Matter**, **Create Matter**, **Search Card**, **Create Card**, **Create Comment**, **Create Time Entry**, **Create Fee** and **Create Cost Recovery (Expense)**. [S45]
- "LEAP doesn't support Triggers just yet", so a Zap has to start in another app. [S45]
- Zapier's own page offers LEAP (Legal) through Zapier MCP, which lets AI tools that support MCP run those actions. [S62]

**What you need**

- A Zapier account and a LEAP login. LEAP recommends turning on multi-factor authentication for your Zapier account. [S45]
- Zapier says each MCP tool call uses two tasks from your Zapier plan. [S62]

**Steps to connect** (LEAP help centre, 18 February 2026)

1. Log in to Zapier and select **App Connections** from the Home page. [S45]
2. Select **Add Connections** and search for **LEAP (Legal)**. [S45]
3. Select it, then **Add Connection**, and enter your LEAP credentials. [S45]
4. Confirm the permissions window. [S45]
5. Build a Zap with a trigger from another app, then add a LEAP action. [S45]

**To disconnect**

- LEAP's article doesn't describe disconnecting. It covers reconnecting from **App Connections** in Zapier. [S45]

**Limits**

- LEAP sends a notification to the staff member each time a Zapier create action runs. [S45]
- LEAP's article doesn't mention AI or MCP. Running LEAP actions from an AI tool through Zapier MCP is Zapier's route, and LEAP hasn't documented it. [S45] [S62]

### LEAP's API and Developer Console

- LEAP's developer site offers REST APIs for apps that integrate with LEAP on desktop, web and mobile, through a developer program. [S51]
- LEAP Enterprise describes an Open API for connecting your own tools and building custom apps. [S50]
- The Power BI connector uses LEAP's API gateway. [S46]
- We couldn't read the API reference itself. Its pages showed only the site menu when we opened them without signing in. [S51]
- We found no LEAP MCP server. [S51] [S54]

## Jobs it's good for

- **Getting across a new file.** Open Matter Summary for an overview with references and a chronology, then ask Matter AI follow-up questions. [S37] [S34]
- **Spotting what doesn't match.** Select several documents and ask Matter AI to compare them for inconsistencies. [S34]
- **First drafts from the file.** Run an AI Prompt for an affidavit or brief to counsel, then refine it in Word with Matter AI for Word. [S36]
- **A research question you want checked.** Ask LawY, request Deep Research, and choose lawyer verification at no extra cost. [S35]
- **Keeping a matter moving.** Use Pathways suggestions and turn the useful ones into tasks. [S38]
- **Family law financial disclosure.** Run bank statements through Ruffle, or have the AI Paralegal source and file documents, checking the costs first. [S44] [S42] [S43]
- **Feeding enquiries into LEAP.** Use Zapier to create a card or matter from a form or spreadsheet. [S45]
- **Firm reporting.** Connect Power BI to LEAP data. [S46]

## What to watch for

**Data leaves Australia when Matter AI runs**

- LEAP stores Australian firms' data in AWS Sydney, but its Trust Center says Matter AI sends relevant matter data to Corto in the United States. [S9] [S12]
- The Word add-in article says Matter AI ingests documents in all your matters the first time it's used. Taken together, documents across your matters may be processed in the US once anyone uses Matter AI. That's our inference. [S36] [S12]
- LEAP's public sub-processor list names AWS, Salesforce, Snowflake, Vanta and Sumo Logic. It doesn't name Corto or the AI model makers. [S11]
- LEAP's security page says a sub-processor register is available for due diligence. [S9]

**Training: the promises and the fine print**

- LEAP's terms say it won't use matter data to improve or train its AI services. [S14]
- LEAP's security page adds "without your explicit consent" to its no-training promise for third-party foundation models. [S9]
- LawY's security page and its terms disagree about whether inputs can be used to train models. [S21] [S23]

**Who can switch it off, and who can see it**

- You can't turn LawY or Matter AI off for individual users. [S35]
- Matter AI chats are private to the user. LawY queries may be visible to colleagues who use LawY through the firm's LEAP account. [S34] [S24]
- LawY conversation history can't currently be deleted. [S35]

**Confidential details in research questions**

- LEAP recommends removing personally identifiable information before sending a LawY question for verification. Verifiers are bound by confidentiality and conflict rules. [S1]
- LawY's terms say any personal information you include is at your own discretion and risk. [S23]

**AI Paralegal talks to your client**

- It messages clients directly by SMS and email, and reminds them for about four weeks. [S42]
- Its shared links open for anyone at the other firm's email domain. [S42]

**Check the work**

- LEAP's terms say its AI services aren't legal advice and a qualified lawyer should review the output before it's relied on. [S14]
- Corto's terms say outputs haven't been reviewed for legal accuracy, and that you agree to check them before using them in any legal advice. [S18]

**Home-made connections**

- LEAP's terms ban automated and programmatic access and scraping, except as the agreement allows. [S14]
- Corto's terms say Matter AI must not be accessed other than through the LEAP product. [S18]
- A Microsoft connector called "Leap" belongs to an unrelated company. [S60]

**Beta features**

- LEAP's product terms say beta features are provided "as is" and used at your own risk, and LEAP can stop them at any time. [S16]

**AI assistants describing LEAP**

- LEAP publishes a page "for AI assistants and answer engines" that tells them how to describe LEAP and not to quote prices from third-party sites. Answers you get from ChatGPT or Claude about LEAP may repeat LEAP's own framing. That last point is our inference. [S13]

## Announced changes

- **1 August 2026 (new clients) and 1 September 2026 (existing clients):** New LEAP General Terms took effect, including clause 9 on AI services. [S14]
- **20 March 2026:** Corto's current Matter AI terms took effect. [S18]
- **Pathways:** Automatic sync configuration "is currently in development and will be available in a future release". [S38]
- **Zapier:** "Support for Triggers is on our roadmap." [S45]
- **Prompts:** LEAP says future versions "may offer integration" between Prompts and standard precedents. [S36]
- **LawY:** Automatic Deep Research "is rolling out in stages". [S30]
- **Security:** LEAP says ISO/IEC 27001 certification is in progress, and SOC 2 Type 1 coverage is being extended to more products during 2026. [S9] [S10]
- **LawY's own assurance:** In a 2025 update, LawY said it was working towards SOC 2 Type 1 and then Type 2. [S32]
- **History:** LEAP's innovations page dates LawY in LEAP to February 2024, Matter AI to March 2024, Generator to August 2024 and AI Prompts to October 2024. [S49]

## What we couldn't establish

- **LEAP's prices.** LEAP doesn't publish them. [S13]
- **The Matter AI terms shown in the product.** LEAP's terms point to terms at the bottom of the Chat History window. We read Corto's public copy and couldn't confirm it's identical. [S15] [S18]
- **Where LawY's processing happens for LEAP users.** LEAP says LawY is powered by Corto, and Corto hosts in the US, but LawY lists five countries. [S12] [S20] [S24]
- **Which LawY training statement applies.** LawY's security page and terms conflict. [S21] [S23]
- **Whether LawY's connector can reach LEAP matters.** Nothing we read says it can. [S26]
- **How much of a matter LawY reads.** LEAP says LawY doesn't extract information from your matters. LawY's post on Automatic Deep Research says it draws on "the documents and details in your own matter files". [S3] [S30]
- **LawY in the AI directories.** LawY's article says to find it in Claude's directory, but it wasn't on the public pages we read. [S26] [S54] [S56]
- **LawY's coverage in LEAP.** LEAP's help says all matter types in Australia, while LEAP's legal AI page labels it "included at no extra cost for select matter types". [S35] [S1]
- **Pathways suggestions.** The help article says up to 9 per matter; LEAP's feature page says up to 10. [S38] [S7]
- **Who Corto is.** LEAP's family law page calls its AI "developed in-house". Corto's privacy policy includes LEAP North America Pty Ltd in its definition of Corto and links to LEAP's list of affiliates, which suggests Corto is in the LEAP group. That's our inference. [S52] [S19]
- **AI Paralegal's per-item costs.** Not published on the pages we read. [S43]
- **Pages we couldn't read.** LEAP's Australian Information Security Policy and Privacy Policy pages showed an error. LawY's and Corto's trust centres blocked automated reading. LEAP's API reference showed no content without a sign-in. [S51]
- **Who built Zapier's LEAP (Legal) app.** LEAP documents it, but Zapier's page doesn't say who maintains it. [S45] [S63]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Legal AI for Australian Law Firms | LEAP | https://www.leaplegalsoftware.com/au/features/legal-ai/ | No date shown | 17 Oct 2026 |
| S2 | Matter AI: Legal AI Assistant for Law Firms | LEAP | https://www.leaplegalsoftware.com/au/features/matterai/ | No date shown | 17 Oct 2026 |
| S3 | LawY: AI Legal Assistant Verified by Lawyers | LEAP | https://www.leaplegalsoftware.com/au/features/integrations/lawy/ | No date shown | 17 Oct 2026 |
| S4 | AI Document Drafting for Law Firms | LEAP | https://www.leaplegalsoftware.com/au/features/ai-document-drafting/ | No date shown | 17 Oct 2026 |
| S5 | AI Paralegal | LEAP | https://www.leaplegalsoftware.com/au/features/ai-paralegal/ | No date shown | 17 Oct 2026 |
| S6 | AutoTime (Matter Activity Recording) | LEAP | https://www.leaplegalsoftware.com/au/features/autotime/ | No date shown | 17 Oct 2026 |
| S7 | Pathways | LEAP | https://www.leaplegalsoftware.com/au/features/pathways/ | No date shown | 17 Oct 2026 |
| S8 | Microsoft Outlook integration and LEAP | LEAP | https://www.leaplegalsoftware.com/au/features/integrations/outlook-365/ | No date shown | 17 Oct 2026 |
| S9 | Security | LEAP | https://www.leaplegalsoftware.com/au/security-2/ | No date shown | 17 Oct 2026 |
| S10 | LEAP Trust Center (overview) | LEAP | https://trust.leaplegalsoftware.com/ | No date shown; latest update posted 22 Jun 2026 | 17 Oct 2026 |
| S11 | LEAP Trust Center: Subprocessors | LEAP | https://trust.leaplegalsoftware.com/subprocessors | No date shown | 17 Oct 2026 |
| S12 | LEAP Trust Center: FAQ | LEAP | https://trust.leaplegalsoftware.com/faq | No date shown | 17 Oct 2026 |
| S13 | Official AI information about LEAP (a page written for AI assistants) | LEAP | https://www.leaplegalsoftware.com/au/ai-info/ | "Last updated: August 2026" | 17 Oct 2026 |
| S14 | LEAP General Terms (PDF) | LEAP | https://a.storyblok.com/f/126141/x/04113e8bd3/leap-global-terms-general-terms.pdf | Current from 1 Aug 2026 (new clients) and 1 Sep 2026 (existing clients) | 17 Oct 2026 |
| S15 | LEAP Third Party Terms (PDF) | LEAP | https://a.storyblok.com/f/126141/x/34ae2f3d96/leap-global-terms-third-party-terms.pdf | Current from 1 Aug 2026 (new clients) and 1 Sep 2026 (existing clients) | 17 Oct 2026 |
| S16 | LEAP Product Terms (PDF) | LEAP | https://a.storyblok.com/f/126141/x/a89a201395/leap-global-terms-product-terms.pdf | Current from 1 Aug 2026 (new clients) and 1 Sep 2026 (existing clients) | 17 Oct 2026 |
| S17 | Legal (LEAP contracts and policies) | LEAP | https://www.leaplegalsoftware.com/legal/ | Terms shown as "Current from 1 August 2026" | 17 Oct 2026 |
| S18 | Matter AI Terms and Conditions | Corto (LEAP's Matter AI supplier) | https://cdn.cortoaws.com/documents/leap-ai-terms.html | "Current as and from 20 March 2026" | 17 Oct 2026 |
| S19 | Privacy Policy | Corto | https://cdn.cortoaws.com/documents/privacy.html | "Effective date: April 4, 2024" | 17 Oct 2026 |
| S20 | Security | Corto | https://www.docorto.ai/security | No date shown | 17 Oct 2026 |
| S21 | Security | LawY | https://www.lawy.ai/security | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S22 | Pricing | LawY | https://www.lawy.ai/pricing | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S23 | Terms and Conditions | LawY | https://www.lawy.ai/terms-and-conditions | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S24 | Privacy Policy | LawY | https://www.lawy.ai/privacy-policy | No date shown (sitemap 7 May 2026) | 17 Oct 2026 |
| S25 | Meet LawY in LEAP | LawY | https://www.lawy.ai/integration/leap | No date shown (sitemap 18 Aug 2026) | 17 Oct 2026 |
| S26 | LawY Connected Agents | LawY Help Centre | https://help.lawy.ai/en/articles/17607791-lawy-connected-agents | "Updated this week" (15 Oct 2026, page data) | 17 Oct 2026 |
| S27 | How to sign into LawY through an integration partner | LawY Help Centre | https://help.lawy.ai/en/articles/15201103-how-to-sign-into-lawy-through-an-integration-partner | 22 Jun 2026 | 17 Oct 2026 |
| S28 | Where is LawY available? | LawY Help Centre | https://help.lawy.ai/en/articles/15077011-where-is-lawy-available | 22 Jun 2026 | 17 Oct 2026 |
| S29 | LawY FAQ's Security | LawY Help Centre | https://help.lawy.ai/en/articles/13933066-lawy-faq-s-security | "Updated yesterday" (15 Oct 2026, page data) | 17 Oct 2026 |
| S30 | Introducing Automatic Deep Research | LawY Blog | https://www.lawy.ai/blog/introducing-automatic-deep-research | No date shown (sitemap 2 Jul 2026) | 17 Oct 2026 |
| S31 | Latest in LawY: March 2026 | LawY Blog | https://www.lawy.ai/blog/latest-in-lawy-march-2026 | No date shown (sitemap 29 Jun 2026) | 17 Oct 2026 |
| S32 | Latest in LawY: 3 updates and enhancements | LawY Blog | https://www.lawy.ai/blog/nov25-new | No date shown (sitemap 28 Jan 2026) | 17 Oct 2026 |
| S33 | About LawY | LawY | https://www.lawy.ai/about | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S34 | Matter AI | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Matter-AI-AU | 24/07/2026 | 17 Oct 2026 |
| S35 | LawY | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/LawY-AU | 01/09/2026 | 17 Oct 2026 |
| S36 | Matter AI for Word | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Matter-AI-for-Word-AU | 21/05/2026 | 17 Oct 2026 |
| S37 | Matter Summary | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Matter-Summary-AU | 04/08/2026 | 17 Oct 2026 |
| S38 | Pathways | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Pathways-AU | 27/07/2026 | 17 Oct 2026 |
| S39 | Matter Issues | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Matter-Issues-AU | 23/06/2026 | 17 Oct 2026 |
| S40 | LEAP Risk | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/LEAP-Risk-AU | 06/02/2026 | 17 Oct 2026 |
| S41 | Generator | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Generator-AU | 29/08/2025 | 17 Oct 2026 |
| S42 | AI Paralegal - Disclosure | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/AI-Paralegal-Disclosure-AU | 16/10/2026 | 17 Oct 2026 |
| S43 | AI Paralegal - Billing | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/AI-Paralegal-Billing-Settings-AU | 24/09/2026 | 17 Oct 2026 |
| S44 | Ruffle | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Ruffle-AU | 11/05/2026 | 17 Oct 2026 |
| S45 | Zapier Integration | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Zapier-Integration-AU | 18/02/2026 | 17 Oct 2026 |
| S46 | Installing Power BI & LEAP Connector | LEAP Help Centre (AU) | https://community.leap.com.au/s/article/Installing-Power-BI-LEAP-Connector-AU | 16/09/2024 | 17 Oct 2026 |
| S47 | Search results for "Copilot" | LEAP Help Centre (AU) | https://community.leap.com.au/s/global-search/Copilot | No date shown; no results returned | 17 Oct 2026 |
| S48 | Discover Apps for LEAP (Australia) | LEAP Marketplace | https://marketplace.leap.build/en-AU/apps | No date shown | 17 Oct 2026 |
| S49 | Innovations | LEAP | https://www.leaplegalsoftware.com/au/innovations/ | No date shown; entries dated Nov 2023 to Sep 2025 | 17 Oct 2026 |
| S50 | LEAP Enterprise: Customisable Legal Practice Platform | LEAP | https://www.leaplegalsoftware.com/au/leap-enterprise-apac/enterprise-integrations/ | No date shown | 17 Oct 2026 |
| S51 | Build Great Apps for LEAP | LEAP Developer | https://developer.leap.build/ | No date shown | 17 Oct 2026 |
| S52 | AI for Family Lawyers | LEAP | https://www.leaplegalsoftware.com/au/family-law/ai-for-family-lawyers/ | No date shown | 17 Oct 2026 |
| S53 | Matter AI (Word add-in listing) | Microsoft Marketplace | https://marketplace.microsoft.com/en-gb/product/WA200007438?tab=Overview | No date shown | 17 Oct 2026 |
| S54 | Connectors directory | Anthropic | https://claude.com/connectors | No date shown | 17 Oct 2026 |
| S55 | Get started with connectors | Anthropic | https://claude.com/docs/connectors/getting-started | No date shown (page metadata 25 Sep 2026) | 17 Oct 2026 |
| S56 | ChatGPT Plugins (including the Legal category) | OpenAI | https://openai.com/business/plugins/ | No date shown | 17 Oct 2026 |
| S57 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 8 hours ago" when read | 17 Oct 2026 |
| S58 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Updated 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S59 | List of all Copilot Studio, Power Platform and Logic Apps connectors | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/connector-reference/ | Updated 2 Oct 2026 (page metadata) | 17 Oct 2026 |
| S60 | Leap (Independent Publisher) (Preview) | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/leapaiip/ | Updated 25 Apr 2025 (page metadata) | 17 Oct 2026 |
| S61 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 17 Oct 2026 |
| S62 | LEAP (Legal) MCP | Zapier | https://zapier.com/mcp/leap-legal | No date shown | 17 Oct 2026 |
| S63 | LEAP (Legal) Integrations | Zapier | https://zapier.com/apps/leap-legal/integrations | No date shown | 17 Oct 2026 |
| S64 | Search results for "Claude" | LEAP Help Centre (AU) | https://community.leap.com.au/s/global-search/Claude | No date shown; only Matter AI model articles and spell-corrected "clause" results returned | 17 Oct 2026 |
| S65 | Search results for "Matter AI LEAP" | Microsoft Marketplace | https://marketplace.microsoft.com/en-gb/search/products?search=Matter%20AI%20LEAP | No date shown; listed LEAP for Outlook, Matter AI and LEAP for Word from LEAP Legal Software | 17 Oct 2026 |
| S66 | LEAP Enterprise features | LEAP | https://www.leaplegalsoftware.com/au/leap-enterprise-apac/leap-enterprise-features/ | No date shown | 17 Oct 2026 |
