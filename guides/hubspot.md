# HubSpot: the AI inside it, and the AI that connects to it
Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

HubSpot's own AI assistant, Breeze Assistant, comes with every plan including the free tools, and it doesn't use credits. [S2][S4][S37]
Its AI agents, which do work like answering customer chats or researching prospects, have all spent HubSpot Credits since 23 July 2026. [S14][S17][S20]
Paid plans include monthly credits, and credit packs bought from 16 September 2026 bill any extra use as overage by default. [S12][S11]
HubSpot has official connectors for ChatGPT, Claude, Microsoft Copilot and Gemini, and they work on any HubSpot plan. [S81][S43][S48][S59][S64]
ChatGPT and Claude can create and update records once you confirm, while HubSpot's Copilot agent and its Gemini connector can only read. [S43][S48][S59][S64]
Each connector sees only what that person can already see in HubSpot, and a Super Admin controls who may connect. [S43][S48][S80]
HubSpot may use your customer data to train its own AI models unless a Super Admin switches off **AI Model Training**, which is on by default. [S5][S3]
Accounts can be hosted in Sydney, but HubSpot's sub-processor list shows its AI providers handle Australian-hosted data in the United States. [S10][S9]
Every vendor here warns the AI can be wrong, so set connectors to ask before they change anything. [S43][S48][S59][S64]

## The tool, and the plans that matter

**Words used in this guide**

- **CRM** is the customer database at the centre of HubSpot. HubSpot calls it Smart CRM. [S12]
- **Hubs** are HubSpot's add-on products. HubSpot's current help articles list Marketing Hub, Sales Hub, Service Hub, Content Hub, Data Hub, Smart CRM and Revenue Hub. [S1]
- Revenue Hub is the new name for Commerce Hub. It covers quotes, contracts, billing and payments. [S40]
- **Seats** are paid user licences. Only paid seats (Core, Sales, Service and Revenue) and Partner seats can use credits. Free and view-only users can't. [S11]
- **HubSpot Credits** are HubSpot's usage currency for agents and other AI that runs on its own. They're spent when an action runs. The allowance resets monthly, and unused credits don't roll over. [S11]
- An **API** is the doorway other software uses to read or change your HubSpot data. Every outside AI connection goes through it and counts toward HubSpot's API usage limits. [S43][S48][S59][S64]
- **MCP** (Model Context Protocol) is a shared standard that lets AI assistants talk to software like HubSpot. Think of it like a standard power socket. HubSpot provides the socket, and any AI tool with the matching plug can use it. [S70][S60]
- A **Super Admin** is HubSpot's top admin role. Most AI switches and app approvals need one. [S3][S80]

**What each plan gets**

| | Free tools | Starter | Professional | Enterprise |
|---|---|---|---|---|
| Breeze Assistant | Yes [S2] | Yes [S2] | Yes, plus building agents and workflows [S2] | Yes [S2] |
| AI writing tools and record summaries | Yes [S24][S25] | Yes [S24][S25] | Yes [S24][S25] | Yes [S24][S25] |
| Connectors for ChatGPT, Claude, Copilot and Gemini | Yes [S43][S48][S59][S64] | Yes | Yes | Yes |
| Monthly credits included | None listed [S12] | 500 [S12][S39] | 3,000, or 5,000 with Data Hub or Customer Platform [S12] | 5,000, or 10,000 with Data Hub or Customer Platform [S12] |
| Data enrichment (no credits) | Not listed [S22] | Yes [S22] | Yes [S22] | Yes [S22] |
| Prospecting agent and data agent | Not listed [S20][S21] | Yes, uses credits [S20][S21] | Yes [S20][S21] | Yes [S20][S21] |
| Customer agent | Not listed [S18] | Not listed [S18] | Yes, uses credits [S18] | Yes [S18] |
| Agent Hub and Agent Builder | Not listed [S1] | HubSpot's pages disagree [S1][S16] | Yes, public beta [S16][S74] | Yes, public beta [S16][S74] |
| Notetaker and deal progression | Not listed | Not listed | Sales Hub or Service Hub Professional [S26][S27] | Sales Hub or Service Hub Enterprise [S26][S27] |
| Content agent and AEO | Not listed | Not listed | Marketing Hub Professional [S28][S29] | Marketing Hub Enterprise [S28][S29] |
| Knowledge base agent | Not listed | Not listed | Service Hub Professional [S30] | Service Hub Enterprise [S30] |
| Sensitive Data settings | Not listed | Not listed | Not listed | Yes [S36] |
| Your own AI model inside workflows | Not listed | Not listed | Not listed | Yes [S79] |

- Credits don't stack across hubs. An account gets the allowance for its highest subscription. [S12]
- Prices: all of these are paid plans. The pricing pages we could read showed US dollars only, and the Starter page says "Price shown in USD", so we haven't quoted any plan prices. Check HubSpot's pricing page for current figures. [S39]
- Extra credits: HubSpot's catalogue lists capacity packs at US$10 per 1,000 credits a month and pay-as-you-go at US$0.010 a credit. We found no AUD rate. [S12][S13]

**Where your data lives**

- HubSpot hosts accounts on Amazon Web Services in the US, Canada, the EU (Germany) and Australia (Sydney). [S10]
- A new account bought on HubSpot's website is placed in a data centre based on where the sign-up IP address is. [S10]
- Starter, Professional and Enterprise accounts can change data centre. Free accounts have to upgrade first. [S10]
- To check yours: settings icon > **Privacy & Consent** > **Data Hosting** tab > *Your data hosting location*. [S10]
- Some data sits outside your hosting location by design. HubSpot says analytics and usage data is transferred to the United States. [S10]
- HubSpot Content, which HubSpot says includes enrichment data, may also be hosted elsewhere. [S10]
- Sub-processors (other companies HubSpot uses) are listed per data centre on HubSpot's sub-processor page. [S9][S10]
- HubSpot itself isn't currently ISO 27001 certified. Its hosting provider, AWS, is. [S10]

## AI built in

Two things apply to every feature in this section.

First, a Super Admin controls the AI switches at settings icon > **Account management** > **AI** > **Access** tab. [S3] The settings page is available on all plans. [S3]

| Switch (exact label) | What it controls | Default |
|---|---|---|
| **Give users access to generative AI tools and features** | Any generative AI feature, including Breeze Assistant [S3] | On [S3] |
| **CRM data** | Lets AI use CRM records, default properties and user-generated content [S3] | On [S3] |
| **Customer conversation data** | Lets AI summarise and respond to conversations such as call transcripts and emails [S3] | On [S3] |
| **Files data** | Lets AI use public files and files in HubSpot's Files tool [S3] | Off [S3] |
| **Give users access to Breeze Assistant** | Breeze Assistant for users [S3] | On [S3] |
| **AI Model Training** | Whether HubSpot may train its own models on your customer data [S3][S5] | On [S3][S5] |

Changes to these switches show in the audit log. In a multi-account setup, each account is set separately. [S3]

Second, for accounts hosted in Australia, HubSpot's sub-processor list names AWS, Google and OpenAI as "AI Service Provider" for HubSpot AI, all processing in the United States. Baseten joins that list from 16 October 2026, also in the United States. [S9]

HubSpot's model cards list models from OpenAI, Anthropic and Google behind its assistant and agents, plus Perplexity for some other AI features. Each card notes "Model Zero Data Retention" and no customer data used for third-party model training. [S8]

A note on names. Breeze Assistant still carries the Breeze name. [S2] HubSpot's old "Understand Breeze" help link now opens a page called "Understand Agent Hub", and current help articles call the agents "customer agent", "prospecting agent" and so on. [S1][S17][S20] HubSpot's April 2026 news still said "Breeze Customer Agent". [S42] It appears HubSpot is dropping Breeze from agent names. That's our inference, and HubSpot hasn't announced it.

### Breeze Assistant

**What it does.** A chat assistant inside HubSpot that answers using your HubSpot data, content you've given it and the user's role. [S2]
It can summarise records and conversations, and list records that match what you ask for. [S2]
Once a calendar is connected, it can prepare you for upcoming meetings. [S2]
It can draft sales emails and generate images and charts from CRM data. [S2]
It can also create deals, notes, products, quotes, agents and workflows, within each user's permissions and plan. [S2]
It can search apps you've installed from HubSpot's App Marketplace, such as Gmail or Slack. [S2][S34]
It keeps chat history (on by default), "memories" of a user's preferences, saved prompts, and projects that group chats with shared instructions and files. [S2][S33]
Since September 2026 it can run a saved prompt daily, weekly or monthly, with results landing as a new chat. [S74]
Outputs can be saved as "artifacts", such as HTML pages or documents, and shared with users, teams or the whole company. [S2]

**Where to find it.** Click **Breeze Assistant** in the top navigation bar. [S2]
The **Breeze** dropdown holds **New chat**, **Chats** and **Artifacts**, with **Memories** under **More**. [S2]
On a record, **Actions** > **Summarize** gives a Breeze Assistant summary. [S25]
It's also in the HubSpot mobile app for iOS and Android. [S37]

**Plans and cost.** All products and plans, free tools included. [S2]
HubSpot says it's included "at no additional cost" and that it doesn't consume credits. [S37][S4]
Some of what it does needs more: building agents or workflows needs Professional or Enterprise, and quotes need Revenue Hub Professional or Enterprise. [S2]
Content generation is capped at 30 requests a minute and 1,000 a day. [S2]

**On by default, and who controls it.** On for all users by default. [S3][S4]
A Super Admin can switch off **Give users access to Breeze Assistant**, or remove it for particular users or teams through the **Breeze Assistant** user permission. [S3][S4]

**Your data.** It only uses CRM, conversation and file data if those switches are on. [S3]
Users can delete memories. [S2][S33]
PPTX and HTML artifacts can be shared as public read-only links, with an optional password. [S2]
HubSpot doesn't say how long it keeps chats, memories or artifacts. [S2][S33]

**In Australia.** The article sets no country limits. [S2] AI processing for Australian-hosted accounts is listed as United States. [S9]

### AI writing tools in HubSpot's editors

**What it does.** Highlight text and HubSpot's AI can rewrite, expand, shorten or change its tone, or apply your brand identity. [S24]
Typing "/" in a rich text section generates a heading, paragraph, image or subsection. [S24]
It also writes page titles and meta descriptions, social posts from blog posts, email text in workflows, and sales emails in the HubSpot Sales Chrome extension for Gmail and the iOS app. [S24]
HubSpot's AI help index also lists AI sales emails in the HubSpot Sales Office 365 add-in. [S84]

