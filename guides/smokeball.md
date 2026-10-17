# Smokeball: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Smokeball's AI is called Archie. It works inside a matter: it answers questions with links to the source documents, drafts letters and emails, reviews documents and suggests next steps. [S1] [S16]
- Archie is a paid add-on. Smokeball's Australian pricing page lists it on the Boost, Grow and Prosper+ plans, but doesn't show its price. [S2]
- Archie also works inside Microsoft Word and the new Outlook through Smokeball's own add-ins. [S12] [S19] [S21]
- You pick the model in Archie's settings. The list includes OpenAI GPT-5.x and Anthropic Claude models in Smokeball, and GPT-4.1 and Google Gemini 3.1 models in the Word add-in. [S15] [S19]
- Smokeball says Archie runs under zero-data-retention agreements and client data is never used to train AI. It says data stays in its home region "as a principle". [S14]
- Every user in the firm has Archie by default. A Firm Owner can switch it off for individual staff. [S16] [S18]
- LawY legal research, with optional checking by a lawyer, comes with the Archie add-on at no extra cost. [S10] [S26]
- We found no official connection between Smokeball and ChatGPT, Claude, Microsoft Copilot or Google Gemini. [S54] [S55] [S56] [S58]
- Smokeball documents a Zapier integration with triggers and actions, and API access for Prosper+ firms building their own apps. [S33] [S34]

## The tool, and the plans that matter

Smokeball is legal practice management software for law firms and conveyancers. Its Australian pricing page says it's trusted by more than 34,000 legal professionals worldwide. [S2]

Prices on Smokeball's Australian pricing page, as read on 17 October 2026. Smokeball says published prices exclude GST. [S2]

| Plan | Price (AUD, per user per month, excl. GST) | Archie AI | Other add-ons |
|---|---|---|---|
| Bill | From $59 | Not available ("No add-ons available") | None |
| Boost | From $129 | Add-on, price not shown | Intake $29 |
| Grow | From $249 | Add-on, price not shown | Intake $59, AutoTime $39 |
| Prosper+ | Custom price | Add-on, price not shown | Intake and AutoTime included |

Sources for the table: [S2]

- Boost is browser-based case management. Grow adds Smokeball's desktop app and is aimed at firms with three or more staff. [S2]
- Smokeball's free trial is for Boost. [S2]
- Smokeball's marketplace listing for Archie says it's "Available for" Grow and Prosper+, while the pricing page and help centre also offer it on Boost. [S48] [S2] [S17]
- Smokeball's terms say tiers apply to all users in a firm, and you can't move down a tier mid-term. [S5]

## AI built in

### Archie, the matter assistant

**What it does**

- Answers questions about a matter, citing the documents it used. [S1] [S16]
- Summarises documents and whole matters. It also compares documents for conflicting terms and drafts correspondence. [S1] [S16]
- Uses "agentic reasoning": it works through a request step by step and checks its own answer. [S16] [S12]
- Creates tasks, memos and calendar events when you ask, after you review and save them. [S23]
- Archie Suggestions offer next steps as tiles, refreshed every 24 hours. Smokeball says suggestions "are not executed automatically". [S24]
- Transcribes your spoken prompt if you use voice dictation. Smokeball says there's no background listening. [S12]

**Where to find it**

- Open a matter in the desktop app and select the **Archie** tab, or the Archie button in the right-hand panel. [S16]
- Settings sit under **Settings** in the bottom-left corner of the Archie screen. [S15]
- Choose a model under **Show AI model options**. The default is **OpenAI GPT-5.2**. Other options include **OpenAI GPT-5.5 (Thinking)**, **Claude Opus 4.8** and **Claude Sonnet 5**. [S15]
- Smokeball says every model offered "passed our privacy and security review" and doesn't "share, use, store or train on our users data". [S15]

**Which plans have it**

- The Archie add-on on Boost, Grow and Prosper+. [S2] [S17]
- Smokeball's June 2026 release notes for Bill and Boost list Archie updates for "Boost + Archie add-on" firms. [S60]
- New Archie features released in April 2026 came at no extra cost for firms that already had Archie. [S12]

**What happens to your data**

