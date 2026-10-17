# Actionstep: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Actionstep's AI is called Actionstep Intelligence, an AI layer built into its practice management platform and released on 11 August 2026. Its first parts are Trace, for AI time capture, and Acumen, for business reporting with an AI assistant. [S3]
- Both are add-on modules. Actionstep doesn't publish prices. It quotes per user, plus implementation fees. [S2]
- Trace is a Windows app that watches the active window in Office apps and PDF readers. It drafts time entries with AI-written narratives for you to review, and nothing posts automatically. [S15] [S3]
- Ask Acumen, in early access, answers plain-English questions about your firm's dashboard figures. Actionstep says Australian firms' data for it is hosted and processed in Australian AWS regions. [S19]
- Actionstep says it doesn't use your data to train AI models. Its Trust Center says AI runs inside Actionstep's AWS environment and your data doesn't leave AWS to reach a third-party AI provider. [S1] [S11]
- Actionstep may keep what you type into its AI features and what they produce, for audit trails and quality checks. [S11]
- Actionstep says "Every AI feature is opt-in." [S1]
- We found no official connection between Actionstep and ChatGPT, Claude, Microsoft Copilot or Google Gemini. Actionstep says an MCP server is coming "later this year". [S35] [S37] [S38] [S40] [S3]
- Actionstep documents a Zapier integration and an API with a $500 setup charge. Third-party AI tools such as AI Legal Assistant also connect. [S23] [S22] [S9]

## The tool, and the plans that matter

Actionstep is cloud practice management software for midsize law firms. In August 2026 it said it supports more than 5,000 firms globally. [S3]

For users in Australia, Actionstep's terms say Actionstep Operations Australia Pty Ltd is responsible for personal information. [S14] Its Australian and New Zealand privacy policy says, "We host customer data in Australia and New Zealand". [S13]

Actionstep doesn't publish prices. Each module is "Priced per user plus implementation fees", with a **Request Pricing** button. Certified implementation partners set firms up, and finance options are offered for implementation. [S2]

| Module | What it is | AI in it | Price |
|---|---|---|---|
| Practice Management | The core platform: matters, documents, email, time and billing | Matter suggestions in the Outlook add-in, and Scout for support questions | Per user plus implementation fees |
| Trace – AI Time Capture | A premium add-on for passive time capture | AI matter mapping, billing codes and narratives | Per user plus implementation fees |
| Acumen – Embedded Analytics | An add-on of dashboards, in early access | "AI-powered Q&A and 'Explain This Number' insights" | Per user plus implementation fees |
| Builder | Document automation | None described | Per user plus implementation fees |
| Capture | Client intake forms | None described | Per user plus implementation fees |
| Legal Accounting | Separate accounting suite | None described | "Only available in North America" |

Sources for the table: [S2] [S5] [S19] [S26] [S21]

- The pricing page shows the add-on modules, including Trace and Acumen, when you select the AU region. [S2]

## AI built in

### Actionstep Intelligence (the AI layer)

**What it does**

- Actionstep describes four capabilities: Context, Observe, Recommend and Execute. Execute "Proposes and carries out approved operational and financial work with human oversight and full audit trails." [S3]
- The first capabilities released are Trace and Acumen. [S3]
- "AI-orchestrated workflow automation" is labelled "Coming soon" on Actionstep's AI page. [S1]
- Actionstep says its AI is "model-agnostic", so it can switch to better models as they emerge. [S1]

**Where to find it**

- Inside Actionstep's own screens, "with no separate system or login". [S4]

**Which plans have it**

- Trace and Acumen are sold as add-on modules. [S2]

**What happens to your data**

- "Actionstep does not use your firm's data to train AI models." [S1]
- The Trust Center says Actionstep doesn't share your data with model providers, and your data isn't used to train or improve the underlying foundation models. [S11]
- It says AI processing happens inside AWS: "Asia Pacific for Australian and New Zealand firms". [S11]
- Actionstep may keep AI inputs and outputs to maintain an audit trail and improve quality. It says AWS doesn't keep them after processing. [S11]
- Access to AI-generated content generally follows each user's permissions. Beta features may instead be limited to a nominated group of users. [S11]
- Actionstep says AI features are covered by your existing agreement. [S11]

**In Australia**

- The Trust Center names Asia Pacific as the processing region for Australian firms. [S11]

### Trace (AI time capture)

**What it does**