**Where to find it.** The AI icon after highlighting text, or "/" in a rich text section. [S24]

**Plans and cost.** All products and plans. [S24] The article doesn't mention credits. Limits are 30 generations a minute and 1,000 a day, with prompts and responses capped at 4,000 tokens. [S24]

**On by default, and who controls it.** It needs **Give users access to generative AI tools and features**, which is on by default. [S3][S24] Some uses also need the normal tool permission, such as edit and publish rights for pages. [S24]

**Your data.** Generated text appears in a side panel for you to check before it goes in. [S24]

**In Australia.** No country limits stated. [S24] Processing as above. [S9]

### Record summaries

**What it does.** An AI summary on contact, company, deal and ticket records, built from logged activities, notes and ownership. [S25]

**Where to find it.** Add the **Record summary** card through **Add card** > **Card library** in the record layout editor, or use **Actions** > **Summarize** on a record. [S25]

**Plans and cost.** All products and plans. [S25] The article doesn't mention credits. [S25]

**On by default, and who controls it.** The card needs the CRM data and customer conversation data switches on. [S25] Admins choose whether the card appears on records. [S25]

**Your data.** It only reflects what's been logged to the record. [S25] With Sensitive Data turned on, some activities such as calls and sales emails may not be summarised. [S25]

**In Australia.** No country limits stated. [S25] Processing as above. [S9]

### Agent Hub, Agent Builder and the Agent Marketplace

**What it does.** Agent Hub is one workspace for viewing and managing HubSpot's ready-made agents and any custom ones. [S1]
Agent Builder creates an agent from inputs, instructions, tools, knowledge sources and automation settings. [S1]
Breeze Assistant can draft an agent's setup from a plain-English description and open it for testing (public beta). [S74]
The Agent Marketplace lists HubSpot-built agents you install and then adjust. Custom agents can't be listed there. [S15]
Agents can also be triggered from workflows. [S1][S84]

**Where to find it.** **More** > **Agents** > **Agent Hub**, or **Agents** > **Agent Hub** if there's no **More** menu. [S1]
Marketplace: **More** > **Agents** > **Agent Marketplace** > **Explore all** > choose an agent > **Add**. [S15]

**Plans and cost.** HubSpot's Agent Hub article lists Starter, Professional and Enterprise for Marketing, Sales, Service, Data and Content Hub, and Professional or Enterprise for Smart CRM and Revenue Hub. [S1]
HubSpot's news post and developer changelog describe Agent Hub and Agent Builder as a public beta for Professional and Enterprise. [S16][S74]
Since 23 July 2026, all AI agents consume HubSpot Credits. [S14]
Custom agents cost 1 credit per "action unit" (beta). [S12]
A test run (HubSpot calls it a simulation) estimates the credit cost without spending any credits or changing the CRM. [S14]
You can cap each agent's monthly runs: **Agents** > **Agent Hub** > **Agents** tab > **Edit** > three dots > **Edit run limit**. [S14]

**On by default, and who controls it.** Agents aren't running until someone installs or builds them. [S1][S15]
Before installing a marketplace agent, a Super Admin turns on the generative AI, CRM data, conversation data, files data and Breeze Assistant switches. [S15]
Creating or customising agents needs Super Admin or the **Agent builder** permission. [S15][S4]
Each agent or project has access settings, such as "Owners and super admins can edit and run". [S4]

**Your data.** Agents can draw on your AI context and knowledge vaults. [S1][S32]
Deleting an agent is permanent and removes its data. [S1]

**In Australia.** No country limits stated. [S1] Processing as above. [S9]

On 23 July 2026 HubSpot retired five agents: Social Post, ABM Landing Page, RFP, Cross-sell/Upsell and Sales to Marketing Feedback. Installed copies stay, but they can't be installed again. [S15]

### Customer agent

**What it does.** Answers customer questions on live chat, email, Facebook Messenger and WhatsApp, using content you sync such as help articles and website pages. [S17][S18]
It can run actions like booking a meeting, and it hands the conversation to a person when it isn't confident or a handoff rule kicks in. [S17]
It can also just suggest replies for staff to check, and those suggestions don't use credits. [S17]
A voice version (public beta) answers inbound calls on your HubSpot phone number. It can't make outbound calls yet. [S19]

**Where to find it.** **More** > **Service** > **Customer Agent** > **Continue to agent setup**. [S18]

**Plans and cost.** Professional or Enterprise of any hub, including Smart CRM and Revenue Hub. [S18]
50 credits per resolved text conversation, and 50 credits per minute of voice (beta). [S12]
You pay per resolved conversation, however many messages it takes. [S17]
A conversation counts as resolved when the agent shares a source or completes an action and the customer doesn't ask for a person within 72 hours, or when it marks a lead's qualification. [S17]
New setups can opt in to 14 days of free access. [S17][S18] HubSpot's April 2026 news post mentioned a 28-day trial. [S42]
When credits run out, it stops taking new conversations, and they follow your handoff process instead. [S17]
Testing doesn't use credits. [S18]

**On by default, and who controls it.** Nothing goes live until it's set up and deployed to a channel, and at least one chat, Facebook or WhatsApp channel must be connected first. [S17][S18]
Editing it needs the **Customer agent editor** permission and an assigned seat. [S17]

**Your data.** Chat replies carry a "Powered by AI" label. [S17]
It needs the generative AI, CRM data, conversation data and files data switches on. [S17]
Voice calls are recorded and transcribed. [S19]

**In Australia.** Neither the chat nor the voice article mentions country limits. [S17][S19] Processing as above. [S9]

### Prospecting agent

**What it does.** Watches companies in your target lists for signals such as funding or product launches. [S20]
For each company it suggests up to three contacts that fit your buyer profiles, then writes personalised outreach. [S20]
It can pull contacts from Apollo, Surfe, ZoomInfo or Seamless, one source at a time. [S20]
You choose **Review before sending** or **Send automatically**. [S20]

**Where to find it.** **More** > **Sales** > **Prospecting Agent**. [S20]

**Plans and cost.** Starter, Professional or Enterprise of Marketing, Sales, Service, Data or Content Hub, and Professional or Enterprise of Smart CRM. Credits required. [S20]
100 credits per lead it recommends outreach for. [S12] HubSpot's April 2026 news post said Professional and Enterprise only. [S42]
Credit-using actions don't run in sandbox accounts. [S20]

**On by default, and who controls it.** Off until you set up a "play". [S20] It needs a Super Admin or the **Access prospecting agent** permission. [S20]

**Your data.** It uses a year of engagement history on each contact, including form submissions, page views, calls, meetings, notes and email opens. [S20]

**In Australia.** No country limits stated. [S20] Processing as above. [S9]

### Data agent and smart properties

**What it does.** A "smart property" is a custom field the AI fills in for each record by answering a question you write. [S21]
It can draw on web research, the company's website, existing property data or call transcripts. [S21]
It also adds workflow actions ("Data Agent: Fill Smart Property" and "Data Agent: Research") and AI columns in Data Studio. [S21]

**Where to find it.** **More** > **Data Management** > **Data Agent**. [S21]

**Plans and cost.** Starter, Professional or Enterprise of Marketing, Sales, Service, Data or Content Hub, and Professional or Enterprise of Smart CRM and Revenue Hub. [S21]
10 credits per response for one record. [S12]

**On by default, and who controls it.** Each user needs the **Data Agent access** switch on. It's on by default for Super Admins. [S21]

**Your data.** HubSpot advises against putting sensitive information into prompts. [S21]

**In Australia.** No country limits stated. [S21] Processing as above. [S9] From 16 October 2026 HubSpot adds Bright Data and Exa Labs as "Web Search Results" providers for HubSpot AI, processing in the US. The list doesn't say which features use them. [S9]

### Data enrichment and buyer intent

**What it does.** Fills in contact and company fields, such as job title and industry. [S22]
Its sources are HubSpot's commercial dataset and outside data providers, plus public information from the web. [S22]
It can hide form fields it can already fill ("form shortening"). [S22]
Buyer intent ("Intent, powered by Data Agent") flags companies showing interest. [S12]
HubSpot's current help articles call this "data enrichment" and don't use the older Breeze Intelligence name. [S22]

**Where to find it.** Settings icon > **Data Management** > **Data Enrichment** > **Settings** tab. [S23]

**Plans and cost.** Starter, Professional or Enterprise of Marketing, Sales, Service, Data or Content Hub, and Professional or Enterprise of Smart CRM and Revenue Hub. [S22]
Enrichment itself doesn't consume credits. [S22]
The catalogue lists 10 credits to "Enable intent signals for one month", and 10 to 50 credits for each beta intent action. It doesn't say whether the first figure is per company. [S12]

**On by default, and who controls it.** Automatic enrichment is off for contacts and companies until a Super Admin turns it on. [S22]
Users need the **Data enrichment access** permission to enrich records. [S23]

**Your data.** When a record is checked against several data points, limited business contact data may go back into HubSpot's commercial dataset. Accounts that only use continuous enrichment don't contribute. [S22]
Turning off AI Model Training doesn't turn off enrichment, and the reverse is also true. [S5]
People can ask HubSpot to remove them from its dataset. Those contacts get an "enrichment opt out" property, and Super Admins get a notification. [S22]

**In Australia.** HubSpot says enrichment data may be hosted outside your data centre. [S10]

### Notetaker and deal progression

**What it does.** Notetaker joins Google Meet, Microsoft Teams and Zoom meetings to record and transcribe them. [S26]
It writes a summary, suggests CRM updates, lists action items and drafts a follow-up email. [S26]
Deal progression (public beta) reads logged calls, meetings and emails, then suggests next steps and deal field updates. [S27]

**Where to find it.** Settings icon > **Notetaker**, then turn on **Conversation recording**, **Transcription and analysis** and **Meetings**. [S26]
Deal progression: **Agents** > **Agent Hub** > **Overview** > **Deal progression** > **Set up deal progression**. [S27]

**Plans and cost.** Sales Hub or Service Hub Professional or Enterprise, with a Sales or Service seat. [S26][S27]
From 14 April 2026, each custom field captured from a transcript costs 10 credits per run. Standard fields are free. [S26]

**On by default, and who controls it.** A Super Admin sets it up. [S26]
The **Require explicit consent** switch emails attendees first, and if anyone declines or doesn't reply, the meeting isn't recorded. [S26]
Deal progression suggestions need approval by default. Automatic updates are optional. [S27]

**Your data.** Recordings are kept for two years. [S26]
HubSpot says you're responsible for the disclosures and consents needed to record. [S26]
Notetaker data is processed by a sub-processor, Hyperdoc Inc. [S26]