- When Archie is switched on, it indexes your firm's 50 most recent matters first. Other matters are read when you open them. [S16]
- Files over Archie's size limits are skipped when it reads a matter. Videos over 1 GB are one example. [S25]
- Archie can see firm details including every user's name and email address, matter parties, tasks, events, memos, invoices, and trust and operating account details. [S16]
- Smokeball says Archie works within one matter at a time and doesn't mix data across matters or firms. [S14] [S3]
- Smokeball says Archie runs under "enterprise agreements with a strict zero-data-retention policy" and client data is never used to train AI models, "neither Smokeball's nor any third party's". [S14]
- Colleagues can see the questions you've asked Archie on a matter. You can clear your own history but not other people's. [S16]
- Smokeball says authorised users can view a log of Archie questions for the matters they can access. [S14]
- In July 2025 Smokeball's chief technology officer said Archie used "a private instance of OpenAI's GPT 4o". The current settings page lists newer models from several companies. [S8] [S15]

**In Australia**

- Smokeball's help centre says, "As a principle, data stays in its home region - Australian data in Australia". [S14]
- Smokeball's privacy notice says its servers and group companies are in the UK, the US and Australia, and its service providers also operate in Japan. [S4]

### Archie in Microsoft Word, with Playbooks

**What it does**

- Drafts, edits and reviews documents in a Word sidebar, using the matter's context. Changes appear as Word tracked changes for you to accept or reject. [S19]
- **Playbooks** check a document against your firm's rules and flag issues, warnings and passes. Each playbook can hold up to 50 rules. [S20]
- A **Translate** app translates selected text or whole documents. [S19]

**Where to find it**

- In Word, select **Add-ins**, then **More add-ins**, open the **Store** tab, search for "Archie" and install the **Smokeball Archie** add-in. Log in with your Smokeball email, password and 2FA code. [S19]
- Playbooks sit under **Review** at the bottom of the Archie panel. [S20]
- Microsoft's Marketplace lists Smokeball Archie as free. It "Can read and make changes to your document" and "Can send data over the Internet". [S50]

**Which plans have it**

- Part of the Archie add-on. It arrived on 4 May 2026 for Grow and Prosper+ firms, and the Bill and Boost notes list it for Boost firms with Archie too. [S38] [S62]

**What happens to your data**

- The Word add-in uses a different set of models: **OpenAI GPT-4.1**, **Gemini 3.1 Flash** and **Gemini 3.1 Pro**. [S19]
- Changes save back to Smokeball differently depending on your plan and whether you use Word desktop or Word on the web. [S19]

**In Australia**

- Described in Smokeball's Australian help centre. [S19]

### Archie in Outlook

**What it does**

- Summarises email threads, suggests quick replies and drafts emails from the matter's dates, tasks and documents. [S11] [S21]
- Files emails and attachments to matters and creates Smokeball tasks from emails. [S11]

**Where to find it**

- In new Outlook or Outlook on the web, select **Apps**, then **Add apps**, search for "Smokeball for Outlook" and select **Add**. [S21]
- Open an email, select **Smokeball for Outlook**, confirm your country and click **Connect to Smokeball**. [S21]
- With the Archie add-on, use **Rapid Reply** or **Draft with Archie** in the Smokeball toolbar. [S21]

**Which plans have it**

- The new Outlook add-in supports Boost, Grow and Prosper+. Archie features need the Archie add-on. [S11] [S21]
- You need a paid Microsoft 365 Business or Education email account. [S11] [S21]

**What happens to your data**

- If you see "Admin approval required", your IT administrator has to allow Outlook add-ins in Microsoft 365. [S21]

**In Australia**

- Described in Smokeball's Australian help centre. [S21]

### LawY legal research inside Archie

**What it does**

- Answers questions of law tailored to the matter's practice area, with links to the resources it considered. [S26]
- **Deep Research** takes about an hour. **Deep Research + Verification** sends the findings to a qualified lawyer and takes about one to three business days. [S26]

**Where to find it**

- Open a matter, select the **Archie** tab, then **Legal Research** in the top-left corner. [S26] [S52]
- If you ask Archie a legal research question, it offers to use LawY instead. [S26]