- Runs in the background on your computer and tracks the active window outside Actionstep, such as Word, Outlook and PDF readers. [S15]
- Captures the app name, file name, subject line and "relevant content", then drafts a time entry with an AI-written narrative. [S15]
- Maps work to matters and billing codes with AI. Suggested matters in blue are "nearly certain"; purple ones are "mostly matches". [S15] [S17]
- Actionstep says entries "are not posted automatically, and the fee earner retains control over what reaches the bill". [S3]
- It doesn't track phone, Teams or Zoom calls. It captures desktop Microsoft Office apps only, and the web versions aren't supported yet. [S15]

**Where to find it**

- An admin turns on the **Trace**, **Trace Timesheet** and **Trace Suggestion** feature flags under **Admin > General**. [S15]
- The installer comes from **Admin > Trace > Installation Information**. IT can deploy it to everyone, or each fee earner can install Trace.msi. [S16]
- Review captured work in **Time > Timesheet**. [S17]
- Set minimum activity times in **My Profile**, under **Trace**, then **Configure**. [S18]

**Which plans have it**

- A premium add-on module. Actionstep planned it for select customers from July 2026 and a full release in August 2026. [S5]
- Early access customers get the installer from an Actionstep representative. [S16]

**What happens to your data**

- Trace "monitors activity in your active window and captures details such as application names, file names, and content". [S16]
- Windows may show a Microsoft Defender SmartScreen warning when you install it. Actionstep says this is normal for new software if the file came from the **Admin > Trace** page. [S16]
- Trace's articles don't say where its AI processing happens. The Trust Center's general answer is AWS in Asia Pacific for Australian firms. [S15] [S11]

**In Australia**

- Trace is listed among the add-ons shown for the AU region on the pricing page. [S2]
- It's supported only on Windows. [S15]

### Acumen and Ask Acumen (business intelligence)

**What it does**

- Pre-built dashboards for firm leaders and fee earners, covering work in progress, billing, collections and utilisation. [S20] [S2]
- **Ask Acumen** answers natural-language questions about the Firm Management dashboard, "grounded in your Actionstep data". [S19]
- Actionstep says answers respect each user's permissions. [S4]

**Where to find it**

- In Practice Management, go to **Insights > Business Intelligence**, click **Firm Management**, then click **Ask Acumen** in the top-right corner. [S19]

**Which plans have it**

- An add-on module, "currently in early access". [S20] [S2]

**What happens to your data**

- Ask Acumen "is powered by Amazon Quick AI Assistant", using models AWS hosts through Amazon Bedrock. Actionstep says "no third-party AI vendor receives or processes your data". [S19]
- "Australian firms are hosted in the AWS Asia Pacific (Sydney) region". AI processing stays within the Australian AWS regions of Sydney and Melbourne. [S19]
- During the beta, Actionstep keeps your questions and the answers to evaluate quality. It says these aren't used to train AI models. [S19]
- You can delete saved chat sessions from **History**. [S19]

**In Australia**

- Actionstep names Sydney for hosting and Australia for processing. New Zealand firms are also served from Sydney. [S19]

### Matter suggestions in the Outlook add-in

**What it does**

- Actionstep says "Our AI intuitively suggests the right matters to file emails and documents". [S26]

**Where to find it**

- The Actionstep add-in for Outlook 365. An admin can approve it for the whole tenant, or deploy it from **Services & add-ins** in the Office 365 admin centre. [S25]

**Which plans have it**

- Listed as "Free + O365 Subscription". It needs an Office 365 Business account using Exchange Online. [S26] [S25]

**What happens to your data**

- Admins can switch between the older add-in and the December 2024 version in **Admin > General Settings > Outlook Add-In (Beta)**. [S25]
- The pages we read don't say how the matter suggestions are made or whether they can be turned off. [S26] [S25]

**In Australia**

- Not stated separately. [S26]

### Scout (AI support assistant)

**What it does**

- Answers questions about using Actionstep from its help articles, with step-by-step guidance. [S21]
- It won't give definitive answers on trust accounting or financial audits, but it can point you to articles. [S21]

**Where to find it**

- Practice Management users launch it from the Knowledge Hub, under **Help** in the main menu, or from the chat bubble in the Help Center. [S21]

**Which plans have it**

- Available to Practice Management and Legal Accounting customers. [S21] [S6]

**What happens to your data**

- "Scout does not access your firm's data." [S21]
- Its April 2026 FAQ says Scout runs on Zendesk's generative AI, with no training on your questions and zero data retention by third-party models. [S21]
- Actionstep's 2025 announcements said Scout was "Powered by the same OpenAI technology behind ChatGPT". [S6] [S7]