**In Australia.** HubSpot's Notetaker article says Hyperdoc is hosted on AWS in the US, the EU (Frankfurt) and Asia (Tokyo). [S26] The sub-processor list gives United States as Hyperdoc's location for Australian-hosted accounts. [S9]

### Content agent, Marketing Studio and AEO

**What it does.** The content agent (beta) drafts LinkedIn posts, blog posts, LinkedIn articles, social posts, campaign assets and landing pages. It never publishes on its own. [S28]
In Marketing Studio, Breeze Assistant calls content and campaign agents to plan campaigns and draft content. [S41]
AEO (beta) tracks how often ChatGPT, Gemini and Perplexity mention your brand for the questions you track. [S29]

**Where to find it.** The content agent shows up in the social tool and in AEO recommendations. Marketing Studio uses it for campaign assets. [S28]
AEO: **More** > **Marketing** > **AEO**. [S29]

**Plans and cost.** Content agent: Marketing Hub Professional or Enterprise, plus credits. [S28] HubSpot's catalogue lists 1,000 credits per piece (beta). [S12]
Marketing Studio: Marketing Hub Professional or Enterprise. [S4]
AEO: Marketing Hub Professional or Enterprise, or a separate HubSpot AEO subscription, with a 28-day trial. [S29]
AEO's monthly answer limit is 2,500 on Professional and 5,000 on Enterprise. [S29]

**On by default, and who controls it.** A Super Admin must turn on the generative AI, files data and Breeze Assistant switches for the content agent. [S28]

**Your data.** The content agent draws on your account data and brand voice settings, so HubSpot suggests reviewing your AI data-sharing settings first. [S28]

**In Australia.** Neither article mentions country limits. [S28][S29] Processing as above. [S9]

### Knowledge base agent

**What it does.** A beta agent that reads closed support tickets to find gaps in your help centre. [S30]
It drafts articles to fill those gaps and suggests edits to existing ones. Drafts aren't published automatically. [S30]

**Where to find it.** **Service** > **Knowledge Base** > **Suggestions** tab. [S30]

**Plans and cost.** Service Hub Professional or Enterprise. 200 credits per generated article. [S30][S12]

**On by default, and who controls it.** A Super Admin must turn on **Customer conversation data**, and it needs at least five closed tickets. [S30]

**Your data.** It scans all conversation data on closed tickets, chats included. [S30]

**In Australia.** No country limits stated. [S30] Processing as above. [S9]

### Breeze Assistant in workflows

**What it does.** Describe a process and Breeze Assistant builds the whole workflow, triggers and actions included. New workflows start switched off until you check them. [S31]

**Where to find it.** In Breeze Assistant, or the workflow editor. [S31]

**Plans and cost.** Professional or Enterprise of Marketing, Sales, Service or Data Hub, Smart CRM or Revenue Hub. [S31]
Each AI action inside a workflow costs 10 credits when it runs. [S12]

**On by default, and who controls it.** Needs Super Admin or Workflows permission, plus the generative AI and Breeze Assistant switches. [S31]

**Your data.** HubSpot recommends turning on CRM data for better results. [S31]

**In Australia.** No country limits stated. [S31] Processing as above. [S9]

### AI context and knowledge vaults

**What it does.** AI context is the business background agents use, such as your brand's tone or your ideal customer profiles. [S1]
Knowledge vaults (beta) hold files and HubSpot content for specific agents and projects. [S32]

**Where to find it.** Agent Hub's **Context** tab. [S1][S32]

**Plans and cost.** Vaults: Starter, Professional or Enterprise of Marketing, Sales, Service, Data or Content Hub, and Professional or Enterprise of Smart CRM. [S32]
Up to 50 vaults, with files up to 50 MB each. [S32]

**On by default, and who controls it.** Vault permissions limit who can edit or use each one. Super Admins can always access all vaults. [S32]

**Your data.** Vaults accept documents, spreadsheets, CRM lists and HubSpot content such as calls. [S32] The article gives no warning about uploading sensitive material. [S32]

**In Australia.** No country limits stated. [S32] Processing as above. [S9]

### HubSpot's own model training

**What it does.** HubSpot may use your customer data to train its own AI models. [S5]
Some models are trained on your account alone, such as sales forecasts. Others learn across many accounts, such as spam detection and deal-close predictions. [S5]
HubSpot says the trained models give predictions and scores, and your business data isn't retrievable from them. [S5]

**Where to find it.** Settings icon > **Account management** > **AI** > **Access** tab > **AI Model Training**, at the bottom. [S5]

**Plans and cost.** All plans. [S3]

**On by default, and who controls it.** On by default. Only a Super Admin can turn it off. [S5]

**Your data.** Turning it off stops future use. It "is not possible to delete previously used data from trained models". [S5]
Accounts with Sensitive Data turned on are opted out automatically and can't opt in. [S5]
HubSpot doesn't let its outside AI providers train on your data, and it enforces zero data retention with them "wherever possible". [S5][S6]

**In Australia.** No Australia-specific statement. [S5]

### Other HubSpot agents

HubSpot's AI help index also lists a company research agent, customer health agent and deal loss agent, plus beta closing, revenue and RFP agents. [S84]
HubSpot retired an "RFP Agent" from the Agent Marketplace on 23 July 2026, yet its help index still has a beta RFP agent article. We can't tell whether these are the same agent. [S15][S84]
HubSpot's agent page adds a campaign agent and a nurture agent. [S38]
Rates in the catalogue include 500 credits for the revenue agent to start chasing one invoice and 10 credits for the nurture agent to personalise one email (both beta). [S12]

## Outside AI that connects

The four assistant connectors and HubSpot's MCP server all sign in as a person, so the AI sees only what that person can already see in HubSpot. [S43][S48][S59][S64][S70]
HubSpot's AI tools page names four: ChatGPT, Claude, Gemini and Microsoft Copilot. [S81]
HubSpot's developer docs say people already using those four should use the connectors, and save its MCP server for building your own agents. [S71]

**Before anyone connects: HubSpot's approval step.** Super Admins and users with the **App Marketplace Access** permission can connect the ChatGPT and Claude connectors without approval. Everyone else needs a Super Admin to approve the connector first. [S43][S48]
For the Copilot agent, a Super Admin or App Marketplace user has to make the first connection and choose its permissions. [S59]
The connector articles point to HubSpot's general app approval steps, which a Super Admin follows like this (Manage access to apps, 10 September 2026): [S80][S43]

1. Click the settings icon in the top navigation bar. [S80]
2. In the left sidebar, go to **Integrations** > **Connected Apps**. [S80]
3. Open the **Approved apps** tab and click **Approve apps**. [S80]
4. Search for and select the app. [S80]
5. In the *Manage access* banner, click **Approve**. [S80]
6. Choose who can install it: **Admins**, **Specific users and teams**, or **Everyone**. [S80]
7. Click **Next: Review data permissions**. [S80]
8. Turn optional permissions on or off, then click **Approve app**. [S80]

To take it away from one person: **Manage access** > **Installed by** tab > **Uninstall**. It can take up to 30 minutes. [S80]
To take it away from everyone: **Manage access** > **Revoke Approval** tab > **Revoke app approval**, type the app's name, then **Revoke**. [S80]
If a Super Admin adds data permissions later, each user has to reconnect to get the new access. [S43][S48]
Super Admins can see in the audit log who connected a connector and when. Writes are logged against both the person and the connector. [S43][S48]
HubSpot's April 2026 changelog describes this as the App Install Governance Tool (public beta), which lets Super Admins set read-only or write access for AI connectors. [S73]

### ChatGPT and HubSpot

**Official?** Yes. It's the "HubSpot connector for ChatGPT", built by HubSpot. [S43] It launched in June 2025 for deep research and added everyday chat in July 2025. [S44][S45] It can now write as well as read. [S43]
OpenAI's plugin directory lists it as HubSpot, made by HubSpot, version 6.0.0. The plugin also bundles four HubSpot skills, including Customer Prep and Pipeline Health. [S86]

**What it can see and do.** It can read contacts, leads, companies, deals, tickets, custom objects, products, quotes, invoices, orders, subscriptions, lists, campaigns, website and landing pages, blog posts, marketing emails, and calls, meetings, notes, tasks and emails. [S43]
It can create and update contacts, leads, companies, deals, tickets, custom objects, line items, products, campaigns, landing pages, blog posts, marketing emails and all the engagement types. [S43]
Users, quotes, invoices, orders, carts, subscriptions, lists, website pages and analytics are read-only. [S43]
HubSpot's object table shows no delete permission for anything. [S43]
Deep research mode writes a longer report with its sources shown in a side panel. [S43]
Before any create or update, ChatGPT shows the change and waits for you to reply Yes or No. [S43]
OpenAI's listing agrees that it can read from and write to deals, contacts, companies, tickets and engagements. [S86]

**What you need.** Any HubSpot plan, free tools included. [S43]
HubSpot says you need an OpenAI account and names no ChatGPT plan. [S43] OpenAI's HubSpot page says availability depends on the plugin, your plan and workspace settings, and doesn't list plans either. [S85]
In ChatGPT Business, apps start switched on. In Enterprise and Edu, new plugins and apps generally stay off until an admin reviews them. [S89]
If you're not a Super Admin and don't have App Marketplace Access, the connector has to be approved first. [S43]

**Steps to connect** (HubSpot, 28 September 2026):

1. In ChatGPT, click your profile icon (bottom left), then **Settings**. [S43]
2. Click **Apps**. [S43]
3. Select **HubSpot**, then **Connect**. [S43]
4. In the dialog, click **Continue to HubSpot**. [S43]
5. Log in to HubSpot and pick the HubSpot account. [S43]
6. On the "Connecting HubSpot Connector for ChatGPT to HubSpot" page, choose the permissions and click **Connect App**. [S43]
7. You land back in ChatGPT. To use it, click **+** > **More** > **HubSpot**, or mention "HubSpot" in your prompt. [S43]
8. For deep research: **+** > **Deep research**, then switch **HubSpot** on in the **Apps** dropdown. [S43]
9. In the connector's tool settings, set **Write tools** to **Needs Approval**. With **Always allow**, edits can happen without asking. [S43]

OpenAI's help centre now labels this route **Settings** > **Plugins**, with **Install plugin** and **Connect**, and says very old versions of the phone apps may still show **Apps**. [S88][S87] Its permission choices run from **Always ask** to **Allow all actions**, and it lists editing a record among actions that may need extra review. [S91]