**Which plans have it**

- Included with the Archie add-on at no extra cost since 13 November 2025, including verification. [S37] [S26] [S51]

**What happens to your data**

- Smokeball says your LawY conversations aren't used to train AI models. If you verify an answer, the verifier sees only the rephrased question, the AI answer and the matter facts you selected, with your name removed. [S10]
- LawY's own security page says it uses models from OpenAI and Google Gemini under zero data retention arrangements. [S53]
- LawY's terms cover use through practice management partners, and let LawY and its providers use inputs and outputs to improve their services, including training machine learning models. [S61]

**In Australia**

- Smokeball says LawY covers all practice areas and matter types across all states. [S26]

### Archie Apps

- **What it does:** Task-specific AI tools inside Archie. The Australian list includes **Bank Statements Analyser**, **Legal Chronology**, **NSW AI Contract Review by InfoTrack** and **Audio Transcription**. [S27] [S9] [S28]
- **Where to find it:** In a matter, select the **Archie** tab, then **Apps**. Each app shows whether Smokeball or a third party such as InfoTrack made it. [S27]
- **Which plans have it:** Audio Transcription is included in the Archie add-on. [S28]
- **What happens to your data:** Audio and video up to 1 GB can be transcribed, and the transcript can be saved to the matter. [S28]
- **In Australia:** The InfoTrack app analyses NSW residential contracts. [S9]

### Knowledge Sources and the Prompt Library

- **What it does:** Knowledge Sources let you upload firm documents or legislation as extra context for Archie. The Prompt Library stores your firm's prompts and ones written by Smokeball. [S29] [S7]
- **Where to find it:** The **Knowledge Sources** tab in the Archie screen. You can make a source active for yourself or for all staff. [S29]
- **Which plans have it:** Available to all Archie users. [S9]
- **What happens to your data:** Uploaded PDF, DOCX, TXT and MD files are text-extracted and used across matters of the types you choose. [S29]
- **In Australia:** Smokeball's examples include the Family Law Act 1975 and the Conveyancing Act 1919 (NSW). [S29]

### Smaller AI features

- **AutoTime descriptions:** Suggests time entry descriptions based on your last 100 edits. It's in beta, needs AutoTime, and works only in the desktop app. It doesn't need the Archie add-on. [S30]
- **Intake forms:** Generates an intake form, or converts a paper form, using Smokeball AI. It comes with the Intake add-on or Prosper+ and doesn't need Archie. [S31]
- **Message summaries:** Summarises a client conversation in the Messages tab if you're a participant. Only staff can see the summary. [S32]

## Outside AI that connects

In plain words, a connector lets a chat assistant such as Claude or ChatGPT look things up in another app, and sometimes make changes there. Anthropic lists each one in its Connectors directory with a Verified or Community label. [S63]

Smokeball's Archie runs OpenAI, Anthropic and Google models inside Smokeball. Using Archie doesn't link Smokeball to your own ChatGPT, Claude or Gemini account. [S15] [S19]

### Claude and Smokeball

**Official?**

- No official connection found. Smokeball isn't among the connectors on Anthropic's public directory page. [S54]
- Smokeball's Australian help centre mentions Claude only in Archie's model list and release notes. [S15] [S39]

**What it can see and do**

- Nothing official. [S54]

**What you need, steps, disconnecting**

- Not applicable. [S54]

**Limits**

- Smokeball's terms make you responsible for keeping user IDs to one person each and for the actions taken with them. [S5]
- Our reading: giving an AI tool your Smokeball login to work in the app sits awkwardly with that. This isn't legal advice.

### ChatGPT and Smokeball

**Official?**

- No official connection found. Smokeball isn't on OpenAI's public plugin page, including its Legal category. [S55]

**What it can see and do**

- Nothing official. [S55]

**Limits**

- Archie's GPT models run inside Smokeball. They aren't a link to your own ChatGPT account. [S15]

### Microsoft Copilot and Smokeball

**Official?**

- No official connection found. Smokeball isn't among Microsoft's federated Copilot connectors, last updated 16 October 2026. [S56]
- Smokeball isn't in Microsoft's list of Power Platform connectors either. [S57]