**In Australia**

- Actionstep launched Scout for firms globally. [S6]

## Outside AI that connects

In plain words, a connector lets a chat assistant such as Claude or ChatGPT look things up in another app, and sometimes make changes there. Anthropic lists each one in its Connectors directory with a Verified or Community label. [S36]

### Claude and Actionstep

**Official?**

- No official connection found. Actionstep isn't among the connectors on Anthropic's public directory page. [S35]
- Actionstep's August 2026 release says an MCP server is coming "later this year". Anthropic's page says Claude can connect to any remote MCP server by its URL. [S3] [S36]

**What it can see and do**

- Nothing official yet. [S35]

**What you need, steps, disconnecting**

- Not applicable. [S35]

**Limits**

- Actionstep's terms make you responsible for keeping usernames and passwords secure and confidential. [S14]
- Our reading: giving an AI tool your Actionstep login to work in the app sits awkwardly with that. This isn't legal advice.

### ChatGPT and Actionstep

**Official?**

- No official connection found. Actionstep isn't on OpenAI's public plugin page, including its Legal category. [S37]

**What it can see and do**

- Nothing official. [S37]

**Limits**

- When Scout used OpenAI technology, Actionstep said it was "fully separate from ChatGPT" and used only Actionstep's help content. [S7]
- Actionstep's CEO wrote in August 2026 that someone using "a tool like ChatGPT" through an AI-native layer would inherit the same guardrails. That reads as a direction, and we found no released feature behind it. [S10]

### Microsoft Copilot and Actionstep

**Official?**

- No official connection found. Actionstep isn't among Microsoft's federated Copilot connectors or its Power Platform connectors. [S38] [S39]

**What Actionstep does offer in Microsoft 365**

- Actionstep for Outlook, Actionstep for Word and Actionstep Builder for Word are listed on Microsoft's Marketplace. None is a Copilot agent. [S34]
- **Qanooni**, a separate legal AI that works in Word and Outlook, has an integration with Actionstep. Actionstep's page lists it as available globally at £100 to £150 per user per month. [S28]

**Limits**

- Qanooni is a third-party product with its own subscription. Actionstep's page says it's hosted on Microsoft Azure. [S28]

### Google Gemini and Actionstep

**Official?**

- No official connection found. Actionstep isn't on Google's list of Connected Apps for Gemini. [S40]

**What Actionstep does offer with Google**

- A Gmail add-on that files emails to matters, and a Google Drive integration for viewing files in matters. Neither involves Gemini. [S42] [S43]

### Actionstep's MCP server (announced)

- On 11 August 2026 Actionstep said it is "expanding Actionstep Intelligence later this year with additional capabilities across search, workflow execution, and an MCP server". [S3]
- Actionstep's API and Zapier help articles don't mention it. [S22] [S23]

### Zapier and Actionstep

**Official?**

- Yes. Actionstep's help centre and integrations directory describe the Zapier integration. [S23] [S27]

**What it can see and do**

- Triggers include a new matter, contact, task or file note, a contact added to a matter, a step change, and a matter update. [S23]
- Actions include creating file notes, tasks, contacts, matters and disbursements, and finding a contact or matter. [S23]
- Zapier's own page offers Actionstep through Zapier MCP, which lets AI tools that support MCP run those actions. [S41]

**What you need**

- A Zapier account and your Actionstep login. The integration is listed as "Free + Zapier Subscription". [S23] [S27]
- Actionstep Support can't directly support Zaps your team builds. [S23]

**Steps to connect** (Actionstep help centre, edited 14 April 2026)

1. Sign up for a Zapier account. [S23]
2. Install the Zapier integration from the link in Actionstep's article, and choose the apps you want to connect. [S23]
3. Authenticate each app with its sign-in. [S23]
4. Build a Zap linking a trigger in one app to an action in the other. Zapier's help has the full instructions. [S23]

**To disconnect**

- Not described in Actionstep's article. [S23]

**Limits**

- Actionstep suggests a custom API integration may suit firms that send a very high number of Zaps in short timeframes. [S23]
- Running Actionstep actions from an AI tool through Zapier MCP is Zapier's route. Actionstep's article doesn't mention it. [S23] [S41]

### Actionstep's API

- The API lets developers build apps that use Actionstep as the back end. [S22]
- There's "a $500 initial setup charge for access to the API", which includes a sandbox. The article doesn't name the currency. [S22]
- Actionstep reviews requests, usually within 7 to 14 business days, and reviews your integration before issuing production credentials. [S22]
- The Trust Center says APIs use token-based authentication and limited-scope access. [S11]