**To disconnect.** Profile icon > **Settings** > **Apps** > **Enabled apps** > **HubSpot** > **Disconnect** (top right). [S43]
OpenAI's help centre gives the current route: **Settings** > **Plugins** > HubSpot > the account's **•••** menu (or **Connection**) > **Disconnect**. [S88]
A Super Admin can also uninstall it for a person, or revoke it for everyone, from **Connected Apps** in HubSpot. [S80]

**Limits.** Bulk creates and updates are capped at 10 records at a time. [S43]
Your custom validation rules, including pipeline stage and association label rules, aren't applied when it creates or updates records. [S43]
If Sensitive Data is turned on in HubSpot, it can't see any engagement data. [S43]
Draft pages and posts only return basic details. Performance figures need a campaign name and date range in your prompt. [S43]
It can't copy whole databases or customer lists, and one ChatGPT account connects to one HubSpot account at a time. [S43]
HubSpot warns that answers can contain errors and recommends a person checks them. [S43]

**Your data and Australia.** On ChatGPT Enterprise, Business or Edu, connector data isn't used for training. [S43]
On Free, Go, Plus or Pro you can opt out of training in ChatGPT's settings. If you don't, HubSpot says OpenAI may use connector data to improve the connector, but not for general model training. [S43]
OpenAI's own help page is broader. On Free, Go, Plus and Pro, it says OpenAI may use information from apps to train its models if **Improve the model for everyone** is on. [S87]
OpenAI keeps data accessed through the connector so the connector can work. [S43]
HubSpot says it respects your data centre while data passes through HubSpot's servers. The article sets no country limits. [S43]

**Not the same thing:** HubSpot also connects to ChatGPT Ads (beta) for running ads in ChatGPT. That's an advertising account link and needs the **Ads publishing** permission. [S47][S46]

### Claude and HubSpot

**Official?** Yes. It's the "HubSpot connector for Claude", built by HubSpot and marked "Anthropic verified" in Claude's directory. [S48][S53] It launched on 29 July 2025, and write access was added on 20 November 2025. [S49][S50]

**What it can see and do.** It can read, create and update contacts, leads, companies, deals, tickets, custom objects, line items, products, pipelines, landing pages, website pages, blog posts, marketing emails, and calls, meetings, notes, tasks and emails. [S48]
It can read and create (but not update) properties, campaigns, campaign assets and marketing events. Quotes are in beta. [S48]
Invoices, orders, payments, subscriptions, lists, campaign attribution, users, teams and inbox conversations are read-only. [S48]
It can't delete anything. [S48]
Before a create or update, Claude shows the change and waits for Yes or No. Afterwards a **View [record type] in HubSpot** link opens the record. [S48]
Claude can also chart and analyse CRM data in plain language. [S49]

**What you need.** Any HubSpot plan. [S48]
A paid Claude plan: Pro, Max, Team or Enterprise. [S48]
On Team and Enterprise, an organisation Owner has to add the connector first. Then each person connects their own HubSpot login. [S51][S54]
HubSpot's approval step applies as described above. [S48]

**Steps to connect** (Claude's help, no date shown; the HubSpot permission screen is from HubSpot's article of 17 September 2026):

1. In claude.ai or the Claude desktop app, go to **Customize** > **Connectors**. [S51]
2. Select **Discover**, type "HubSpot" in **Search connectors** and open the listing. [S51]
3. Select **Connect to Claude**. On Team or Enterprise you'll see **Request** instead if an Owner hasn't added it yet. [S51]
4. Sign in to HubSpot and choose the HubSpot account. [S51][S48]
5. On HubSpot's permissions page, choose what to allow and click **Connect app**. [S48]
6. Back in Claude, HubSpot shows **Connected** under **Your connectors**. [S51]
7. In a chat, select **+** > **Connectors** and switch **HubSpot** on. [S51][S48]
8. On the connector's page, set **Tool permissions** for write tools to **Needs approval**. [S51][S48]

HubSpot's own article still shows the older route: profile icon > **Settings** > **Connectors** > **Browse** > **HubSpot** > **Connect**. [S48]

**For Team and Enterprise Owners:**

1. Go to **Customize** > **Connectors** and select **Discover**. [S51]
2. Find HubSpot. [S51]
3. Select **Connect for your team** to add it for the whole organisation. [S51]
4. To try it yourself first, select the arrow beside that button and choose **Connect just for me**. [S51]
5. Connect your own account with **Connect to Claude**. [S51]
6. Member requests appear under **Organization settings** > **Connectors** in **Requested by your team**. [S52]

Owners can set tool permissions for the whole organisation, and members can't override them. [S54]
Enterprise admins can stop people connecting HubSpot with accounts outside the organisation. [S48][S54]

**To disconnect.** **Customize** > **Connectors** > **HubSpot** > **Disconnect**. Use the three-dot menu > **Remove** to take it off your account. [S51]
Team and Enterprise Owners remove it for everyone in **Organization settings** > **Connectors**. [S51]
HubSpot's article describes the older path: profile icon > **Settings** > **Connectors** > **HubSpot** > **Disconnect**. [S48]

**Limits.** Bulk creates and updates are capped at 10 records. [S48]
Conditional property rules and pipeline stage checks are applied, but association label checks aren't. [S48]
Only published pages and posts return content. Performance figures need a campaign name and date range. [S48]
If Sensitive Data is on, it can't see engagement data. [S48]
One Claude account connects to one HubSpot account at a time. [S48]
HubSpot's FAQ says Claude drafts campaign and workflow content for you to build yourself. Its object table lists marketing emails as create and update, so check what your account shows. [S48]
HubSpot says Claude can make mistakes and recommends a person checks anything important. [S48]
Claude's listing carries Anthropic's general caution to only use connectors from developers you trust. [S53]

**Your data and Australia.** HubSpot says Anthropic doesn't use data shared through HubSpot to train its models "except in certain instances", such as feedback or opting in. [S48]
On Team, Enterprise and the API, Anthropic doesn't train on your chats unless you send feedback or otherwise allow it. [S55]
On Free, Pro and Max, a privacy setting called "Help Improve our AI models" controls training, under **Settings** > **Privacy**. [S56]
HubSpot says it respects your data centre while data passes through HubSpot's servers. After that, your Anthropic terms govern where it's processed. [S48]
Anthropic notes that settings for where Claude runs don't change where connected services operate. [S54]
HubSpot may collect summaries of tool calls, with names of people, companies and deals anonymised. [S48]

**Two other Claude routes.** Claude Tag (Claude in Slack, public beta) has its own HubSpot link that an admin sets up with a HubSpot private app token and read scopes. [S57]
It connects with its own credential instead of a person's login. [S57]
Anthropic's Claude for Small Business package (13 May 2026) includes HubSpot-based workflows in Claude Cowork. [S58]

### Microsoft Copilot and HubSpot

Microsoft has renamed Microsoft 365 Copilot to Microsoft Copilot, and Microsoft 365 Copilot Chat to Microsoft Copilot Chat. Some screens still show the old names. [S63]
There are two official routes, and they behave differently. [S59][S60][S61]

**Route 1: the HubSpot Agent for Copilot**

**Official?** Yes, built by HubSpot. [S59]

**What it can see and do.** Read-only. It can't create or edit HubSpot data. [S59]
It reads contacts, companies, deals, tickets, users, line items, quotes, invoices, orders, carts, products, subscriptions, lists, and calls, meetings, notes, tasks and emails. [S59]
It works in Copilot Chat and Copilot in Teams, on web, desktop and mobile. [S59]

**What you need.** Any HubSpot plan. [S59]
HubSpot says you need "a Microsoft 365 Copilot license or the Microsoft 365 Copilot Chat add-on license" with an eligible Microsoft 365 licence. [S59]
A Microsoft 365 admin has to make the agent available, and a HubSpot Super Admin or App Marketplace user makes the first connection. [S59]

**Steps for the Microsoft 365 admin** (HubSpot, 24 September 2026):

1. In the Microsoft 365 admin center, go to **Agents** > **All agents**. [S59]
2. Search for **HubSpot**. [S59]
3. Check its status is **Available**. If not, open it and select **Unblock**. [S59]
4. On the **Users** tab, choose who can install it. **All users in the organization can install** saves people adding it themselves. [S59]

**Steps for each user:**

1. Open Microsoft 365 Copilot Chat, or Copilot in Microsoft Teams. [S59]
2. Under **Agents** in the left sidebar, click **HubSpot**. [S59]
3. Type a prompt, or pick a suggested HubSpot prompt. [S59]
4. When asked, click **Sign in to HubSpot**. [S59]
5. Choose your HubSpot account and permissions, then click **Connect app**. [S59]

**To disconnect.** HubSpot's article only says to disconnect and reconnect if you want a different HubSpot account. It gives no steps. [S59]

**Limits.** One HubSpot account per Copilot account. [S59]
If Sensitive Data is on, it can't see engagement data. [S59]
It can't copy CRM data or whole customer lists. [S59]
HubSpot says Copilot can make mistakes and recommends a person checks the output. [S59]

**Route 2: Microsoft's HubSpot connector (a "federated connector")**

**Official?** Yes. Microsoft lists HubSpot as a Microsoft-published federated connector in its CRM category. [S61]

**What it can see and do.** Federated connectors use MCP to fetch live data with each person's own sign-in. Nothing is copied into Microsoft 365. [S60]
They work in Copilot Chat, agents, Cowork, Copilot in Word, Excel, PowerPoint and Outlook, and the Researcher agent. [S60]
Microsoft started rolling out create, update and delete actions in early October 2026, where a connector provides those tools. They need the user's approval, and Researcher stays read-only. [S60]
Microsoft's docs don't list which HubSpot tools this connector offers. [S60][S61]

**What you need.** Microsoft-published federated connectors are on by default in a Microsoft 365 tenant unless an admin turns them off. [S60]
Admins manage them under **Copilot connectors** > **Your connections** in the Microsoft 365 admin center, and can limit them to groups with **Add staging**. [S60]
With the **Allowed agent types** setting, an admin can keep these connectors off, including future ones, and switch them on one at a time. [S60][S62]

**Steps to connect** (Microsoft, 30 September 2026):

1. Open Microsoft 365 Copilot Chat. [S60]
2. Select the **...** menu, then **Settings**. [S60]
3. Select **Sources**. [S60]
4. Find HubSpot, select **Connect** and sign in with your own HubSpot login. [S60]
5. Ask your question, naming HubSpot in the prompt. [S60]

**To disconnect.** Turn the source off in Researcher or manage it in Copilot Chat settings. Admins can disable the connector for the tenant. [S60]

**Limits.** Microsoft's write approval options are **Allow once**, **Allow for conversation** and **Always allow**. Write tools default to **Needs approval**. [S60]