**What Smokeball does offer in Microsoft 365**

- Smokeball's own add-ins for Outlook and Word, including the Smokeball Archie add-in, are listed on Microsoft's Marketplace. [S50]
- Smokeball's help centre notes that Microsoft's Copilot is available in classic Outlook. That's Microsoft's own assistant, and Smokeball doesn't describe any link between it and Smokeball. [S42]
- Smokeball's Power BI integration lets you build reports from Smokeball data. Smokeball notes Power BI "offers AI-powered insights (via Microsoft Copilot)". [S43]

**Limits**

- Smokeball's help centre doesn't describe any Copilot agent or connector for Smokeball. [S42] [S43]

### Google Gemini and Smokeball

**Official?**

- No official connection found. Smokeball isn't on Google's list of Connected Apps for Gemini. [S58]

**Limits**

- The Archie Word add-in uses Gemini 3.1 models. That's inside Smokeball's add-in and isn't your Gemini app. [S19]

### Zapier and Smokeball

**Official?**

- Yes. Smokeball's help centre documents the Smokeball app in Zapier. [S33]

**What it can see and do**

- Triggers: contact updated, new contact, new expense, new fee, new lead, new matter, new memo and new task. [S33]
- Actions: create a calendar event, lead, matter, matter memo, organisation contact, person contact or task, upload a file to a matter, and find a contact by name. [S33]
- Zapier's own page offers Smokeball through Zapier MCP, which lets AI tools that support MCP run Smokeball actions. [S59]

**What you need**

- A Zapier account and your Smokeball login. [S33]
- Smokeball's support covers the integration working in Smokeball. Questions about Zapier's own features go to Zapier. [S33]

**Steps to connect** (Smokeball help centre, edited 3 August 2026)

1. Log in to Zapier and go to **App Connections** on the left menu. [S33]
2. Select **Add connection**, type Smokeball and select it. [S33]
3. Select **Add connection**, confirm your region in the window that opens, and log in with your Smokeball credentials. [S33]
4. Create a Zap with a Smokeball trigger or action. [S33]

**To disconnect**

- Smokeball's article doesn't describe disconnecting. [S33]

**Limits**

- Smokeball's article doesn't mention AI or MCP. Running Smokeball actions from an AI tool through Zapier MCP is Zapier's route. [S33] [S59]

### Smokeball's API

- Firms building their own app can apply for API access if they're on Prosper+ and have in-house or hired developers. [S34]
- Australian firms use Australian endpoints: api.smokeball.com.au, with sign-in at auth.smokeball.com.au. [S44]
- Access is limited by read and write scopes, such as `matters/read` and `documents/write`. [S46]
- The default limit is 5 requests a second. [S45]
- Smokeball's developer documentation index lists no MCP server. [S47]

### Other AI apps that connect to Smokeball

- **AI Legal Assistant** is an Australian AI tool for document review, research and chronologies. Documents you create in it are saved to the Smokeball matter. [S35]
- **AI Legal Toolbox** by Elysia Partners works in Outlook. Once connected, it can look up Smokeball matters and contacts and create time entries. [S36]
- In both cases Smokeball says it integrates with the tool but doesn't develop or manage it. [S35] [S36]
- Smokeball's Australian marketplace listed 109 partners on 17 October 2026, including Archie itself. [S49]
- Smokeball's privacy notice says third-party apps you enable handle your data under their own terms and privacy policies, and Smokeball isn't responsible for their privacy practices. [S4]

## Jobs it's good for

- **Catching up on a matter.** Ask Archie for a summary of the matter's documents, meetings and deadlines, linked to the sources. [S1] [S16]
- **A reply drafted from the file.** In Outlook, use Draft with Archie to write an email from the matter's key dates and documents, then adjust the tone. [S11] [S21]
- **Checking a contract against your firm's rules.** Build a Playbook in the Word add-in and run it on the draft. [S20]
- **Turning a recording into a file note.** Transcribe an audio or video file and save the transcript to the matter. [S28]
- **Bank statements in family law.** Use the Bank Statements Analyser to filter transactions and spot patterns. [S9]
- **A legal question with a second opinion.** Ask LawY in the Legal Research tab and send the deep research for verification. [S26]
- **Admin from a chat.** Ask Archie to create a task or calendar event, then check it before saving. [S23]