### Other AI apps that connect to Actionstep

- **AI Legal Assistant**, from Sydney, has a two-way integration for document drafting. It was "available immediately to new and existing Actionstep customers across Australia and New Zealand" from November 2025. [S9]
- **Lexidesk** answers calls and web enquiries with AI and syncs client details and summaries to Actionstep. It's listed as available globally. [S29] [S1]
- **Rising Tide AI** offers AI process automation, listed for the UK only. [S30]
- Actionstep's integrations directory has an "AI Integrations" section, which featured Lexidesk when we read it. The directory can be filtered by location, including AU. [S31]
- Actionstep's terms say third-party apps you enable may access your data, and Actionstep isn't responsible for what they do with it. [S14]

## Jobs it's good for

- **Capturing time from email and documents.** Let Trace draft entries from your Outlook and Word work, then review them on the Timesheet. [S15] [S17]
- **Asking about firm performance.** Ask Acumen a question such as revenue this quarter or outstanding fees. [S4] [S19]
- **Filing email.** Use the Outlook add-in's matter suggestions to file emails and attachments. [S26]
- **"How do I" questions.** Ask Scout for steps from Actionstep's help articles. [S21]
- **Drafting with an Australian AI tool.** Connect AI Legal Assistant to work on documents linked to Actionstep matters. [S9]
- **Routine record creation.** Use Zapier to create matters, contacts or file notes from other apps. [S23]

## What to watch for

**Trace reads your screen**

- Trace records application names, file names, email subject lines and content from whatever window is active. [S16] [S17]
- It errs "on the side of capturing more time rather than less", so expect to clean up entries. [S15]

**What Actionstep keeps**

- Actionstep may retain AI inputs and outputs for audit trails and quality assurance. [S11]
- During the Ask Acumen beta, chats are kept for evaluation. [S19]

**Who gets beta features**

- Actionstep says once a beta feature is enabled, it "may be available to all your Actionstep users". [S24]
- Some AI features in beta may be limited to a nominated group rather than following individual permissions. [S11]

**Where data is hosted**

- Actionstep's pages describe hosting regions differently. One lists Australia, Europe, Singapore and the United States, another adds New Zealand, and the Trust Center lists the USA, Canada, Ireland and Australia. [S32] [S33] [S11]
- Actionstep's public sub-processor list includes AWS and Microsoft Azure, and no separate AI model company. [S12]

**Check the work**

- The Trust Center says "Outputs are an aid, not advice" and should be reviewed by a qualified person before being relied on. [S11]

**Outside apps**

- Third-party apps you enable can access your data, and Actionstep isn't responsible for their use of it. [S14]

## Announced changes

- **10 August 2025:** Actionstep set up an AI Center of Excellence and listed roadmap items including document intelligence, contextual AI search and AI-enhanced workflows. [S8]
- **28 January 2026:** Trace was announced as a premium add-on, for select customers from July 2026 and a full release planned for August 2026. [S5]
- **11 August 2026:** Actionstep Intelligence was released. Search, workflow execution and an MCP server are promised "later this year". [S3]
- **Coming soon:** AI-orchestrated workflow automation, where agents carry out tasks within limits administrators set. [S1]
- **Previewed:** Workflow 2.0, which moves matters between phases automatically. [S4]
- **Trace:** Support for web-based Microsoft apps "will be coming in later releases". [S15]
- **Acumen:** Still in early access, with chat retention described as part of the beta. [S19] [S20]

## What we couldn't establish

