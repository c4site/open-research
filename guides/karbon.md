# Karbon: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Karbon's built-in AI is called Karbon AI. It summarises emails and client histories, drafts emails and suggests who to assign work to. [S2] [S8]
- Karbon AI has been available to all customers since 31 March 2026, at no extra cost for now. It's switched on for everyone by default, and an admin can turn it off for the whole firm. [S8] [S2] [S15]
- Karbon says its AI runs on Microsoft's Azure OpenAI Service and isn't trained on your firm's data. It processes data only in the region where your Karbon data is stored. [S2] [S8] [S16]
- In Triage, AI labels can sort incoming email and, if you set it up, clear, assign or draft replies to emails automatically. [S19]
- Kai, Karbon's "AI coworker", and its AI Agents are in early access. Karbon says Kai's actions wait for your sign-off. [S3] [S4]
- We found no official connection between Karbon and Claude, ChatGPT, Microsoft Copilot or Google Gemini. [S35] [S37] [S39] [S42]
- Karbon announced a public MCP server in June 2026 so firms can bring Karbon data into other AI tools. Its developer docs list the address but no instructions. [S5] [S32]
- For your own tools, the Karbon API comes with the Business and Enterprise plans. [S1] [S32]
- Karbon's AI terms were last updated in September 2023. They don't mention Kai or AI Agents. [S7]

## The tool, and the plans that matter

Karbon is practice management software for accounting and bookkeeping firms. It brings email, workflow, client records, billing and a client portal together. [S1]

Karbon says it has customers in 34 countries, and its team is based in the US, Australia, New Zealand, Canada and the UK. [S27]

These are the prices on Karbon's pricing page with Australian dollars selected, as read on 17 October 2026. Prices are per user, per month. [S1]

| Plan | Paid annually (AUD, excl. GST) | Paid monthly (AUD, excl. GST) | What the plan adds |
|---|---|---|---|
| Team | $59 | $79 | Integrated email, collaboration, workflow, time tracking and budgets, billing, payments and engagements. No Karbon API. |
| Business | $89 | $109 | Everything in Team, plus automatic client reminders, task automation, industry integrations and the Karbon API. |
| Enterprise | Custom pricing | Custom pricing | Everything in Business, plus an enterprise platform, a dedicated Karbon contact, customisation and "Unlimited Usage Limits". |

Sources for the table: [S1]

- With AUD selected, the page says "All prices exclude GST." [S1]
- Monthly billing is "only available for teams of 4+". [S1]
- Karbon says you can pay in Australian dollars, depending on your location. [S1]
- Karbon's machine-readable copy of its pricing says it was last updated on 30 June 2026. [S43]
- The pricing page doesn't list AI by plan. Karbon's AI page says Karbon AI "is currently available to all Karbon customers at no additional cost". [S1] [S2]
- Karbon says it will announce any future AI pricing to customers in advance. [S2]
- Kai and AI Agents are in early access. We didn't find a price for either. [S3] [S4]
- Karbon's period close product, Aider, is sold through a demo. We didn't find its price. [S12] [S14]
- Enterprise customers can choose "dedicated data hosting in an Azure local cloud center". [S25]

## AI built in

Karbon groups its AI on one page, under Karbon AI, Kai, Agentic Workflows and Meeting Intelligence. [S2]

### Karbon AI (summaries, drafting and suggestions)

**What it does**

- **Client Summary** puts emails, notes, work and billing data into a single client brief. Since March 2026 it draws on more than 100 notes and timeline entries. [S2] [S8]
- **Work Conversations Summary** gives the highlights and recent updates on any work item. [S2]
- **Email Summary** shortens long email threads and internal discussions. [S2]
- **Compose and Refine Emails** drafts and improves emails, with options for tone, length and language. [S2]
- **Quick Replies** offers editable suggested replies. **Create Email from Tasks** drafts a client email from your progress on tasks. [S2]
- **Smart Suggestions** suggests colleagues and contacts to assign, based on past work. [S2]
- **Time-Tracking** flags missed time entries based on the tasks you completed. [S2]

**Where to find it**

- Karbon describes these features inside its email, work, client and time tracking areas. The pages we read don't give menu paths for each one. [S2]
- Karbon's help centre lists three Karbon AI articles: an overview, a security note and an access note. We read the security and access notes, but couldn't find a working link to the overview. [S17] [S15] [S16]