**Your data and Australia (both routes).** Microsoft says prompts, responses and data accessed through Microsoft Graph aren't used to train its foundation models. [S63][S59]
Once HubSpot data is shared with Copilot, Microsoft's terms govern it. [S59]
For customers outside the EU, Microsoft says queries may be processed in the US, the EU or other regions. [S63]

### Gemini and HubSpot

There are three official routes. [S64][S66][S68] The first two look like the same connector at different stages, but neither vendor says so. That's our inference. [S64][S67][S65]

**Route 1: the HubSpot connector for Gemini**

**Official?** Yes. HubSpot documents it as the "HubSpot connector for Gemini". [S64] Its Google Workspace Marketplace listing, "HubSpot Integration", names Google as the developer. [S67]

**What it can see and do.** Read-only. It fetches contacts, companies and deals, how they link to each other, and their default properties. [S64]
It works in the Gemini app and the Gemini side panel in Gmail, Docs, Sheets and Chat. [S64]
You call it by typing **@HubSpot** before your prompt. [S64]
It can pull lists of contacts, companies or deals by default properties, such as companies in one state. [S64]
It's English only. [S64]

**What you need.** Any HubSpot plan. [S64]
HubSpot says you need a paid Google Workspace Business Standard, Business Plus or Enterprise plan with "Gemini Alpha" turned on, and you connect using the same email you use for Gmail. [S64]
Google has since renamed Gemini Alpha to Gemini Beta. Only an admin can turn it on. [S69]
Google Workspace Marketplace admins control whether the organisation can use the connector. [S64]

**Steps to connect from the Gemini app** (HubSpot, 21 August 2026):

1. Go to gemini.google.com. [S64]
2. Bottom left, click **Settings & Help**, then **Apps**. [S64]
3. Switch **HubSpot** on. [S64]
4. Sign in with your HubSpot login. [S64]

**To disconnect.** gemini.google.com > **Settings & Help** > **Apps** > switch **HubSpot** off > **Disconnect**. [S64]

**Limits.** One HubSpot account per Google Workspace account. [S64]
No access to Sensitive Data properties. [S64]
HubSpot says Gemini can make mistakes and recommends a person checks the output. [S64]
HubSpot's marketing page describes Gemini drafting emails and notes "you can action back in HubSpot". Its help article says the connector can't edit HubSpot data. [S81][S64]

**Route 2: Gemini in Google Workspace integrations**

**Official?** Yes. Google announced on 15 September 2026 that HubSpot is one of seven tools Gemini in Workspace can reach through MCP. [S65]

**What it can see and do.** Google's help says these integrations "currently only support read actions". [S66]
For HubSpot it lists finding contacts or companies and viewing active deal details. [S66]

**What you need.** Google says the feature is on by default for users with Gemini for Workspace access. [S65]
Google's help lists Google AI Pro or Ultra on personal accounts, and Business Standard, Business Plus, Enterprise Standard, Enterprise Plus, Enterprise Essentials, Enterprise Essentials Plus and Google AI Pro for Education on work accounts. [S66]
For work accounts, an admin has to allow integrations. [S66]
Admins manage this at **Apps** > **Google Workspace Marketplace apps** > **Apps list**, for the whole domain, an organisational unit or a group. [S65]

**Steps to connect** (Google, no date shown):

1. On a computer, open the Google Workspace Marketplace integrations page, which is filtered to Gemini integrations. [S66]
2. Select HubSpot. [S66]
3. Click **Connect**. [S66]
4. Follow the on-screen steps to grant access. [S66]
5. In Gmail, Docs or Sheets, open the Gemini panel, type **@** and choose HubSpot. [S66][S64]

**To disconnect.** In your Google Account's security settings, find *Your connections to third-party apps & services* > **See all connections** > the app > **Delete all connections you have with [app]** > **Confirm**. [S66]

**Route 3: Gemini Enterprise**

**Official?** Yes. Google lists HubSpot as a third-party connector for Gemini Enterprise (Business edition), using a Google-managed sign-in app. [S68]

**What it can see and do.** Its listed action is "Manage CRM Objects". Google doesn't say whether that includes writing. [S68]

**Steps to connect** (Google, 16 September 2026):

1. A HubSpot administrator authorises the HubSpot connector in Gemini Enterprise first. [S68]
2. The connector is switched on in Gemini Enterprise under **Settings & help** > **Manage team** > **Connectors**. [S68]
3. Each person then authorises their own HubSpot account. [S68]

**Your data and Australia (all routes).** HubSpot says Google doesn't use data shared through HubSpot to train its models. [S64]
Google's terms govern retention, and your Workspace licence governs where data is processed. [S64]
HubSpot may collect anonymised summaries of tool calls. [S64]

### Any MCP-compatible AI tool and HubSpot (HubSpot's MCP server)

**Official?** Yes, built by HubSpot. Its public beta began on 1 September 2025, and HubSpot called it generally available in April 2026. [S76][S73]

**What it can see and do.** It reads and writes CRM records and activities, landing and website pages, blog posts, campaigns, marketing email drafts, pipelines, custom properties and lists. [S70]
Quotes are in beta, and inbox conversations are read-only. [S70][S74]
Several write tools need the user's explicit confirmation, including creating or updating records and publishing pages. [S70]
Every action respects the person's existing HubSpot permissions. [S70]

**Who it's for.** People building their own agents or connecting AI tools that don't have an official connector. [S71]

**What you need.** A HubSpot user who can open the **Development** area, and an AI tool that supports OAuth with PKCE, which is a secure sign-in handshake. [S70]
HubSpot's MCP overview page says the account admin connects first and other users connect after that. [S72]
The same page says the server doesn't reach custom Sensitive Data properties. [S72]
Some tools need particular plans. AEO tools need Marketing Hub Professional or Enterprise, and quotes need Revenue Hub Professional or Enterprise. [S70]
Free tools accounts can't create custom pipelines. [S70]

**Steps to connect** (HubSpot developer docs, no date shown):

1. In HubSpot, click **Development** in the main navigation. [S70]
2. In the left sidebar, click **MCP Connectors**. [S70]
3. Click **Create MCP connector**. [S70]
4. Fill in **Name**, **Description**, **Redirect URL** (the sign-in return address your AI tool gives you) and **Icon**, then click **Create**. [S70]
5. Copy the client ID, client secret and redirect URL from the connector page. [S70]
6. In your AI tool, add an MCP server at `https://mcp.hubspot.com` using those details. [S70]
7. Sign in, choose the HubSpot account, grant permissions and authorise. [S70]
8. Ask the AI to run `get_user_details` to see what it can reach. [S70]

**To disconnect.** HubSpot's setup page doesn't describe revoking access. [S70]

**Limits.** Searches return up to 200 results a page, and lookups take up to 100 IDs. [S70]
There's no vector search, and the query tool can't join tables. [S70]
Turning on Sensitive Data blocks activities and conversations. [S70]
When HubSpot adds tools, existing users have to reinstall to get the new permissions. [S70][S74]

### Coding agents and HubSpot (Agent CLI and the developer MCP server)

**Official?** Yes, both built by HubSpot. [S78][S77]

**What they can see and do.** The Agent CLI (beta) lets AI coding agents take on repetitive CRM jobs, including analysis and summaries. [S78]
It acts with the connected person's permissions, "which can include creating, updating, or deleting records". [S78]
It can read contacts, companies, deals, tickets, custom objects, workflows, pipelines, properties and activity history. Revenue records are read-only. [S78]
A `--dry-run` option previews changes where it's available. [S78]
The developer MCP server runs on your own computer and helps build HubSpot apps and website content. Its setup page doesn't say it touches CRM data. [S77]

**What you need.** Agent CLI: any HubSpot plan and a compatible coding agent, such as Claude Code, Claude Cowork or the ChatGPT app. A Super Admin has to allow you to connect. [S78]
Claude Cowork Team or Enterprise users may need an admin to allow `api.hubapi.com` first. [S78]
Developer MCP server: HubSpot CLI 8.2.0 or later, and Claude Code, Codex CLI, Cursor, Gemini CLI, VS Code or Windsurf. [S77]

**Steps to connect the Agent CLI** (HubSpot, 26 August 2026):

1. Open your AI coding agent. [S78]
2. Paste HubSpot's install prompt into it. The prompt tells the agent to install the CLI, sign in and add HubSpot's skills. [S78]
3. Sign in to HubSpot when asked. [S78]
4. Review the permissions it asks for. [S78]
5. Click **Connect app**. [S78]

**Steps to set up the developer MCP server** (HubSpot developer docs, no date shown):

1. Check you have HubSpot CLI 8.2.0 or later with `hs --version`, or install it with `npm install -g @hubspot/cli`. [S77]
2. Run `hs mcp setup`. [S77]
3. Pick your tools with the arrow keys and spacebar, then press Enter. [S77]
4. Choose standalone mode or the global CLI. [S77]
5. Restart your coding tool. In Claude Code, `/mcp` should list HubSpotDev. [S77]

**To disconnect.** The Agent CLI article doesn't describe revoking access. It only says Super Admins control who can connect. [S78]

**Limits.** HubSpot recommends starting with reports and analysis before anything that changes data. [S78]

### Your own AI model and HubSpot (the custom LLM workflow action)

**Official?** Yes. HubSpot's "Use a custom LLM" workflow action calls an outside model with your own account key. [S79]

**What it can see and do.** It sends a prompt to the model during a workflow and uses the answer in later steps, for jobs like summarising a record or sorting incoming data. [S79]
It supports OpenAI, Anthropic (Claude), Cohere, xAI (Grok) and Google (Gemini). [S79]

**What you need.** An Enterprise subscription. [S79]
An API key from the AI provider, which for OpenAI must come from an account owner and for Anthropic from an admin or developer. [S79]

**Steps to connect** (HubSpot, 15 July 2026):

1. Go to **More** > **Automation** > **Workflows**. [S79]
2. Open or create a workflow and set its enrolment triggers. [S79]
3. Click the **+** icon and search for **Use a custom LLM**. [S79]
4. In **AI provider**, click **Connect** next to your provider. [S79]
5. Paste your API key and click **Connect to [LLM provider]**. [S79]
6. Choose an **AI model** and write the **Prompt message**. **Advanced settings** has **Temperature** and **Reasoning effort**. [S79]
7. Click **Save**. [S79]

**To disconnect.** Settings icon > **Integrations** > **Connected Apps** > the provider > **Actions** > **Uninstall**. [S79]