## What to watch for

**Who can see what**

- Archie is on for everyone by default. Only a Firm Owner can switch it off for a user, in **Settings > Staff & Users > Permissions**, using the **Archie** column. [S16] [S18]
- Your Archie questions on a matter are visible to colleagues working on it. [S16]
- Archie can see every user's name and email address and the matter's invoice and trust account details. [S16]

**Where your data goes**

- Smokeball says data stays in its home region "as a principle" and asks you to contact Smokeball for details of your firm's setup. [S14]
- Archie's model list spans OpenAI, Anthropic and Google, and Smokeball doesn't say where each model processes Australian data. [S15] [S19]
- Smokeball says the sub-processors that apply depend on the integrations you've enabled, and can be reviewed in its marketplace. [S14]
- Smokeball's terms let it de-identify and aggregate client data for research, benchmarking and developing new products. [S5]

**Check the work**

- Smokeball's help centre says an Archie answer "may sound correct and read well" but "may not be correct", and asks you to "Trust but verify". [S16]
- From October 2026 Archie highlights placeholders in drafts and asks you to fill in missing information. [S41]
- Smokeball's June 2026 article quotes a December 2024 joint statement by three Australian legal regulators about entering confidential client information into public AI chatbots. We didn't read the regulators' statement itself. [S13]

**Things Archie can do in your system**

- Archie can create tasks, memos and calendar events. Smokeball says all such actions "require explicit user confirmation before execution". [S23] [S38]
- Archie reads billing data but "cannot create, modify, or delete billing records", according to the June 2026 release notes. [S39]

**Outside apps**

- Third-party AI apps that connect to Smokeball handle your data under their own terms. [S4] [S35]

## Announced changes

- **31 July 2024:** Smokeball launched Archie. [S6]
- **24 March 2025:** The Archie Prompt Library became generally available. [S7]
- **3 September 2025:** Archie Apps and Knowledge Sources were released. [S9]
- **13 November 2025:** LawY became a free inclusion with the Archie add-on. [S37]
- **25 November 2025:** The Audio Transcription app became available to firms with Archie. [S37]
- **2 April 2026:** The new Outlook add-in brought Archie into Outlook. Smokeball listed Outlook mobile app support as "coming soon" in that post. [S11]
- **4 May 2026:** Archie moved to a new agentic model, gained the Word add-in, voice dictation and the ability to create tasks, memos and events. [S38]
- **11 June 2026:** The model selector returned and Archie began reading read-only billing data. [S39]
- **3 September 2026:** Archie began answering from live matter data "instead of cached data up to 6 hours old". [S40]
- **Coming soon:** Tone profiles, which apply your firm's writing rules to each audience. [S12]
- **Not yet:** Smokeball says Archie can't yet add attachments or reminders to events, and "Full workflow automation is also not yet supported". [S23]
- **Classic Outlook:** Smokeball will keep supporting it while Microsoft does, but new features go only to the new add-in. [S22]

## What we couldn't establish