**Which plans have it**

- Karbon's AI page says the features are available across paid plans and need an active subscription. [S2]
- Karbon AI became available to all customers on 31 March 2026. [S8] [S9]
- A Karbon help article dated September 2026 still asks users for feedback "before the full release". [S15]

**What happens to your data**

- Karbon says "Karbon AI is built on the Azure OpenAI Service." [S2] [S16]
- Karbon says "Karbon does not use your firm's data to train AI models." [S2]
- Karbon's AI terms say Karbon "is not authorized to train the Karbon AI, with or without client/customer data", and that OpenAI and Azure OpenAI "have represented that neither will use client/customer data to train the AI models". [S7]
- The same terms say Microsoft will process and store what you submit to Karbon AI, and its output, to monitor for abuse. Authorised Microsoft staff "may review data that has triggered its automated systems." [S7]
- Since March 2026, Karbon says its AI features "process data exclusively within the region where your Karbon data is stored", so there are no cross-region transfers. [S8]
- Karbon AI is on for all users by default. Account admins can turn it off for the whole firm in Settings > Karbon AI > Enable Karbon AI. [S2] [S15]
- We found no setting to turn it off for one person. [S2] [S15]

**In Australia**

- The AI page's example of in-region processing is UK data staying in the UK. It doesn't name Australia. [S2]
- Karbon's status page has referred to "the Australian domain". That suggests Australian firms run on a separate Australian instance. That's our inference; Karbon's pages we read don't say where Australian data is stored. [S26]
- Karbon offers AUD pricing, and its help articles use Australian examples such as ATO notices. [S1] [S19]

### AI labels and actions in Triage

**What it does**

- Karbon's AI Categorization reads emails arriving in Triage and labels them, such as High Priority, Client Query or FYI. [S19]
- You can attach one optional action to each label. When the AI applies the label, the action runs automatically. [S19]
- The actions are Clear, Add to My Week, Add to My Week and Clear, Save for Later, Assign, Assign and Clear, and Draft Reply to All. In Shared Triage, only Clear and the Assign actions are offered. [S19]
- An action only runs if the AI is at least 80% confident the label fits. If an email matches several labels, only the most confident label's action runs. [S19]
- Assign actions only run when the email is already linked to a contact or work item in Karbon. [S19]
- Draft Reply to All writes a draft using the whole conversation and your composer settings. It won't overwrite a draft that's already there. [S19]
- When an action runs, Karbon adds a timestamped entry to the email's timeline, so you can see what the AI did. [S19]
- Hover over a label to see why the AI applied it. [S18]

**Where to find it**

- For your own Triage, click your name in the side menu, then Email Labels. [S19]
- For a Shared Triage, an admin goes to Settings > Shared Triage, selects the Shared Triage, then Email Labels. [S19]
- To add an action, edit a label, turn Action from Off to On, pick the action and click Save. Turn Action back to Off to remove it. [S19]
- You start with five labels and can have up to 25. High Priority is a system label you can rename but can't delete. [S19]

**Which plans have it**

- The help article doesn't say which plans include AI labels. [S19]

**What happens to your data**

- The AI reads each email's subject, body and sender to decide on a label. [S19]
- Activity from Assign actions is visible to everyone on the conversation. Activity from other actions is visible only to you. [S19]
- The article doesn't say whether the firm-wide Karbon AI switch also turns off labels. [S19] [S15]

**In Australia**

- The help article's own examples include an "ATO Notice" label and emails about STP submissions. [S19]

### Kai, the AI coworker (early access)

**What it does**

- Karbon describes Kai as "The AI coworker that knows your firm and works like part of your team." [S3]
- Kai answers questions from your live Karbon data and serves up client summaries, work status and items at risk. [S3]
- Karbon says Kai can handle tasks such as "workpaper creation, timesheet review, and work prioritization". [S3]
- At launch, Karbon said Kai can help you expand and price services and take on repetitive tasks, through a chat interface. [S5]

**Where to find it**

- Kai is built into Karbon. A June 2026 release note says Karbon's refreshed header lays the groundwork for "upcoming innovations, including Kai". [S3] [S10]

**Which plans have it**

- Karbon says Kai is "available to Karbon customers now in limited early access". You can join a waitlist. [S3]
- We found no price or plan for Kai. [S3]

**What happens to your data**