**Limits.** HubSpot warns the key gives access to your account with that provider, so keep it secure. [S79]
The article doesn't say what data goes to the provider or who pays for usage. [S79] We'd expect the provider to bill your key directly, but that's an inference.

### Your other apps and HubSpot's AI (agents and Breeze Assistant reaching out)

**Official?** Yes, both directions are HubSpot features. [S35][S34]

**What it can see and do.** Agents built in Agent Builder can connect over MCP to Amplitude, Asana, Atlassian, Box, Canva, Fathom, G2, Gmail, Gong, Google Calendar, Google Chat, Google Drive, Linear, Notion, Slack, Xero and Zapier. Agents can read data there and take actions. [S35]
Each tool can be set to Always allow, Ask permission or Never allow. [S35]
Breeze Assistant can search apps you've installed from the App Marketplace, such as Slack, Gmail, Google Docs and Teams. [S34]

**What you need.** Agent connections: Starter, Professional or Enterprise of Marketing, Sales, Service, Data or Content Hub, or Professional or Enterprise of Smart CRM, plus Agent Builder permissions. [S35]
Breeze Assistant searches: any plan, with Breeze Assistant switched on. [S34]

**Steps to connect apps to Breeze Assistant** (HubSpot, 28 September 2026):

1. In HubSpot's **App Marketplace**, select the app and click **Install**. [S34]
2. Finish the install and read the setup guide in the **Overview** section. [S34]
3. Click **Breeze Assistant** in the top navigation bar. [S34]
4. Use the **Apps** dropdown in the right panel to pick sources, or turn on **Use all apps as sources**. [S34]

The agent connection article describes signing in through on-screen prompts, or pasting a server address for Zapier, but gives no click path. [S35]

**To disconnect.** Agents: the **Connectors** tab in Agent Builder. [S35] Breeze Assistant: uninstall the app, and Breeze Assistant stops using its data. [S34]

**Limits.** HubSpot retired eight Breeze Assistant connectors on 26 September 2026: Smartsheet, GitBook, Azure DevOps, Guru, ReadMe, Productboard, Helpjuice and Document360. [S34]
Prompts can include up to five web addresses. [S34]

### Other AI assistants and HubSpot

HubSpot's AI tools page names only ChatGPT, Claude, Gemini and Copilot. [S81] None of the HubSpot pages we read mention an official connector for other assistants, such as Perplexity or Mistral's Le Chat. We didn't run a separate search for them.
The documented alternative is HubSpot's MCP server, which works with any tool that supports OAuth with PKCE. [S70][S71]
HubSpot's help centre also has a page for a Lovable connector (an AI app builder). It's a private beta and HubSpot marks the page confidential, so we've left the details out. [S83]

## Jobs it's good for

- **Prepare for a sales call.** Ask Claude or ChatGPT for the company, its open deals and the latest emails and meetings. Both can read engagement history unless Sensitive Data is on. [S48][S43] On any plan, Breeze Assistant can summarise a record, or prepare you for meetings once your calendar's connected. [S2][S25]
- **Log the call straight after.** Tell ChatGPT or Claude what was agreed and have it add a note and a follow-up task. It shows the change and waits for your yes. [S43][S48]
- **A Monday pipeline check.** Ask for open deals by stage, with a chart. Claude and Breeze Assistant can both chart CRM data. [S49][S2]
- **Tidy up a handful of records.** Up to 10 at a time through ChatGPT or Claude. Check the result, since ChatGPT skips your custom validation rules. [S43][S48]
- **A weekly digest.** Schedule a Breeze Assistant prompt to run every Monday. It lands as a new chat. [S74]
- **Answer website chats after hours.** The customer agent answers from your help articles and website pages and hands over to a person when it's unsure. Professional plan or above, paid per resolved conversation. [S17][S18][S12]
- **Fill in missing company details.** Data enrichment fills fields like industry and job title from Starter up, without credits. [S22] For questions enrichment can't answer, a smart property researches each record for 10 credits a response. [S21][S12]
- **Turn meetings into notes and deal updates.** Notetaker records Zoom, Teams or Google Meet calls, and deal progression suggests field changes for you to approve. Sales Hub or Service Hub Professional. [S26][S27]
- **First drafts of content.** Breeze Assistant has guides for drafting blog posts and landing pages. [S84] The content agent drafts posts and campaign assets on Marketing Hub Professional and never publishes by itself. [S28]
- **Check a campaign's results.** Ask Claude or ChatGPT about a campaign by name and date range. [S48][S43]
- **Find holes in your help centre.** The knowledge base agent reads closed tickets and drafts the missing articles for review. Service Hub Professional, 200 credits an article. [S30][S12]
- **Look up a deal without leaving Teams.** The HubSpot Agent for Copilot answers in Copilot Chat and Teams. [S59]
- **Pull a list into a Google Doc or Sheet.** In the Gemini side panel, @HubSpot can fetch contacts at a lifecycle stage. [S64]
- **Turn a manual process into a workflow.** Describe it to Breeze Assistant on Professional. The workflow arrives switched off for you to check first. [S31]

## What to watch for

**Switches that are on until someone turns them off**

- **AI Model Training** is on, so HubSpot may train its models on your customer data. Turning it off only works going forward. [S3][S5]
- Breeze Assistant is on for every user, and AI can use your CRM and conversation data. [S3][S4]
- In a Microsoft 365 tenant, Microsoft's own federated connectors, HubSpot included, are on unless an admin turns them off. [S60][S61]
- In Google Workspace, Gemini's tool integrations, HubSpot included, are on for users with Gemini for Workspace access. [S65]
- Microsoft's and Google's docs don't say whether HubSpot's app approval step applies to their routes. [S60][S65][S66] We'd check this before assuming HubSpot's approval protects you. That's our inference.

**Who can connect outside AI**

- Anyone with the **App Marketplace Access** permission can connect ChatGPT or Claude without asking. That includes agencies and consultants who hold it. [S43][S48]
- Super Admins can review connection attempts in the audit log. [S43][S48]
- Revoking approval uninstalls the app for everyone. Removing one person can take up to 30 minutes. [S80]

**AI that writes to your CRM or talks to customers**

- With **Always allow** set, ChatGPT and Claude can edit records without asking. HubSpot recommends **Needs Approval**. [S43][S48]
- The ChatGPT connector skips your custom validation rules. Claude applies pipeline stage checks but not association label checks. [S43][S48]
- The connectors can't delete records. The Agent CLI can, within the person's permissions. [S43][S48][S78]
- Breeze Assistant can create deals, notes, products and workflows within each person's permissions. [S2]
- The prospecting agent can send emails without anyone reading them if you choose **Send automatically**. [S20]
- The customer agent talks to customers directly. Its chat replies carry a "Powered by AI" label. [S17]
- Deal progression asks for approval by default, but automatic updates can be switched on. [S27]

**Customer personal information**

- For Australian-hosted accounts, HubSpot lists its AI providers as processing in the United States. [S9]
- New sub-processors for HubSpot AI start on 16 October 2026. HubSpot promises at least 30 days' notice of sub-processor changes to customers who opt in to notifications. [S9]
- Notetaker recordings are kept for two years, and HubSpot puts recording consent on you. [S26]
- Once data reaches ChatGPT, Claude, Copilot or Gemini, that vendor's terms apply. [S43][S48][S59][S64]
- On personal ChatGPT and Claude plans, whether your connector data can be used for training depends on your plan and privacy settings. [S43][S56]
- HubSpot may keep anonymised summaries of what the AI asked for through its connectors. [S48][S59][S64]
- Sensitive Data (Enterprise only) blocks engagement data from the connectors, and it opts you out of model training. [S36][S43][S48][S59][S5]
- The knowledge base agent reads every conversation on closed tickets. [S30]
- Data enrichment may feed limited business contact data back into HubSpot's dataset. [S22]
- HubSpot advises keeping sensitive information out of data agent prompts. [S21]
- Breeze Assistant artifacts can be shared through a public link. [S2]

**Accuracy and checking**

- HubSpot says Claude, Gemini and Copilot can all make mistakes. It recommends a person checks anything important, and suggests asking the AI for citations. [S48][S64][S59]
- Microsoft says generated responses "aren't guaranteed to be 100% factual". [S63]
- Record summaries only cover what's been logged. [S25]
- Credit estimates from test runs can differ from what an agent actually spends. [S14]

**Cost surprises**

- Every AI agent has used credits since 23 July 2026. [S14]
- On credit packs bought from 16 September 2026, extra use is billed as overage by default. It arrives monthly in arrears on its own invoice. [S11]
- Once you buy packs, HubSpot sets an account spend limit 50% above your monthly credits. Limits for individual features aren't on by default. [S11]
- Without packs, credit-using features pause when credits run out. [S11]
- Billing contacts and Super Admins get alerts at 75%, 85% and 90% of credits used. [S11]
- Unused credits expire each month. [S11]
- Some features charge credits when switched on and again monthly while they stay on. [S12]
- Phone minutes and SMS used by agents are charged separately. [S12]
- If a customer replies to an email more than 72 hours later, the customer agent's conversation reopens and can cost credits again. [S17]
- Beta features may start costing credits later. HubSpot aims for 30 days' notice but says that may not always happen. [S11]
- Test runs are free, and each agent can have a monthly run limit. [S14]

## Announced changes