- **Prices.** Actionstep doesn't publish them for any module. [S2]
- **Where Trace's AI runs, and on which model.** Trace's articles don't say. [S15] [S16]
- **What powers Scout.** The April 2026 FAQ says Zendesk's generative AI; the 2025 announcements said OpenAI technology. [S21] [S6]
- **Trace and websites.** The same article says website tracking "will be in a future release" and that Trace "also captures activity you perform on web sites". [S15]
- **Trace's minimum time.** One article says a 15-second threshold for emails and documents; the newer settings article says the default minimum is 5 seconds. [S15] [S18]
- **Hosting regions.** Actionstep's pages list different regions. [S11] [S32] [S33]
- **Whether Trace and Acumen are generally available in Australia.** The pricing page lists them for AU, but the help centre still calls Acumen early access and mentions an early access programme for Trace. [S2] [S20] [S16]
- **The MCP server.** No details, dates or documentation yet. [S3]
- **The API setup fee's currency.** The article says "$500" only. [S22]
- **The Outlook add-in's matter suggestions.** We couldn't find how they work or whether they can be switched off. [S26] [S25]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Law Firm Artificial Intelligence (AI for Law firms) | Actionstep | https://www.actionstep.com/artificial-intelligence/ | No date shown (page metadata 12 Aug 2026) | 17 Oct 2026 |
| S2 | Pricing | Actionstep | https://www.actionstep.com/pricing/ | No date shown (page metadata 20 Aug 2026) | 17 Oct 2026 |
| S3 | Actionstep Releases Actionstep Intelligence: AI Built for the Business of Midsize Law Firms | Actionstep (news) | https://www.actionstep.com/blog/actionstep-releases-actionstep-intelligence-ai-built-for-the-business-of-midsize-law-firms/ | Posted 11 Aug 2026 | 17 Oct 2026 |
| S4 | AI for Law Firms: Actionstep Intelligence Webinar Recap | Actionstep Blog | https://www.actionstep.com/blog/ai-for-law-firms-actionstep-intelligence-webinar-recap/ | Posted 28 Sep 2026 | 17 Oct 2026 |
| S5 | Actionstep Accelerates AI Innovation With Trace, a Next-Gen Time Capture Module for Modern Law Firms | Actionstep (news) | https://www.actionstep.com/blog/actionstep-accelerates-ai-innovation-with-trace-a-next-gen-time-capture-module-for-modern-law-firms/ | Posted 29 Jan 2026 (release dated 28 Jan 2026; page metadata 15 Jul 2026) | 17 Oct 2026 |
| S6 | Actionstep Introduces Scout AI Support Assistant | Actionstep (news) | https://www.actionstep.com/blog/actionstep-introduces-scout-ai-support-assistant/ | Posted 1 Jul 2025 | 17 Oct 2026 |
| S7 | Meet Scout: Your New AI Support Assistant for Actionstep | Actionstep Blog | https://www.actionstep.com/meet-scout-your-new-ai-support-assistant-for-actionstep-practice-management/ | Posted 18 Jun 2025 | 17 Oct 2026 |
| S8 | Actionstep Establishes AI Center of Excellence | Actionstep (news) | https://www.actionstep.com/actionstep-establishes-ai-center-of-excellence-helping-midsize-law-firms-leverage-ai-for-the-management-of-law/ | Posted 10 Aug 2025 | 17 Oct 2026 |
| S9 | AI Legal Assistant Announces Integration with Actionstep | Actionstep (news) | https://www.actionstep.com/blog/ai-legal-assistant-announces-integration-with-actionstep/ | Posted 26 Nov 2025 (release dated 12 Nov 2025) | 17 Oct 2026 |
| S10 | The Difference Between Using AI and Becoming an AI-Native Law Firm | Actionstep Blog | https://www.actionstep.com/blog/the-difference-between-using-ai-and-becoming-an-ai-native-law-firm/ | Posted 3 Aug 2026 | 17 Oct 2026 |
| S11 | Trust Center: FAQ (including "AI in Actionstep" and "Data Sovereignty") | Actionstep | https://www.actionstep-trust.com/faq | No date shown | 17 Oct 2026 |
| S12 | Trust Center: Subprocessors | Actionstep | https://www.actionstep-trust.com/subprocessors | No date shown | 17 Oct 2026 |
| S13 | Privacy Policy (Australia and New Zealand) | Actionstep | https://www.actionstep.com/privacy-policy-australia-and-new-zealand/ | "Last Updated: 3 March, 2026" | 17 Oct 2026 |
| S14 | Terms of Use | Actionstep | https://www.actionstep.com/terms/ | "Last updated: 14-April-2026" | 17 Oct 2026 |
| S15 | About Trace | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/52520331660307-About-Trace | Edited 6 Aug 2026 (help centre data) | 17 Oct 2026 |
| S16 | Installing Trace | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/52922246806931-Installing-Trace | Edited 6 Aug 2026 (help centre data) | 17 Oct 2026 |
| S17 | Reviewing and Recording Time Entries Using Trace | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/52524297058963-Reviewing-and-Recording-Time-Entries-Using-Trace | Edited 12 Oct 2026 (help centre data) | 17 Oct 2026 |
| S18 | Setting Minimum Activity Times for Trace Suggestions | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/56260144759699-Setting-Minimum-Activity-Times-for-Trace-Suggestions | Edited 9 Oct 2026 (help centre data) | 17 Oct 2026 |
| S19 | Reviewing AI-Generated Insights About Your Business Intelligence Dashboards | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/54160035903379-Reviewing-AI-Generated-Insights-About-Your-Business-Intelligence-Dashboards | Edited 10 Aug 2026 (help centre data) | 17 Oct 2026 |
| S20 | About the Firm Management Dashboard | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/51073934778899-About-the-Firm-Management-Dashboard | Edited 13 Oct 2026 (help centre data) | 17 Oct 2026 |
| S21 | Using Scout (AI Support Assistant) FAQ | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/50482508470803-Using-Scout-AI-Support-Assistant-FAQ | Edited 20 Apr 2026 (help centre data) | 17 Oct 2026 |
| S22 | Actionstep API | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/50482549518355-Actionstep-API | Edited 24 Apr 2026 (help centre data) | 17 Oct 2026 |
| S23 | About Using Actionstep with Zapier | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/50482542026003-About-Using-Actionstep-with-Zapier | Edited 14 Apr 2026 (help centre data) | 17 Oct 2026 |
| S24 | About Actionstep's Beta Testing Program | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/50482538737043-About-Actionstep-s-Beta-Testing-Program | Edited 14 Apr 2026 (help centre data) | 17 Oct 2026 |
| S25 | Setting Up the Outlook Add-in | Actionstep Help Center | https://support.actionstep.com/hc/en-us/articles/50717863869459-Setting-Up-the-Outlook-Add-in | Edited 15 Sep 2026 (help centre data) | 17 Oct 2026 |
| S26 | Outlook add-in for Office 365 (integration page) | Actionstep | https://www.actionstep.com/integrations/outlook-add-in-for-office-365/ | No date shown (page metadata 17 Jun 2025) | 17 Oct 2026 |
| S27 | Zapier (integration page) | Actionstep | https://www.actionstep.com/integrations/zapier/ | No date shown (page metadata 29 Sep 2024) | 17 Oct 2026 |
| S28 | Qanooni AI (integration page) | Actionstep | https://www.actionstep.com/integrations/qanooni/ | No date shown (page metadata 16 Oct 2026) | 17 Oct 2026 |
| S29 | Lexidesk (integration page) | Actionstep | https://www.actionstep.com/integrations/lexidesk/ | No date shown (page metadata 2 Sep 2025) | 17 Oct 2026 |
| S30 | Rising Tide AI (integration page) | Actionstep | https://www.actionstep.com/integrations/rising-tide-ai/ | No date shown (page metadata 14 Jul 2026) | 17 Oct 2026 |
| S31 | Integrations | Actionstep | https://www.actionstep.com/integrations/ | No date shown (page metadata 2 Oct 2026) | 17 Oct 2026 |
| S32 | Cybersecurity | Actionstep | https://www.actionstep.com/cybersecurity/ | No date shown (page metadata 29 Sep 2024) | 17 Oct 2026 |
| S33 | FAQs | Actionstep | https://www.actionstep.com/faqs/ | No date shown (page metadata 19 May 2026) | 17 Oct 2026 |
| S34 | Search results for "Actionstep" | Microsoft Marketplace | https://marketplace.microsoft.com/en-gb/search/products?search=Actionstep | No date shown; listed Actionstep for Word, Actionstep for Outlook and Actionstep Builder for Word | 17 Oct 2026 |
| S35 | Connectors directory | Anthropic | https://claude.com/connectors | No date shown | 17 Oct 2026 |
| S36 | Get started with connectors | Anthropic | https://claude.com/docs/connectors/getting-started | No date shown (page metadata 25 Sep 2026) | 17 Oct 2026 |
| S37 | ChatGPT Plugins (including the Legal category) | OpenAI | https://openai.com/business/plugins/ | No date shown | 17 Oct 2026 |
| S38 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Updated 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S39 | List of all Copilot Studio, Power Platform and Logic Apps connectors | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/connector-reference/ | Updated 2 Oct 2026 (page metadata) | 17 Oct 2026 |
| S40 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 17 Oct 2026 |
| S41 | Actionstep MCP | Zapier | https://zapier.com/mcp/actionstep | No date shown | 17 Oct 2026 |
| S42 | Gmail (integration page) | Actionstep | https://www.actionstep.com/integrations/gmail/ | No date shown (page metadata 29 Sep 2024) | 17 Oct 2026 |
| S43 | Google Drive (integration page) | Actionstep | https://www.actionstep.com/integrations/google-drive/ | No date shown (page metadata 29 Sep 2024) | 17 Oct 2026 |