- Karbon says Kai works "within the security and permission settings your firm has established in Karbon". [S3]
- Karbon says "Every agent action goes through the AI Agent Management System, where you can approve, edit, or reject outputs" and "Nothing executes without your sign-off." [S3]
- Karbon says your client information, communications and work history "never leave". [S3]
- The Kai page doesn't name the AI model Kai uses, or say whether firm data trains it. [S3]

**In Australia**

- Karbon's pages don't say which countries early access covers. [S3] [S5]

### AI Agents and agentic workflows (early access)

**What it does**

- Karbon names five AI Agents: Bookkeeper, Practice Manager, Tax Preparer, Client Relationship Manager and Fractional CFO. [S4]
- Karbon says the agents can reconcile transactions, draft emails, send client reminders and prepare end-of-month workpapers, following your firm's playbook. [S4]
- They work inside your existing jobs, checklists and client timelines. [S4]

**Where to find it**

- Karbon's agents page offers a demo booking. It gives no product steps. [S4]

**Which plans have it**

- Karbon labels the agents and Agentic Workflows "Early Access". We found no plan or price. [S4] [S2]

**What happens to your data**

- Karbon says "You decide what AI Agents can do, when they need approval, and what requires a human touch." [S4]
- It also says you can "Review their work before it goes out or let them run automatically." [S4]
- Karbon says firms will later be able to configure each agent's capabilities. [S2]
- The agents page has no training or retention statement. [S4]

**In Australia**

- Karbon's pages don't say whether early access includes Australian firms. [S4]

### AI in period close (Aider)

**What it does**

- Karbon bought Aider, founded in New Zealand, in September 2025. Karbon now describes it as a period close automation platform. [S13] [S14]
- Aider runs close checks on Xero and QuickBooks Online books and syncs progress to Karbon work items. [S14]
- The AI Rule Builder turns a plain-English description of a check into a rule, which you review and adjust before saving. [S10]
- AI Document Validation checks each document a client uploads against what was requested, and asks the client if it doesn't match. [S11] [S14]

**Where to find it**

- In Aider's period close, connected to Karbon work items. Client questions go through the Karbon for Clients portal. [S14] [S11]

**Which plans have it**

- Not on the pricing page. Karbon's release notes point you to a demo or your Karbon representative. [S12] [S1]

**What happens to your data**

- The Aider pages and release notes we read have no AI data statement. [S14] [S11]

**In Australia**

- Karbon's release notes describe the rebuilt Aider and AI Document Validation as live "for all US customers". They don't mention Australia. [S12] [S11]
- When Karbon bought Aider, it said Aider had customers in Australia and New Zealand among other countries. [S13]

### Meeting Intelligence (coming soon)

- **What it does:** records, transcribes and summarises client meetings, with action items and follow-ups. [S2]
- Karbon's launch release describes an AI notetaker app that joins client meetings and puts structured notes into Karbon. [S5]
- **Where to find it:** not yet available. [S2]
- **Which plans have it:** not stated. [S2] [S5]
- **What happens to your data:** not stated. [S5]
- **In Australia:** not stated. [S5]

## Outside AI that connects

A quick word on the jargon. MCP (Model Context Protocol) is an open standard that lets an AI assistant use outside tools. An API is the door a product opens so other software can read or change its data. Karbon describes its planned MCP server as connecting Karbon "to external AI tools via an open standard". [S5]

### Claude and Karbon

**Official?**

- No official connection found. Karbon isn't in Anthropic's connectors directory as read on 17 October 2026. [S35]

**What Karbon has said**

- Karbon announced a public MCP server on 3 June 2026 that "Connects Karbon to external AI tools via an open standard". It didn't name Claude. [S5]
- Karbon's developer documentation lists an MCP server address, https://mcp.karbonhq.com, with no instructions. [S32]

**What that means for you**

- Anthropic says that if you have a connector's address, you can add it as a custom connector, whether or not it's in the directory. [S36]
- Karbon hasn't published what its server can read or change. It also hasn't said how you sign in or which plans can use it. So we can't tell you whether connecting it works, or what it would expose. [S32] [S5]
- Anthropic says custom connectors haven't been reviewed by Anthropic. [S36]

### ChatGPT and Karbon

**Official?**

- No official connection found. Searching ChatGPT's plugin directory for Karbon from Australia on 17 October 2026 returned "No plugins found". [S37]
- OpenAI's business plugins page doesn't mention Karbon. [S38]
- Karbon's MCP server announcement didn't name ChatGPT. [S5]