| Date | Change | Source |
|---|---|---|
| 4 Jun 2025 | HubSpot's ChatGPT connector launched for deep research | [S44] |
| 24 Jul 2025 | ChatGPT connector added everyday chat | [S45] |
| 29 Jul 2025 | HubSpot connector for Claude launched | [S49] |
| 11 Aug 2025 | OpenAI made the HubSpot connector available in chat for Plus | [S90] |
| 1 Sep 2025 | HubSpot's remote MCP server entered public beta | [S76] |
| 20 Nov 2025 | Claude connector gained write access (beta at the time) and engagement history | [S50] |
| 13 Jan 2026 | Self-service MCP connector setup ("MCP Auth Apps") entered public beta, announced 20 Jan | [S76] |
| 14 Apr 2026 | Remote and developer MCP servers generally available; App Install Governance Tool in public beta | [S73] |
| 14 Apr 2026 | Customer and prospecting agents moved to pay-per-outcome pricing | [S42] |
| 14 Apr 2026 | Notetaker's custom field capture started costing 10 credits per run | [S26] |
| 13 May 2026 | Anthropic launched Claude for Small Business, with HubSpot workflows | [S58] |
| 29 Jun 2026 | MCP server can create, edit and publish landing pages | [S75] |
| 9 Jul 2026 | OpenAI replaced ChatGPT's App Directory with a Plugin Directory; existing app connections carried on | [S90] |
| 13 Jul 2026 | Custom assistants retired and moved into Breeze projects | [S33] |
| 23 Jul 2026 | All AI agents now use credits; five agents retired; Agent Hub and Agent Builder in public beta | [S14][S15][S16] |
| 25 Aug 2026 | Microsoft retired the PowerShell switch for federated connectors in favour of **Allowed agent types** | [S62] |
| 31 Aug 2026 | Notetaker and video call recordings now only create meeting records | [S26] |
| 15 Sep 2026 | MCP server and Claude connector expanded (custom objects, quotes beta, inbox conversations); Breeze Assistant can build agents (beta) and run scheduled prompts | [S74] |
| 15 Sep 2026 | Google added HubSpot to Gemini in Workspace, on by default (post corrected 30 Sep) | [S65] |
| 16 Sep 2026 | Fall 2026 Spotlight: rebuilt Breeze Assistant, Marketing Studio, updated prospecting agent, mobile Notetaker | [S41] |
| 16 Sep 2026 | ChatGPT Ads integration (beta) and a HubSpot and OpenAI "AI Growth Bundle" for new customers | [S46][S47] |
| 16 Sep 2026 | New credit packs default to pay-as-you-go overage | [S11] |
| 16 Sep 2026 | Customer agent voice billing began | [S19] |
| 26 Sep 2026 | Eight Breeze Assistant app connectors retired | [S34] |
| Early Oct 2026 | Microsoft began rolling out write actions for federated connectors | [S60] |
| 16 Oct 2026 | Baseten, Bright Data and Exa Labs become HubSpot AI sub-processors, processing in the US | [S9] |
| 31 Oct 2026 | Sign-up deadline for ChatGPT ad credits in the AI Growth Bundle; the offer page names US and EU advertisers | [S82] |
| Not dated | Commerce Hub renamed Revenue Hub | [S40] |
| Not dated | Microsoft 365 Copilot renamed Microsoft Copilot (page dated 9 Jul 2026) | [S63] |
| Not dated | Google renamed Gemini Alpha to Gemini Beta (page updated 13 Oct 2026) | [S69] |

## What we couldn't establish

- **AUD prices.** We couldn't load HubSpot's AUD plan prices. The pages we read showed US dollars, and HubSpot's catalogue prices extra credits in US dollars only. [S39][S12][S13]
- **Which ChatGPT plans can use the HubSpot plugin today.** OpenAI's pages say it depends on plan, workspace, role and region, and its HubSpot page lists no plans. [S85][S87] In 2025 HubSpot noted chat wasn't available on Plus. [S45] OpenAI's release notes show chat reached Plus on 11 August 2025, but no current OpenAI page names plans for it. [S90]
- **Whether Starter can build custom agents.** HubSpot's Agent Hub article includes Starter [S1], and its setup guide lists Agent Builder from Starter up. [S4] Its Breeze Assistant article, news post and developer changelog say Professional or Enterprise. [S2][S16][S74]
- **Trial lengths and plans for two agents.** The customer agent article says 14 days free [S17], but HubSpot's April news post said 28 days. [S42] The prospecting agent article includes Starter [S20], but the news post said Professional and Enterprise. [S42]
- **How long Breeze Assistant keeps chats, memories and artifacts.** Not stated. [S2][S33]
- **How HubSpot reaches Anthropic's models.** Its model cards list Claude models [S8], but Anthropic isn't on its sub-processor list. [S9]
- **Whether connector traffic for Australian-hosted accounts stays in Sydney** before it reaches the AI vendor. HubSpot says it respects your data centre, with no Australia-specific detail. [S43][S48]
- **Microsoft's HubSpot federated connector.** We couldn't find which HubSpot tools it exposes, whether write actions are live for HubSpot, which licence it needs, or whether HubSpot's approval step applies. [S60][S61]
- **Removing the HubSpot Agent for Copilot.** HubSpot's article has no steps. [S59]
- **Which Gemini rules apply now.** HubSpot's article (21 August) requires Gemini Alpha. Google's September launch says it's on by default for Gemini for Workspace users. [S64][S65][S69] We also couldn't confirm whether the Gemini Enterprise connector can write. [S68]
- **Revoking an MCP connector.** HubSpot's setup page doesn't cover it. [S70]
- **Claude's Free plan.** HubSpot says a paid Claude plan is needed [S48], while Anthropic says directory connectors are available to all users. [S54] We didn't test it.
- **Data enrichment and credits.** The enrichment article says no credits [S22]. HubSpot's setup guide marks the data enrichment permission as credit-using, which may be because it covers buyer intent too. [S4]
- **Whether "Breeze Intelligence" is still sold under that name.** Current help articles don't use it. [S22]
- **Australian availability of ChatGPT Ads and the AI Growth Bundle.** Neither page mentions Australia. [S47][S82]
- **AI-specific certifications.** HubSpot's AI trust page mentions independent audits but names no AI standard such as ISO 42001. [S7]
- **The Lovable connector.** It's a private beta, and HubSpot marks the page confidential. [S83]
- **Connectors for other AI assistants.** Our web search allowance ran out partway through, so we didn't search separately for official HubSpot links to Perplexity, Mistral or other assistants. The HubSpot pages we read name only the four covered here. [S81]