- **The price of the Archie add-on.** Smokeball's Australian pricing page says "Learn more" instead of a price. [S2]
- **Whether Boost firms can buy Archie.** The pricing page and help centre say yes, but the marketplace listing names only Grow and Prosper+. [S2] [S17] [S48]
- **Where Archie's AI processing happens for Australian firms.** Smokeball's principle is that data stays in its home region, but it doesn't say where each model runs. [S14] [S15]
- **Which billing data Archie reads.** The June 2026 release notes say Archie reads fees and disbursements. The getting-started article, edited in September 2026, says it can't access time and fee entries or expenses. [S39] [S16]
- **Smokeball's sub-processor list.** We couldn't find it in the marketplace pages we read. [S14] [S49]
- **How long the Archie question log is kept.** Not stated. [S14] [S16]
- **Outlook mobile support.** The April 2026 post calls it "coming soon" in one place and lists it as supported in its FAQ. [S11]
- **Who maintains Zapier's Smokeball app.** Smokeball documents the integration, but we didn't confirm who built it. [S33] [S59]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Archie AI: Legal Assistant for Australian Law Firms | Smokeball | https://www.smokeball.com.au/archie | No date shown (sitemap 12 Oct 2026) | 17 Oct 2026 |
| S2 | Legal Software Pricing for Australian Law Firms | Smokeball | https://www.smokeball.com.au/pricing | No date shown (sitemap 20 Aug 2026) | 17 Oct 2026 |
| S3 | Smokeball security policy | Smokeball | https://www.smokeball.com.au/security | "Last updated 09/07/2026" | 17 Oct 2026 |
| S4 | Privacy Notice | Smokeball | https://www.smokeball.com.au/privacy | "Last updated 02/06/2026" | 17 Oct 2026 |
| S5 | Terms of service | Smokeball | https://www.smokeball.com.au/terms | "Last updated 09/07/2026" | 17 Oct 2026 |
| S6 | Smokeball AI Revolutionises the Legal Tech Industry | Smokeball Blog | https://www.smokeball.com.au/blog/smokeball-ai-revolutionises-the-legal-tech-industry | 31 Jul 2024 | 17 Oct 2026 |
| S7 | Archie AI is Getting a Major Upgrade | Smokeball Blog | https://www.smokeball.com.au/blog/archie-is-getting-a-major-upgrade | 13 Mar 2025 | 17 Oct 2026 |
| S8 | Celebrating one year of Archie AI, our legal AI matter assistant | Smokeball Blog | https://www.smokeball.com.au/blog/celebrating-one-year-of-archie-our-ai-matter-assistant | 23 Jul 2025 | 17 Oct 2026 |
| S9 | Say hello to new Archie AI features | Smokeball Blog | https://www.smokeball.com.au/blog/say-hello-to-new-archie-ai-features | 3 Sep 2025 | 17 Oct 2026 |
| S10 | Smokeball announces LawY integration with Archie AI | Smokeball Blog | https://www.smokeball.com.au/blog/smokeball-announces-lawy-integration-with-archie-ai | 19 Nov 2025 | 17 Oct 2026 |
| S11 | Bring AI productivity to your inbox with the new Smokeball Outlook add-in | Smokeball Blog | https://www.smokeball.com.au/blog/bring-ai-productivity-to-your-inbox-with-the-new-smokeball-outlook-add-in | 2 Apr 2026 | 17 Oct 2026 |
| S12 | The next generation of Archie AI has arrived | Smokeball Blog | https://www.smokeball.com.au/blog/the-next-generation-of-archie-ai-has-arrived | 29 Apr 2026 | 17 Oct 2026 |
| S13 | What is the difference between a general AI assistant and legal AI built for law firms? | Smokeball Blog | https://www.smokeball.com.au/blog/what-is-the-difference-between-a-general-ai-assistant-and-legal-ai-built-for-law-firms | 25 Jun 2026 ("Last updated: June 2026") | 17 Oct 2026 |
| S14 | How Smokeball AI keeps your data private and secure | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/41226626717079-How-Smokeball-AI-keeps-your-data-private-and-secure | Edited 15 Jun 2026 (help centre data) | 17 Oct 2026 |
| S15 | Configure Archie Settings | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/35181898764951-Configure-Archie-Settings | Edited 21 Sep 2026 (help centre data) | 17 Oct 2026 |
| S16 | Getting Started with Archie, the Smokeball AI Assistant | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/24407844681751-Getting-Started-with-Archie-the-Smokeball-AI-Assistant | Edited 6 Sep 2026 (help centre data) | 17 Oct 2026 |
| S17 | Getting Started with Archie for Smokeball Boost | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/30752793429527-Getting-Started-with-Archie-for-Smokeball-Boost | Edited 19 May 2025 (help centre data) | 17 Oct 2026 |
| S18 | Managing staff and user permissions | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/8402863411991-Managing-staff-and-user-permissions | Edited 7 Oct 2026 (help centre data) | 17 Oct 2026 |
| S19 | Using the Archie Word Add-in | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/39699442435095-Using-the-Archie-Word-Add-in | Edited 1 Oct 2026 (help centre data) | 17 Oct 2026 |
| S20 | Using Archie Playbooks to Review Documents | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/43694624466455-Using-Archie-Playbooks-to-Review-Documents | Edited 23 Sep 2026 (help centre data) | 17 Oct 2026 |
| S21 | Connect to New Outlook | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/31216774250135-Connect-to-New-Outlook | Edited 27 Aug 2026 (help centre data) | 17 Oct 2026 |
| S22 | Microsoft Integrations for Smokeball Grow and Prosper+ | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/32905188463511-Microsoft-Integrations-for-Smokeball-Grow-and-Prosper | Edited 24 Apr 2026 (help centre data) | 17 Oct 2026 |
| S23 | Creating tasks, memos and events with Archie | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/39618100098967-Creating-tasks-memos-and-events-with-Archie | Edited 4 May 2026 (help centre data) | 17 Oct 2026 |
| S24 | Using Archie Suggestions | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/40283902464151-Using-Archie-Suggestions | Edited 13 Oct 2026 (help centre data) | 17 Oct 2026 |
| S25 | Archie file size limits | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/37629892969623-Archie-file-size-limits | Edited 21 Aug 2026 (help centre data) | 17 Oct 2026 |
| S26 | Using LawY in Archie for legal research | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/33653338648599-Using-LawY-in-Archie-for-legal-research | Edited 5 Nov 2025 (help centre data) | 17 Oct 2026 |
| S27 | Getting Started with Archie Apps | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/32304670869399-Getting-Started-with-Archie-Apps | Edited 8 Sep 2025 (help centre data) | 17 Oct 2026 |
| S28 | Transcribe audio files using Archie | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/36561902022679-Transcribe-audio-files-using-Archie | Edited 25 May 2026 (help centre data) | 17 Oct 2026 |
| S29 | Upload Knowledge Sources to use with Archie | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/33653315990423-Upload-Knowledge-Sources-to-use-with-Archie | Edited 8 Sep 2025 (help centre data) | 17 Oct 2026 |
| S30 | Generate AutoTime descriptions using Smokeball AI | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/34416807166103-Generate-AutoTime-descriptions-using-Smokeball-AI | Edited 1 Sep 2025 (help centre data) | 17 Oct 2026 |
| S31 | Generate a custom Intake Form using Smokeball AI | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/24606986834583-Generate-a-custom-Intake-Form-using-Smokeball-AI | Edited 3 Oct 2025 (help centre data) | 17 Oct 2026 |
| S32 | Summarise a matter conversation with AI | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/21308177955735-Summarise-a-matter-conversation-with-AI | Edited 18 Jun 2026 (help centre data) | 17 Oct 2026 |
| S33 | Zapier Integration | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/15431574575511-Zapier-Integration | Edited 3 Aug 2026 (help centre data) | 17 Oct 2026 |
| S34 | Request Smokeball API access for your app | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/24804817026327-Request-Smokeball-API-access-for-your-app | Edited 17 Mar 2025 (help centre data) | 17 Oct 2026 |
| S35 | AI Legal Assistant Integration | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/29380827229975-AI-Legal-Assistant-Integration | Edited 23 Jul 2026 (help centre data) | 17 Oct 2026 |
| S36 | AI Legal Toolbox Integration | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/44056406222231-AI-Legal-Toolbox-Integration | Edited 7 Oct 2026 (help centre data) | 17 Oct 2026 |
| S37 | Smokeball Grow and Prosper+ Releases November 2025 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/36083001262231-Smokeball-Grow-and-Prosper-Releases-November-2025 | Edited 25 Nov 2025 (help centre data) | 17 Oct 2026 |
| S38 | Smokeball Grow and Prosper+ Releases May 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/40063185076887-Smokeball-Grow-and-Prosper-Releases-May-2026 | Edited 27 May 2026 (help centre data) | 17 Oct 2026 |
| S39 | Smokeball Grow and Prosper+ Releases June 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/40870816082711-Smokeball-Grow-and-Prosper-Releases-June-2026 | Edited 23 Jun 2026 (help centre data) | 17 Oct 2026 |
| S40 | Smokeball Grow and Prosper+ Releases September 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/43238244923799-Smokeball-Grow-and-Prosper-Releases-September-2026 | Edited 30 Sep 2026 (help centre data) | 17 Oct 2026 |
| S41 | Smokeball Grow and Prosper+ Releases October 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/43867861521943-Smokeball-Grow-and-Prosper-Releases-October-2026 | Edited 9 Oct 2026 (help centre data) | 17 Oct 2026 |
| S42 | Smokeball and compatibility with New Outlook | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/14456059242135-Smokeball-and-compatibility-with-New-Outlook | Edited 24 Apr 2026 (help centre data) | 17 Oct 2026 |
| S43 | Power BI Integration | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/27898948586007-Power-BI-Integration | Edited 29 Jul 2026 (help centre data) | 17 Oct 2026 |
| S44 | Base URLs | Smokeball Developer Docs | https://docs.smokeball.com/docs/api-docs/z2q8vla6b77g8-base-urls | No date shown | 17 Oct 2026 |
| S45 | Rate Limits | Smokeball Developer Docs | https://docs.smokeball.com/docs/api-docs/vj4jovpoopdov-rate-limits | No date shown | 17 Oct 2026 |
| S46 | Scopes | Smokeball Developer Docs | https://docs.smokeball.com/docs/api-docs/qf83nz2scopes-scopes | No date shown | 17 Oct 2026 |
| S47 | Documentation index (llms.txt) | Smokeball Developer Docs | https://docs.smokeball.com/llms.txt | No date shown | 17 Oct 2026 |
| S48 | Archie powered by Smokeball AI (marketplace listing) | Smokeball Marketplace | https://marketplace.smokeball.com/partners/archie | No date shown | 17 Oct 2026 |
| S49 | Smokeball Marketplace (Australia) | Smokeball Marketplace | https://marketplace.smokeball.com/?selectaregion=5 | No date shown; 109 partners listed | 17 Oct 2026 |
| S50 | Smokeball Archie (Word add-in listing) | Microsoft Marketplace | https://marketplace.microsoft.com/en-gb/product/WA200010415?tab=Overview | No date shown | 17 Oct 2026 |
| S51 | Meet LawY in Smokeball | LawY | https://www.lawy.ai/integration/smokeball | No date shown (sitemap 11 Sep 2026) | 17 Oct 2026 |
| S52 | How to sign into LawY through an integration partner | LawY Help Centre | https://help.lawy.ai/en/articles/15201103-how-to-sign-into-lawy-through-an-integration-partner | 22 Jun 2026 | 17 Oct 2026 |
| S53 | Security | LawY | https://www.lawy.ai/security | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S54 | Connectors directory | Anthropic | https://claude.com/connectors | No date shown | 17 Oct 2026 |
| S55 | ChatGPT Plugins (including the Legal category) | OpenAI | https://openai.com/business/plugins/ | No date shown | 17 Oct 2026 |
| S56 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Updated 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S57 | List of all Copilot Studio, Power Platform and Logic Apps connectors | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/connector-reference/ | Updated 2 Oct 2026 (page metadata) | 17 Oct 2026 |
| S58 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 17 Oct 2026 |
| S59 | Smokeball MCP | Zapier | https://zapier.com/mcp/smokeball-1 | No date shown | 17 Oct 2026 |
| S60 | Smokeball Bill and Boost Releases June 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/40870909742359-Smokeball-Bill-and-Boost-Releases-June-2026 | Edited 25 Jun 2026 (help centre data) | 17 Oct 2026 |
| S61 | Terms and Conditions | LawY | https://www.lawy.ai/terms-and-conditions | No date shown (sitemap 15 Oct 2026) | 17 Oct 2026 |
| S62 | Smokeball Bill and Boost Releases May 2026 | Smokeball Support Hub (AU) | https://support.smokeball.com/hc/en-au/articles/40150404843799-Smokeball-Bill-and-Boost-Releases-May-2026 | Edited 1 May 2026 (help centre data) | 17 Oct 2026 |
| S63 | Get started with connectors | Anthropic | https://claude.com/docs/connectors/getting-started | No date shown (page metadata 25 Sep 2026) | 17 Oct 2026 |