### Microsoft Copilot and Karbon

**Official?**

- No official connection found. Karbon isn't on Microsoft's list of federated Copilot connectors, updated 16 October 2026. [S39]
- Microsoft's galleries of partner-built and Microsoft-built Copilot connectors don't list Karbon either. [S40] [S41]

**What Karbon does connect to**

- Karbon integrates with Microsoft 365 email, calendars, OneDrive, SharePoint, Teams and Microsoft Entra ID. Karbon doesn't describe any of these as a Copilot connection. [S28]
- The Teams integration imports recorded and transcribed Teams meetings into the right client's timeline in Karbon. [S30]

### Google Gemini and Karbon

**Official?**

- No official connection found. Searching the Google Workspace Marketplace for Karbon on 17 October 2026 returned "No matching results". [S42]

**What Karbon does connect to**

- Karbon integrates with Gmail, Google Calendar and Google Drive. [S28]
- Karbon says it "does not use Google Workspace APIs to develop, improve, or train generalized AI and/or ML models". [S24]

### Karbon's MCP server and API (the developer route)

**Official?**

- Yes, for the API. Karbon publishes a REST API with a developer centre and guides. [S31] [S32]
- Karbon's developer documentation also lists an MCP server address, https://mcp.karbonhq.com. We found no page explaining it. [S32]
- In March 2026 Karbon published an early quick-reference guide, KARBON_API.md, for "developers and AI agents working with the Karbon API". [S33]

**What it can see and do**

- The API covers clients, work items, invoices and payments, custom fields, files, budgets and time, with webhooks for changes. [S31] [S32]
- We couldn't establish what the MCP server can read or change. [S32]

**What you need**

- A Business or Enterprise plan. Firms are limited to one API application per account. [S32] [S1]
- Access to Karbon's Settings, to switch on API access. The help article doesn't say which role that needs. [S20]
- Someone who can program. The API has a limit of 120 requests a minute. [S31]