## Sources

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Understand Agent Hub (reached via the old "Understand Breeze" link, /ai/understand-breeze) | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/understand-agent-hub | 16 Sep 2026 | 15 Oct 2026 |
| S2 | Use Breeze Assistant | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/use-breeze-assistant | 16 Sep 2026 | 15 Oct 2026 |
| S3 | Manage AI settings | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-management/manage-your-ai-settings | 8 Sep 2026 | 15 Oct 2026 |
| S4 | Set up a HubSpot account to adopt AI features | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/set-up-a-hubspot-account-to-adopt-ai-features | 16 Sep 2026 | 15 Oct 2026 |
| S5 | Understand HubSpot's AI model training | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-management/hubspot-ai-mode-training | 8 Sep 2026 | 15 Oct 2026 |
| S6 | HubSpot AI Cloud Infrastructure: Frequently Asked Questions | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-security/hubspot-ai-cloud-infrastructure-frequently-asked-questions | 21 Jul 2026 | 15 Oct 2026 |
| S7 | HubSpot's AI Trust and Safety | HubSpot | https://www.hubspot.com/products/artificial-intelligence/ai-trust | No date shown | 15 Oct 2026 |
| S8 | HubSpot's AI Model Cards | HubSpot Trust Center | https://trust.hubspot.com/ai | No date shown | 15 Oct 2026 |
| S9 | HubSpot Sub-Processors Page | HubSpot Legal | https://legal.hubspot.com/sub-processors-page | 16 Sep 2026 | 15 Oct 2026 |
| S10 | HubSpot Cloud Infrastructure and Data Hosting: Frequently Asked Questions | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-security/hubspot-cloud-infrastructure-and-data-hosting-frequently-asked-questions | 24 Jul 2026 | 15 Oct 2026 |
| S11 | Manage HubSpot Credits | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-management/understand-hubspot-credits-and-billing | 16 Sep 2026 | 15 Oct 2026 |
| S12 | HubSpot Product & Services Catalog | HubSpot Legal | https://legal.hubspot.com/hubspot-product-and-services-catalog | No date shown | 15 Oct 2026 |
| S13 | HubSpot Credits (Put HubSpot to work for you with credits) | HubSpot | https://www.hubspot.com/products/artificial-intelligence/credits | No date shown | 15 Oct 2026 |
| S14 | Test and control agent credit usage | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/test-and-control-agent-credit-usage | 29 Sep 2026 | 15 Oct 2026 |
| S15 | Install agents from the Agent Marketplace | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/install-agents-from-the-agent-marketplace | 16 Sep 2026 | 15 Oct 2026 |
| S16 | Meet Agent Hub and Agent Builder: One place to build and manage AI agents with shared context | HubSpot Newsroom | https://www.hubspot.com/company-news/meet-agent-hub-and-agent-builder | Updated 23 Jul 2026 | 15 Oct 2026 |
| S17 | Understand the customer agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/customer-agent/understand-the-customer-agent | 16 Sep 2026 | 15 Oct 2026 |
| S18 | Set up the customer agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/customer-agent/set-up-the-customer-agent | 16 Sep 2026 | 15 Oct 2026 |
| S19 | Set up customer agent voice | HubSpot Knowledge Base | https://knowledge.hubspot.com/calling/set-up-customer-agent-voice | 16 Sep 2026 | 15 Oct 2026 |
| S20 | Set up and use the prospecting agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/prospecting/use-the-prospecting-agent | 16 Sep 2026 | 15 Oct 2026 |
| S21 | Set up and use the data agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/data-management/use-data-agent | 13 Oct 2026 | 15 Oct 2026 |
| S22 | Get started with data enrichment | HubSpot Knowledge Base | https://knowledge.hubspot.com/records/get-started-with-data-enrichment | 10 Jul 2026 | 15 Oct 2026 |
| S23 | Manage data enrichment settings | HubSpot Knowledge Base | https://knowledge.hubspot.com/records/manage-data-enrichment-settings | 31 Jul 2026 | 15 Oct 2026 |
| S24 | Generate and refine content with AI | HubSpot Knowledge Base | https://knowledge.hubspot.com/website-pages/generate-content-with-breeze | 10 Sep 2026 | 15 Oct 2026 |
| S25 | Summarize a record | HubSpot Knowledge Base | https://knowledge.hubspot.com/records/summarize-records | 21 Sep 2026 | 15 Oct 2026 |
| S26 | Record and take notes in meetings with Notetaker | HubSpot Knowledge Base | https://knowledge.hubspot.com/meetings-tool/record-and-take-notes-in-meetings-with-meeting-notetaker | 16 Sep 2026 | 15 Oct 2026 |
| S27 | Move deals forward with deal progression | HubSpot Knowledge Base | https://knowledge.hubspot.com/records/move-deals-forward-with-deal-progression | 1 Oct 2026 | 15 Oct 2026 |
| S28 | Create content with content agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/website-and-landing-pages/create-content-with-content-agent | 16 Sep 2026 | 15 Oct 2026 |
| S29 | Set up and analyze AEO | HubSpot Knowledge Base | https://knowledge.hubspot.com/seo/set-up-and-analyze-ai-visibility | 27 Aug 2026 | 15 Oct 2026 |
| S30 | Set up and manage a knowledge base agent | HubSpot Knowledge Base | https://knowledge.hubspot.com/knowledge-base/create-a-knowledge-base-agent | 16 Sep 2026 | 15 Oct 2026 |
| S31 | Build workflows using Breeze Assistant | HubSpot Knowledge Base | https://knowledge.hubspot.com/workflows/use-ai-assistants-in-workflows | 3 Aug 2026 | 15 Oct 2026 |
| S32 | Manage AI context with knowledge vaults | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/manage-breeze-context-with-knowledge-vaults | 21 Aug 2026 | 15 Oct 2026 |
| S33 | Create and manage projects in Breeze Assistant | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/create-and-manage-breeze-projects | 16 Sep 2026 | 15 Oct 2026 |
| S34 | Search connected apps with Breeze Assistant | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai-tools/use-breeze-assistant-with-connected-apps | 28 Sep 2026 | 15 Oct 2026 |
| S35 | Connect apps to HubSpot's AI agents | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/customize-breeze-agents-with-hubspot-mcp-client | 18 Sep 2026 | 15 Oct 2026 |
| S36 | Store Sensitive Data in HubSpot | HubSpot Knowledge Base | https://knowledge.hubspot.com/account-security/store-sensitive-data | 8 Sep 2026 | 15 Oct 2026 |
| S37 | Free AI Assistant for Every Team: HubSpot Breeze Assistant | HubSpot | https://www.hubspot.com/products/artificial-intelligence/breeze-ai-assistant | No date shown | 15 Oct 2026 |
| S38 | Run, Build, and Manage Your AI Agents: Agent Hub | HubSpot | https://www.hubspot.com/products/artificial-intelligence | No date shown | 15 Oct 2026 |
| S39 | HubSpot Starter: For Startups & Small Businesses | HubSpot | https://www.hubspot.com/products/crm/starter | No date shown | 15 Oct 2026 |
| S40 | CPQ, Billing & Payments Software: HubSpot Revenue Hub | HubSpot | https://www.hubspot.com/products/revenue | No date shown | 15 Oct 2026 |
| S41 | Fall 2026 Spotlight: HubSpot just made its most foundational product release | HubSpot Newsroom | https://www.hubspot.com/company-news/fall-26-spotlight | Updated 16 Sep 2026 | 15 Oct 2026 |
| S42 | HubSpot's Customer Agent and Prospecting Agent: Now you pay when the task is complete | HubSpot Newsroom | https://www.hubspot.com/company-news/hubspots-customer-agent-and-prospecting-agent-now-you-pay-when-the-task-is-complete | Updated 13 Apr 2026 | 15 Oct 2026 |
| S43 | Set up and use the HubSpot connector for ChatGPT | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/connect-your-hubspot-account-to-chatgpt | 28 Sep 2026 | 15 Oct 2026 |
| S44 | HubSpot launches first CRM deep research connector with ChatGPT | HubSpot Newsroom | https://www.hubspot.com/company-news/hubspot-deep-research-connector-for-chatgpt | Updated 4 Jun 2025 | 15 Oct 2026 |
| S45 | Expanding the HubSpot connector for ChatGPT | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/hubspot-connector-chatgpt | 24 Jul 2025 | 15 Oct 2026 |
| S46 | HubSpot and OpenAI deepen partnership to bring AI transformation to every SMB | HubSpot Newsroom | https://www.hubspot.com/company-news/hubspot-and-openai-deepen-partnership | Updated 16 Sep 2026 | 15 Oct 2026 |
| S47 | Connect and manage ChatGPT Ads account in HubSpot | HubSpot Knowledge Base | https://knowledge.hubspot.com/connect-and-manage-chatgpt-ads-account-in-hubspot | 15 Sep 2026 | 15 Oct 2026 |
| S48 | Set up and use the HubSpot connector for Claude | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/set-up-and-use-the-hubspot-connector-for-claude | 17 Sep 2026 | 15 Oct 2026 |
| S49 | HubSpot launches first CRM connector for Anthropic's Claude | HubSpot Newsroom | https://www.hubspot.com/company-news/hubspot-connector-claude | Updated 29 Jul 2025 | 15 Oct 2026 |
| S50 | Take Action With Claude: Update CRM Records and Access Engagement History | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/claude-write-access-to-crm | 20 Nov 2025 | 15 Oct 2026 |
| S51 | Get started with connectors | Anthropic (Claude docs) | https://claude.com/docs/connectors/getting-started | No date shown | 15 Oct 2026 |
| S52 | Connectors directory | Anthropic (Claude docs) | https://claude.com/docs/connectors/directory | No date shown | 15 Oct 2026 |
| S53 | HubSpot connector (Claude directory listing) | Anthropic | https://claude.com/connectors/hubspot | No date shown (listing says added November 2025) | 15 Oct 2026 |
| S54 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated over 2 weeks ago" (no calendar date) | 15 Oct 2026 |
| S55 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | 18 Aug 2026 | 15 Oct 2026 |
| S56 | How do I change my model improvement privacy settings? | Anthropic Privacy Center | https://privacy.claude.com/en/articles/12109829-how-do-i-change-my-model-improvement-privacy-settings | 3 Aug 2026 | 15 Oct 2026 |
| S57 | Connect HubSpot (Claude Tag) | Anthropic (Claude docs) | https://claude.com/docs/claude-tag/admins/connections/hubspot | No date shown | 15 Oct 2026 |
| S58 | Introducing Claude for Small Business | Anthropic | https://www.anthropic.com/news/claude-for-small-business | 13 May 2026 | 15 Oct 2026 |
| S59 | Set up and use the HubSpot Agent for Copilot | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/set-up-and-use-the-hubspot-agent-for-copilot | 24 Sep 2026 | 15 Oct 2026 |
| S60 | Federated connectors overview: Microsoft 365 Copilot connectors | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | 30 Sep 2026 | 15 Oct 2026 |
| S61 | Microsoft-built connectors gallery: Microsoft 365 Copilot connectors | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 30 Sep 2026 | 15 Oct 2026 |
| S62 | Manage federated connector availability | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-federated-connectors | 28 Apr 2026 | 15 Oct 2026 |
| S63 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy | 9 Jul 2026 | 15 Oct 2026 |
| S64 | Set up and use the HubSpot connector for Gemini | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/set-up-and-use-hubspot-connector-for-gemini | 21 Aug 2026 | 15 Oct 2026 |
| S65 | Connect to more tools with Gemini in Google Workspace | Google Workspace Updates | https://workspaceupdates.googleblog.com/2026/09/connect-to-more-tools-with-gemini-in-Google-Workspace.html | 15 Sep 2026 (corrected 30 Sep 2026) | 15 Oct 2026 |
| S66 | Use integrations with Gemini in Workspace | Google Docs Editors Help | https://support.google.com/docs/answer/16796422?hl=en | No date shown | 15 Oct 2026 |
| S67 | HubSpot Integration (Google Workspace Marketplace listing) | Google | https://workspace.google.com/marketplace/app/hubspot_integration/584788731981 | 26 Aug 2026 | 15 Oct 2026 |
| S68 | Connect your Google apps and third-party data (Gemini Enterprise) | Google | https://support.google.com/g/answer/16550932?hl=en | 16 Sep 2026 | 15 Oct 2026 |
| S69 | Turn access to Google Workspace with Gemini Beta on or off | Google Workspace Help | https://knowledge.workspace.google.com/admin/gemini/turn-access-to-google-workspace-with-gemini-alpha-on-or-off | 13 Oct 2026 | 15 Oct 2026 |
| S70 | Integrate AI tools with the HubSpot MCP server | HubSpot Developer Docs | https://developers.hubspot.com/docs/apps/developer-platform/build-apps/integrate-with-the-remote-hubspot-mcp-server | No date shown | 15 Oct 2026 |
| S71 | Using the HubSpot MCP server | HubSpot Developer Docs | https://developers.hubspot.com/docs/build-with-ai/remote-mcp-server | No date shown | 15 Oct 2026 |
| S72 | HubSpot MCP Server | HubSpot Developers | https://developers.hubspot.com/ai-tools/mcp | No date shown | 15 Oct 2026 |
| S73 | Spring 2026 Spotlight | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/spring-2026-spotlight | 14 Apr 2026 | 15 Oct 2026 |
| S74 | Fall 2026 Spotlight: Developer / Builder Updates | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/fall-2026-spotlight | 15 Sep 2026 | 15 Oct 2026 |
| S75 | Developer updates for June 2026 | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/june-2026-rollup | 29 Jun 2026 | 15 Oct 2026 |
| S76 | Public Beta: Self-Service MCP Auth Apps for the HubSpot Remote MCP Server | HubSpot Developer Changelog | https://developers.hubspot.com/changelog/public-beta-self-service-mcp-auth-apps-for-the-hubspot-remote-mcp-server | 20 Jan 2026 | 15 Oct 2026 |
| S77 | Set up the developer MCP server | HubSpot Developer Docs | https://developers.hubspot.com/docs/developer-tooling/local-development/developer-mcp/setup | No date shown | 15 Oct 2026 |
| S78 | Use the HubSpot Agent CLI | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/use-the-hubspot-agent-cli | 26 Aug 2026 | 15 Oct 2026 |
| S79 | Create and use custom LLM workflow actions | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/create-and-use-custom-llm-workflow-actions | 15 Jul 2026 | 15 Oct 2026 |
| S80 | Manage access to apps | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/manage-access-to-ai-connectors | 10 Sep 2026 | 15 Oct 2026 |
| S81 | Your HubSpot context in every AI tool | HubSpot | https://www.hubspot.com/ai-tools | No date shown | 15 Oct 2026 |
| S82 | AI Growth Bundle offer page | HubSpot | https://offers.hubspot.com/ai-growth-bundle | No date shown | 15 Oct 2026 |
| S83 | Build apps with the HubSpot connector for Lovable (private beta, marked confidential; don't publish details) | HubSpot Knowledge Base | https://knowledge.hubspot.com/integrations/hubspot-connector-for-lovable | 15 Sep 2026 | 15 Oct 2026 |
| S84 | AI Topics (index of HubSpot's AI help articles) | HubSpot Knowledge Base | https://knowledge.hubspot.com/ai/topics | No date shown | 15 Oct 2026 |
| S85 | HubSpot plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/hubspot/ | No date shown | 15 Oct 2026 |
| S86 | HubSpot (ChatGPT plugin listing) | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_697acb8e53d88191bf7a79e62012ae14 | No date shown; version 6.0.0 | 15 Oct 2026 |
| S87 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S88 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S89 | Admin controls, security, and compliance for plugins and apps | OpenAI Help Center | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S90 | ChatGPT release notes | OpenAI Help Center | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
| S91 | Managing app permissions in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001495-managing-app-permissions-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