**Steps to connect** (Karbon's help article, dated 28 April 2026)

1. In Karbon, go to Settings. Under Integrations and Tools, select API Applications. [S20]
2. Select the API Applications tab, then click Enable API Access. [S20]
3. The page refreshes and your API application appears, named after your practice. Click Manage next to it. [S20]
4. Copy the Application ID (your bearer token) and the Access Key. Karbon says to treat both "like passwords" and store them securely. Never paste them into a chat or a website. That last part is our advice. [S20]

**To disconnect**

- To cut off access, go to Settings > Integrations and Tools > API Applications, click Manage, then Rotate next to the Access Key. Karbon says the old key stops working immediately. [S20]
- We didn't find steps for switching API access off completely. [S20]

**Limits**

- One API application per account. [S32]
- Rotating the key breaks every integration still using the old key until you update it. [S20]

### Zapier and Karbon

- Karbon lists a Zapier integration that connects your Karbon contacts and organisations with other apps. [S29]
- New or updated contacts and organisations can trigger updates in other apps, and other apps can update them in Karbon. [S29]
- Karbon says you can reach "the full Karbon API through Zapier's Webhooks by Zapier feature". [S29]
- Karbon's Zapier page doesn't mention AI, plans or setup steps. [S29]

## Jobs it's good for

- **Catching up on a long thread.** Use Email Summary before you reply. [S2]
- **Before a client meeting.** Client Summary pulls emails, notes, work and billing into one brief. Check it against the timeline. [S2] [S8]
- **A client update from your task list.** Create Email from Tasks drafts it from your progress. You edit and send. [S2]
- **Sorting a busy inbox.** Set up AI labels for things like ATO notices or payroll changes. Start without actions until you trust the labels. That's our advice, based on how the actions work. [S19]
- **Missed time.** Let Karbon AI flag time entries you forgot, then fix them. [S2]
- **Month-end close for Xero or QuickBooks Online clients.** Aider runs close checks and flags exceptions. Karbon describes the newest version as live for US customers. [S14] [S12]
- **A custom tool, for someone who can code.** On Business or Enterprise, use the Karbon API and KARBON_API.md. [S20] [S33]

## What to watch for

**On for everyone by default**

- Karbon AI is enabled for all users by default. Only an account admin can turn it off, and only for the whole firm. [S2] [S15]

**Email actions can run without you**

- A label action fires automatically whenever the AI is at least 80% sure. Clear removes the email from Triage, and Assign routes it to a colleague. [S19]
- Draft Reply to All includes everyone on the original thread. It creates a draft, and the article doesn't describe it sending anything. [S19]
- Check the email timeline to see what the AI did. [S19]

**Terms older than the features**

- Karbon's AI terms were last updated on 27 September 2023. They don't mention Kai or AI Agents. [S7]
- Those terms list prohibited uses that include "Provide legal or financial advice" and "Implement fully-automated decision making." [S7]
- The terms provide Karbon AI "AS-IS" and say production use is "AT YOUR SOLE RISK". [S7]

**Microsoft can see some prompts**

- Under Karbon's terms, Microsoft stores what you send to Karbon AI to watch for abuse, and authorised Microsoft staff may review flagged data. [S7]

**Where Australian data sits**

- Karbon says its AI keeps processing in the region where your Karbon data is stored, but the pages we read don't say where Australian firms' data is stored. [S8] [S2]
- Karbon's privacy policy, last updated February 2025, doesn't mention AI and doesn't name hosting countries. [S23]
- Karbon's trust centre asks for a work email before it shows anything, so we couldn't read it. [S34]

**Early access means change**

- Kai and AI Agents are early access. Karbon says Kai's actions need your sign-off, but its agents page also says you can let agents "run automatically". [S3] [S4]
- Karbon said in June 2026 that agentic workflows will let AI "take autonomous action" inside firm workflows. [S5]

**No official AI connections yet**

- None of Claude, ChatGPT, Copilot or Gemini has an official Karbon connection we could find. [S35] [S37] [S39] [S42]
- Karbon's MCP server is announced but undocumented. Wait for Karbon's own instructions before connecting client data to an outside AI. That's our advice. [S5] [S32]

**API keys are passwords**

- Karbon says to treat the Application ID and Access Key like passwords. [S20]
- One person with those keys can reach whatever the API can reach. That's our inference from how the keys work. [S20]

**Security basics**

- Karbon's web application is SOC 2 Type 2 certified. Karbon says it hasn't yet been certified to ISO 27001. [S22]
- Data and backups are encrypted at rest with AES-256. [S22]

## Announced changes

Karbon's Kai release says "Many of the features announced are available immediately, while others will roll out over the coming months." It doesn't say which. [S5]

- **27 September 2023:** Karbon's AI terms were last updated. [S7]
- **30 September 2025:** Karbon announced it had bought Aider. It listed "AI agents that execute tasks and streamline workflows" as coming soon. [S13]
- **January 2026:** Karbon Practice Intelligence was renamed Karbon Analytics. [S21]
- **11 March 2026:** Karbon published KARBON_API.md in early access. [S33]
- **31 March 2026:** Karbon AI became available to all customers, with in-region processing. [S8]
- **27 April 2026:** Karbon's rebuilt Aider period close went live for US customers. [S12]
- **3 June 2026:** At Karbon Next 2026, Karbon launched Kai in early access and announced an AI notetaker, a public MCP server, embedded AI in Karbon Analytics and agentic period close checks. [S5] [S6]
- **29 June 2026:** The AI Rule Builder for period close checks was released. [S10]
- **5 August 2026:** AI Document Validation went live for US customers. [S11]
- **Coming soon:** Meeting Intelligence, which records, transcribes and summarises client meetings. [S2]
- **Later:** settings for each agent's capabilities. [S2]

## What we couldn't establish

- **Karbon's MCP server.** We couldn't find what it can read or change, how you sign in, which plans can use it, which AI apps it supports, or whether it's live. Its address gave us a "not found" page. [S32] [S5]
- **Where Australian firms' data is stored and processed.** Karbon says AI stays in-region but doesn't name Australia's region. [S8] [S2]
- **Karbon's trust centre.** It asks for a work email before showing content. [S34]
- **Which AI model Kai, AI Agents and AI labels use**, and whether the 2023 AI terms cover them. [S3] [S4] [S7] [S19]
- **Whether the firm-wide switch turns off AI labels and Kai.** The help article only names Karbon AI. [S15] [S19]
- **Prices and plans for Kai, AI Agents and Aider.** [S3] [S4] [S12]
- **Whether Kai and AI Agents early access is open to Australian firms.** [S3] [S4]
- **Whether Aider's AI features are offered in Australia.** The release notes say US customers. [S11] [S12]
- **AI in Karbon Analytics.** It was announced in June 2026, but the Analytics help topic has no article about it. [S5] [S21]
- **Karbon's help centre search** returned no results to us, so we may have missed help articles on Kai, agents or the MCP server. [S17]
- **The Karbon AI overview article.** The help topic lists it, but we couldn't open it. [S17]
- **Customer numbers.** Karbon's about page says customers in 34 countries. Its June 2026 release says 40. [S27] [S5]
- We didn't rely on third-party claims. Other companies advertise their own Karbon MCP servers and connectors. They aren't Karbon's, and we didn't review them.

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Practice Management Plans to Suit Every Accounting Firm (pricing, viewed with AUD selected) | Karbon | https://karbonhq.com/pricing/ | No date shown (© 2026) | 17 Oct 2026 |
| S2 | AI-Powered Practice Management for Accounting Firms (Karbon AI) | Karbon | https://karbonhq.com/feature/ai/ | No date shown (© 2026) | 17 Oct 2026 |
| S3 | Kai by Karbon: the AI coworker for your firm | Karbon | https://karbonhq.com/feature/kai/ | No date shown (© 2026) | 17 Oct 2026 |
| S4 | AI Agents (Early Access) | Karbon | https://karbonhq.com/feature/agents/ | No date shown (© 2026) | 17 Oct 2026 |
| S5 | Karbon launches Kai, the AI coworker that knows your firm | Karbon Magazine (media release) | https://karbonhq.com/resources/karbon-launches-kai/ | 3 Jun 2026 | 17 Oct 2026 |
| S6 | Special Event: Kai and Practice Management's AI Evolution | Karbon | https://karbonhq.com/resources/webinars/karbon-product-roadmap-reveal-june-2026/ | No date shown (keynote at Karbon Next 2026) | 17 Oct 2026 |
| S7 | Karbon AI Supplemental Terms | Karbon | https://karbonhq.com/karbon-ai-beta-terms-of-use/ | Last updated 27 Sep 2023 | 17 Oct 2026 |
| S8 | Karbon AI is now available to all customers, plus clearer document visibility and greater control | Karbon release notes | https://karbonhq.com/release-notes/mar-31-2026/ | 31 Mar 2026 (date from Karbon's release notes list) | 17 Oct 2026 |
| S9 | Karbon release notes (list) | Karbon | https://karbonhq.com/release-notes/ | Latest entry 6 Oct 2026 | 17 Oct 2026 |
| S10 | Automated engagement renewals, AI-assisted period close, and Gusto integration | Karbon release notes | https://karbonhq.com/release-notes/june-29-2026/ | 29 Jun 2026 | 17 Oct 2026 |
| S11 | End client back-and-forth with Client Questions and AI Document Validation in Aider's Period Close Automation | Karbon release notes | https://karbonhq.com/release-notes/aug-5-2026/ | 5 Aug 2026 | 17 Oct 2026 |
| S12 | Period close automation powered by Aider, create work from engagements, Gusto integration, and more | Karbon release notes | https://karbonhq.com/release-notes/apr-27-2026/ | 27 Apr 2026 | 17 Oct 2026 |
| S13 | Karbon acquires Aider to deliver the future of AI-powered accounting and bookkeeping | Karbon Magazine (media release) | https://karbonhq.com/resources/karbon-acquires-aider/ | 30 Sep 2025 | 17 Oct 2026 |
| S14 | Aider + Karbon | Karbon | https://karbonhq.com/integrations/aider/ | No date shown (© 2026) | 17 Oct 2026 |
| S15 | How can I get access to Karbon AI? | Karbon Help | https://help.karbonhq.com/en/s/articles/7853999-how-can-i-get-access-to-karbon-ai | 28 Sep 2026 | 17 Oct 2026 |
| S16 | How secure is Karbon AI? | Karbon Help | https://help.karbonhq.com/en/s/articles/7854015-how-secure-is-karbon-ai | 14 Oct 2025 | 17 Oct 2026 |
| S17 | Karbon AI (help topic) | Karbon Help | https://help.karbonhq.com/en/s/topic/0TORh0000003svTOAQ/karbon-ai | No date shown | 17 Oct 2026 |
| S18 | Anatomy of Triage | Karbon Help | https://help.karbonhq.com/en/s/articles/63015897-anatomy-of-triage | 27 Jul 2026 | 17 Oct 2026 |
| S19 | How AI Label Actions Work in Karbon Triage | Karbon Help | https://help.karbonhq.com/s/articles/2000273-ai-label-actions-triage | 10 Aug 2026 | 17 Oct 2026 |
| S20 | Setting Up API Access in Karbon | Karbon Help | https://help.karbonhq.com/s/articles/000017541-setting-up-api-access-karbon | 28 Apr 2026 | 17 Oct 2026 |
| S21 | Karbon Analytics (help topic) | Karbon Help | https://help.karbonhq.com/en/s/topic/0TORh0000003svWOAQ/karbon-analytics | No date shown; notes the January 2026 rename | 17 Oct 2026 |
| S22 | Security | Karbon | https://karbonhq.com/security/ | No date shown (© 2026) | 17 Oct 2026 |
| S23 | Privacy Policy | Karbon | https://karbonhq.com/privacy-policy/ | Last updated 3 Feb 2025 | 17 Oct 2026 |
| S24 | Use of Google API Services | Karbon | https://karbonhq.com/use-of-google-api-services/ | No date shown (© 2026) | 17 Oct 2026 |
| S25 | Karbon for Enterprise | Karbon | https://karbonhq.com/enterprise/ | No date shown | 17 Oct 2026 |
| S26 | Some users are experiencing access issues in the Australian domain | Karbon Status | https://status.karbonhq.com/cmqhqe1v707xs2jlms6nue7fx | 17 Jun 2026 | 17 Oct 2026 |
| S27 | About Karbon | Karbon | https://karbonhq.com/about/ | No date shown | 17 Oct 2026 |
| S28 | With Karbon, your firm's apps connect better (integrations) | Karbon | https://karbonhq.com/integrations/ | No date shown | 17 Oct 2026 |
| S29 | Zapier + Karbon | Karbon | https://karbonhq.com/integrations/zapier/ | No date shown (© 2026) | 17 Oct 2026 |
| S30 | Microsoft Teams + Karbon | Karbon | https://karbonhq.com/integrations/teams/ | No date shown (© 2026) | 17 Oct 2026 |
| S31 | Karbon Developer Center | Karbon | https://developers.karbonhq.com/ | No date shown; release notes run to 23 Sep 2026 | 17 Oct 2026 |
| S32 | Karbon API documentation (llms.txt) | Karbon | https://developers.karbonhq.com/llms.txt | No date shown; release notes listed to 23 Sep 2026 | 17 Oct 2026 |
| S33 | New Developer Quick-Reference Guide (Early Access) | Karbon Developer Center | https://developers.karbonhq.com/release-notes/2026-03-11/ | 11 Mar 2026 | 17 Oct 2026 |
| S34 | Karbon Trust Center | Karbon (hosted by Conveyor) | https://app.conveyor.com/profile/karbonhq | No date shown. Asks for a work email before showing content | 17 Oct 2026 |
| S35 | Connectors and plugins (Claude Marketplace) | Anthropic | https://claude.com/connectors | No date shown. Karbon not listed | 17 Oct 2026 |
| S36 | Connector verification | Anthropic | https://claude.com/docs/connectors/verification | No date shown | 17 Oct 2026 |
| S37 | ChatGPT plugin directory: search for "Karbon" | OpenAI | https://chatgpt.com/plugins?q=Karbon | No date shown. "No plugins found" (searched from Australia, signed out) | 17 Oct 2026 |
| S38 | Plugins: Connect tools and apps to ChatGPT and Codex | OpenAI | https://openai.com/business/plugins/ | No date shown | 17 Oct 2026 |
| S39 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | ms.date 30 Sep 2026; updated 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S40 | Partner-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-partners | ms.date 27 Apr 2026; updated 25 Sep 2026 (page metadata) | 17 Oct 2026 |
| S41 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | ms.date 30 Sep 2026 (page metadata) | 17 Oct 2026 |
| S42 | Google Workspace Marketplace: search for "karbon" | Google | https://workspace.google.com/marketplace/search/karbon | No date shown. "No matching results" | 17 Oct 2026 |
| S43 | Karbon site summary for AI tools (llms-full.txt), pricing section | Karbon | https://karbonhq.com/llms-full.txt | Pricing section "Last updated: 2026-06-30" | 17 Oct 2026 |
