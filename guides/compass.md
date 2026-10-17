# Compass: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Compass is a school management system made by Compass Education, based in Hawthorn, Victoria. Schools use it for attendance, Chronicle behaviour and wellbeing notes, learning tasks, reports, payments and parent messages. [S2] [S7] [S11]
- Compass's AI offer is called Compass AI. It works through a connector that lets a school "bring its own LLM". In plain terms, staff ask an outside assistant such as Claude, and the assistant reads Compass data to answer. [S8] [S9]
- The connector is read-only. Compass says it "cannot create, change or delete anything in Compass". [S9]
- Nothing connects by default. Your Compass account manager has to switch the feature on, and your school has to approve each AI provider before staff can sign in. [S9] [S10]
- Compass publishes setup steps for Claude, as a custom connector, and for Gemini Enterprise, set up once by a school's Google administrator. Anthropic's connector directory doesn't list Compass yet. [S9] [S28]
- Compass's privacy addendum also names ChatGPT and Microsoft Copilot as examples. We found no Compass setup steps for either, and no Compass listing in OpenAI's or Microsoft's directories. [S10] [S9] [S34] [S35]
- Compass says it doesn't use connector data to train AI and doesn't store your AI conversations. Once data reaches the AI provider, that provider's own policy decides how long it's kept. [S10]
- The assistant only sees what your Compass role allows. Compass strips medical, access-restriction and contact details, but two tools can return free-text notes that may mention health or pastoral matters. [S9]
- Inside Compass, an AI support agent called Susie answers how-to questions. Compass's timetabling product, Griddle, uses AI to build elective lines. [S17] [S22]

## The tool, and the plans that matter

Compass is a cloud-based school management system developed in Australia. [S25] [S5]

The company, Compass Education Pty Ltd, has its registered office in Hawthorn, Victoria. [S11]

- Compass says it was founded in 2010 and now supports "5,000+ schools and 5M users". [S2]
- Its PCI DSS page says it works "with over 1,800 schools in Australia". [S25]
- Compass says it's Department of Education approved in NSW, Victoria, Queensland, Tasmania and WA. [S3]
- It says more than 700 Catholic schools use it through a partnership with CEnet. [S4]
- Independent schools can buy Compass Private, which Compass calls "Compass's bespoke solution" for independent schools. [S5]
- In WA, Compass announced in August 2023 that it had won the tender to supply school management software to more than 800 public schools. [S24]
- Compass says it's hosted "from Australia-based data centres". [S6]
- It lists ISO 27001 and PCI DSS Level 1 among its security credentials. [S2] [S25]
- We found no prices on Compass's website. It offers demos and an information pack instead. [S1]

| What | Who it's for | AI in it | Price |
|---|---|---|---|
| Compass (the school management system) | Government, Catholic and independent schools | Susie, the AI support agent. The Compass AI connector once it's switched on. | Not published |
| Compass Private | Independent schools | Not described separately | Not published |
| Compass AI | Schools that register interest | A read-only connector for outside assistants. Setup steps exist for Claude and Gemini Enterprise. | Not published |
| Griddle | School timetablers | AI line generation for elective classes | Not published. Griddle offers to cover its subscription until a school's current timetabling licence ends. |

Sources for the table: [S1] [S5] [S8] [S9] [S17] [S21] [S22]

- Compass AI sits on top of CompassOS, which Compass describes as the layer that joins its products under one login. CompassOS is "currently in a pilot phase with a small number of schools". [S8]
- The Compass AI page invites schools to register interest. It gives no release date or price. [S8]
- Compass's features page groups its modules into five areas: leadership and administration, wellbeing, school community, learning management, and finance. [S7]

## AI built in

### Compass AI (through your own assistant)

**What it does**

- Compass says "Compass AI puts that connected picture to work, using the tools your staff already rely on." [S8]
- "At its core is the Compass MCP Connector, which lets a school bring its own LLM tool". An LLM (large language model) is the engine behind assistants such as Claude and Gemini. [S8]
- Compass says that with student, attendance, extracurricular, timetable and activity data in one place, "Compass AI can answer complex questions across the whole school". [S8]
- The questions and answers happen in the outside assistant. Compass supplies the data, read-only. Each connection is covered under "Outside AI that connects" below. [S9]

**Where to find it**

- The Compass AI page asks schools to register interest. [S8]
- The connector only works once "your Compass account manager" has switched the Compass AI feature on for your school. Until then, sign-in works but every request returns an error. [S9]

**Which plans have it**

- Compass doesn't say which contracts include Compass AI or what it costs. [S8] [S9]

**What happens to your data**

- Compass says the connector fetches only what each request needs. It "does not pre-index or continuously sync your Compass data" and keeps nothing beyond the active session. [S10]
- Compass says it doesn't use connector data to train AI or machine learning models, or for advertising. [S10]
- Compass says it "does not independently store the content of your AI conversations or the Compass data returned during a session". [S10]
- The AI provider handles the data under its own policy. Compass "does not control how AI providers handle or retain data once it has been transmitted". [S10]
- Admin switches: the account manager turns the feature on, and the school or education authority approves each AI provider. School administrators manage who holds the permissions needed, and can remove a person's access. [S9] [S10]

**In Australia**

- The Compass AI page sits on Compass's Australian site, and the privacy addendum points Australian complaints to the Office of the Australian Information Commissioner. [S8] [S10]
- A Compass UK post from July 2026 says Compass's AI features are "soon to be released in the UK". That suggests Australian schools have them first. That's our inference. [S19]

### Susie, Compass's AI support agent

**What it does**

- Compass introduced Susie in April 2025 as "our new AI-powered support agent". [S17]
- Susie answers questions about using Compass with "instant answers and step-by-step guidance", at any time of day. [S17]
- If needed, Susie hands you over to Compass's support team. [S17]
- Compass says Susie "learns over time to better respond to your needs". [S17]

**Where to find it**

- Compass says Susie is "live on every page within Compass". You type your question. [S17]

**Which plans have it**

- The announcement doesn't limit Susie to any plan. [S17]

**What happens to your data**

- Compass doesn't say what powers Susie, where your questions go or how long they're kept. [S17]
- Compass's main privacy policy doesn't mention AI. [S11]

**In Australia**

- Susie was announced in Compass's Australian customer updates. [S17]
- Compass's UK pages describe a similar agent called Terry, which "uses knowledge base content created by our Customer Success, Training and Support teams". [S18]

### Griddle line generation (Compass's timetabling product)

- **What it does:** Griddle builds school timetables. Its line generation page says "Harness the power of AI and generate the most efficient combination of classes possible." [S22]
- Griddle says its automated tools take the strain while you "retain the flexibility to intervene manually". [S22]
- **Where to find it:** Griddle is a separate product that syncs with Compass. Compass calls it "our cloud-based timetabling platform". [S20] [S14]
- Griddle's about page says its general manager joined Compass in 2022 and now leads Griddle. [S23]
- **Which plans have it:** It's a Griddle subscription. Griddle offers to cover it until a school's current timetabling licence expires. No prices are published. [S21]
- **What happens to your data:** Griddle's pages don't say how its AI uses school data. [S21] [S22]
- **In Australia:** Compass held a Griddle launch event in Melbourne in March 2024. It says Griddle was developed with A2I2 at Deakin University. [S20]

### AI in Compass's security monitoring (described in 2024)

- Compass's August 2024 EduTECH post says its platform includes "AI and machine learning to monitor activity and restrict access from high-risk regions". [S27]
- The same post lists multi-factor authentication and ISO27001 certification. [S27]
- We found no other description of this monitoring, and no setting for it. [S27]

## Outside AI that connects

A quick translation of the jargon. **MCP** (Model Context Protocol) is "an open standard that enables AI assistants to securely interact with external services", in Compass's words. A **connector** is the link an assistant uses to reach another service. [S10]

- Compass's connector goes by three names: "Compass AI Agent Connector" in the privacy addendum, "Compass MCP Connector" on the Compass AI page, and "Compass Education for AI assistants" on the setup page. [S10] [S8] [S9]
- "The Connector is operated by Compass", at https://mcp.compass.education/mcp. [S10] [S9]
- Compass says it "is compatible with any MCP-supported AI provider that has been approved by a school". [S10]
- Two things must happen at school level first: Compass AI switched on, and the AI provider approved. Then each person needs the right Compass permissions and signs in for themselves. [S9] [S10]

### Claude and Compass

**Official?**

- Yes, on Compass's side. Compass runs the connector, and its setup page gives steps for Claude. [S9] [S10]
- It isn't in Anthropic's Connectors Directory. The directory's published list on 17 October 2026 had no Compass Education connector, and Compass says a listing is still to come. [S28] [S9]
- So you add it as a custom connector. Anthropic says custom connectors "allow connections to unverified services". [S29]

**What it can see and do**

- Read-only. It "cannot create, change or delete anything in Compass". [S9]
- Compass lists 27 tools. They cover the student directory and profiles, Chronicle entries, attendance, learning tasks with results, calendars and class schedules, school events, and reference lists such as year levels and terms. [S9]
- You only see what your Compass role allows. Tools your role can't use are hidden. [S9]
- Compass says "A parent only sees their own children", which suggests parent accounts can connect too where a school allows it. That's our reading. [S9]
- Compass says "Medical, access-restriction and contact PII are stripped server-side before they reach the assistant." PII means personally identifiable information. [S9]
- Two tools go further. The single Chronicle entry tool returns the full entry, "unredacted by design". Attendance notes' free text "may carry medical / pastoral commentary". [S9]
- The student record tool returns counts only, such as how many medical records exist, without their contents. [S9]
- The privacy addendum also lists "Communication records (where permitted by your school's Compass configuration)". The published tool list has no messages tool. [S10] [S9]
- In ordinary chats, Claude asks for your approval before it uses a connector's tools. [S30]

**What you need**

- Compass AI switched on for your school by your Compass account manager. [S9]
- Your school or education authority's approval of Claude as an AI provider. [S10]
- The Compass permissions your school requires for the connector. [S10]
- A Claude account. On the Free plan you can add one custom connector. Pro and Max users add their own. [S29] [S30]
- On Claude Team or Enterprise, an Owner adds the custom connector for the organisation first. Members can't add it themselves. [S29] [S30]

**Steps to connect** (Compass's setup page, not dated, and Anthropic's docs)

1. In Claude on the web or desktop, go to **Customize > Connectors**. Compass's page calls this **Settings › Connectors**. [S29] [S9]
2. Click **Add custom connector**. [S9] [S29]
3. Paste `https://mcp.compass.education/mcp` as the server URL, then click **Add**. [S9]
4. Claude opens Compass's school picker. Search for your school by name. [S9]
5. Log in with your normal Compass details. Compass says your assistant "never sees your password". [S9]
6. In a chat, click **+**, choose **Connectors** and switch Compass on for that conversation. [S29]
7. Ask a question. One of Compass's examples is "What does Alice have due in the next fortnight across all her subjects?" [S9]

On Team and Enterprise plans, an Owner first goes to **Organization settings > Connectors**, selects **Add**, then **Custom**, and chooses **Web** if asked. They enter the URL and click **Add**. Members then find the connector under **Customize > Connectors** with the **Custom** label and click **Connect**. [S29]

**To disconnect**

- In Claude, go to **Customize > Connectors** and click **Remove**, or the three-dot menu next to Compass. Owners use **Organization settings > Connectors**. [S29]
- In Compass, ask your school administrator to remove MCP access from your account. [S10]
- Or email legal@compass.education. Compass says it will revoke your access token within 5 business days. [S10]
- Revoking doesn't touch your Compass account. Data that already passed through the AI provider stays under that provider's retention policy. [S10]

**Limits**

- Compass says each provider's handling of the data "is governed by their own privacy policy". [S10]
- Anthropic says its consumer plans (Free, Pro and Max) use chats for training if you allow it. It leaves out "raw content from connectors", including remote MCP servers, unless that content is copied into the conversation. [S31]
- Anthropic says it won't use inputs or outputs from its commercial products, such as Claude for Work, to train its models by default. [S32]
- Anthropic warns that malicious servers can hide instructions for Claude, and that a developer can change how a tool behaves after you connect. [S30]
- If a tool says you're not authorised, Compass suggests asking the assistant to run its key-check tool and sharing the result with your Compass admin. [S9]

### ChatGPT and Compass

**Official?**

- No official connection found. [S9] [S34]
- Compass's privacy addendum names ChatGPT (OpenAI) as an example of an approved assistant, where it supports MCP. [S10]
- Compass's setup page gives no ChatGPT steps, and OpenAI's public plugin pages list no Compass plugin. [S9] [S34]

**What it can see and do**

- Nothing documented. [S9]

**What you need, steps, disconnecting**

- Not documented by Compass. [S9]
- In general, OpenAI lets ChatGPT Business, Enterprise and Edu workspaces connect a custom MCP server from **Plugins**, using **Add custom MCP server**. In Business, only admins and owners can create and publish one. [S33]
- Compass doesn't say whether its connector works that way, and the school would still have to approve ChatGPT first. [S10] [S9]

**Limits**

- OpenAI says you're responsible for vetting any third-party MCP server you add to a workspace. [S33]

### Microsoft Copilot and Compass

**Official?**

- No official connection found. [S9] [S35] [S36] [S37]
- Compass's privacy addendum names Copilot (Microsoft) as an example assistant. Its setup page gives no Copilot steps. [S10] [S9]
- Microsoft's list of federated Copilot connectors, last updated 16 October 2026, doesn't include Compass. Neither does Microsoft's partner connector gallery or a Microsoft Marketplace search for "compass education". [S35] [S36] [S37]

**What it can see and do**

- Nothing documented. [S9]
- Compass does link to Office 365 outside its partner program, alongside things like single sign-on and calendar feeds. Compass doesn't describe that as an AI connection. [S13]
- Copilot inside your school's own Microsoft 365 is covered in our separate Microsoft 365 guide.

**Limits**

- Microsoft says partners can submit federated connectors to Microsoft for approval. Compass isn't on the published list. [S35]

### Google Gemini and Compass

**Official?**

- Yes, for Gemini Enterprise only. Compass's setup page has a section headed "Gemini Enterprise (school IT admin only)". [S9]
- Gemini Enterprise is a Google Cloud product. Google's setup guide covers its Standard, Plus, Pay-as-you-go and Frontline editions. [S38]
- The everyday Gemini app doesn't list Compass among its connected apps. [S39]
- Gemini's custom apps for personal accounts are for people 18 and over in the US, and the feature "isn't available if you sign in with a work or school Google Account". [S40]

**What it can see and do**

- The same read-only connector and tools as Claude. [S9]
- One admin connects it for the whole school. Staff in the groups the admin authorises can then ask Gemini about Compass data "without each user adding their own connector". [S9]
- Each person still sees only what their own Compass role shows them. [S9]
- Google says every action call needs the user's confirmation by default, unless the tool is marked read-only. [S38]

**What you need**

- A Google Workspace administrator with access to Gemini Enterprise. [S9]
- Google lists set-up work in Google Cloud first, including an organisation policy override for custom MCP data stores and the Discovery Engine Editor role. [S38]
- Compass AI switched on for the school, and Gemini approved as an AI provider. [S9] [S10]

**Steps to connect** (Compass's setup page, not dated; Google's guide, updated 16 October 2026)

1. Sign in to the Gemini Enterprise admin console as a Workspace administrator. [S9]
2. Compass says to go to **Connectors › Custom MCP server › Add custom MCP server**. Google's guide describes this as **Data stores**, then **Create data store**, then searching for **Custom MCP Server** and clicking **Add MCP server**. [S9] [S38]
3. Paste `https://mcp.compass.education/mcp` as the server URL. [S9]
4. Confirm the sign-in (OAuth) handshake. A school picker appears. Pick your school once and Gemini remembers it for the whole organisation. [S9]
5. Authorise the connector for the staff groups who should use it. [S9]
6. Google's guide says no tools are switched on at first. Open the data store, click **Actions > Reload custom actions**, select the actions and click **Enable actions**. [S38]

**To disconnect**

- Compass doesn't give Gemini Enterprise removal steps, and Google's setup guide doesn't cover deleting the data store. [S9] [S38]
- The Compass-side routes still work: ask your school administrator, or email legal@compass.education. [S10]

**Limits**

- Compass says its connector appears to Gemini Enterprise "as a standard third-party MCP server, so the same admin docs apply (including audit logging and per-group access control)". [S9]
- Google's guide lets the admin pick a "Multi-region" location but says nothing more about where the data is processed. [S38]

### Compass's Public API (the developer route)

**Official?**

- Yes. The Compass Public API "is available for 3rd party vendors and schools to develop against". [S15]
- Compass's integrations page describes "a robust, public RESTful API". [S14]

**What it can see and do**

- The documentation lists 183 endpoints. Some only read, and others create or change records such as Chronicle entries, events and clubs. [S15]
- Compass says API use "is recorded with personally identifiable information for auditing purposes". [S15]

**What you need**

- Permission from Compass: "Please contact Compass Support to request access." [S15]
- The person whose API key is used needs the APIAccess permission. The key is shown in People Management. [S15]
- Software vendors go through Compass's Approved Integration Partner process. Compass asks for evidence such as ISO 27001 certification and hosting details, and says hosting "in most jurisdictions" has to be onshore. [S13]
- Compass says the review "may take 3-6 months", and approval comes with a pricing assessment for setup and ongoing use. [S13]

**Steps to connect** (Compass's API documentation and partner page, neither dated)

1. Contact Compass Support and name the school or vendor you represent. [S15]
2. Vendors email legal@compass.education with the integration type, the data needed, security evidence and how often they'll call the API. [S13]
3. Once approved, send requests with the person's key in the CompassApiKey header. [S15]

**To disconnect**

- Not documented. [S15] [S13]

**Limits**

- Use "is limited to pre-approved vendors and schools", and some may be rate-limited. [S15]
- "Frequent (multi-day) API requests for large data sets will not typically be permitted." [S13]
- Compass's terms say access to the platform for "third-party integration (including automated or manual processes) is not permitted", and Compass watches for "screen scraping, bot use and script automation". [S12]

### Zapier, Make and Power Automate

- Compass's integrations page names none of them. [S14]
- Compass lists RSS feeds, SchoolFront news widgets, iCal, SAML/SSO, Google Apps and Office 365 as integrations available outside its partner program. [S13]

## Jobs it's good for

- **One student's attendance.** Ask "Show me Harry Smith's attendance for the current term and flag any unapproved absences." That's one of Compass's own examples. [S9]
- **A year level at a glance.** The cohort attendance tool lists each student's class percentage, so you can ask which Year 8 students are below 80%. [S9]
- **What's due.** Ask what a student has due in the next fortnight across all subjects. [S9]
- **When a class meets.** Ask when Year 11 Business Management next meets and who's rostered. [S9]
- **This week's Chronicle.** List the Chronicle entries logged this week for Year 9, grouped by category. The list tools return structured fields without the free-text body. [S9]
- **Calendar sums.** Ask how many teaching days are in a month, or when Term 2 starts. [S9]
- **"How do I" questions.** Ask Susie inside Compass. [S17]
- **Elective lines.** Timetablers can let Griddle's AI build the lines, then adjust them by hand. [S22]

## What to watch for

**Student data leaves Compass**

- When the connector runs, "your Compass data passes through the AI provider's infrastructure". [S10]
- Compass doesn't control how the provider keeps it, so read that provider's privacy policy before you connect. [S10]
- Compass recommends schools "consult with their privacy officer or legal adviser before enabling any AI integration". [S10]
- It also asks administrators to review their obligations under "applicable state and federal privacy legislation" before staff use the connector with student data. [S10]

**Not every sensitive detail is filtered**

- Medical, access-restriction and contact details are stripped. [S9]
- The full Chronicle entry tool is "unredacted by design", and attendance notes can include health or pastoral comments. [S9]
- Chronicle entries and attendance notes are free text that people type. Text like that could carry instructions aimed at the AI. That's our inference, based on Anthropic's warning about hidden instructions. [S30]

**The login sets the limit**

- The assistant sees only what your Compass role can see. [S9]
- So an administrator's login exposes everything that administrator can see. That's our inference from the above.

**Personal AI accounts**

- On Claude's Free, Pro and Max plans, chats can be used for training if you allow it. Raw connector content is left out unless it's copied into the chat. [S31]
- Claude's work plans aren't used for training by default. [S32]
- Compass leaves the choice of AI provider to the school. Our reading: student data belongs in an account your school has approved and manages. [S10]

**Department schools**

- Compass won the WA Department of Education's tender to supply more than 800 public schools. [S24]
- Compass says the connector needs approval from "the user's school or education authority". Our reading: in a department school, check with the department before you connect. [S10]

**Menu names differ**

- Compass's page says **Settings › Connectors** in Claude. Anthropic's current docs say **Customize > Connectors**. [S9] [S29]
- Compass's Gemini Enterprise menu path doesn't match Google's own guide. [S9] [S38]

**Cost**

- Compass hasn't published a price for Compass AI. [S8]
- Claude's Free plan allows one custom connector. [S30]
- Gemini Enterprise is a separate Google Cloud product. We didn't research its price. [S38]

**Who switches what**

- Your Compass account manager: the Compass AI feature. [S9]
- Your school or education authority: which AI providers are approved. [S10]
- School administrators: user permissions, and removing a person's MCP access. [S10]
- Claude Team and Enterprise Owners: adding the custom connector for the organisation. [S29]
- Your Google Workspace administrator: the Gemini Enterprise connector, and which staff groups get it. [S9]

**Check the answers**

- Compass says a "no results" answer is "usually a scope or phrasing mismatch". Ask again and name the year level, dates or student. [S9]

**Logins and AI browser agents**

- Compass's terms forbid shared logins and third-party integration through the platform, and Compass watches for bots. [S12]
- Our reading: use the connector your school has approved, and don't give any AI tool your Compass password. This isn't legal advice.

## Announced changes

- **24 April 2025:** Susie launched. [S17]
- **14 May 2026:** the last change to Compass's AI/MCP privacy addendum, according to the page's details. [S10]
- **9 June 2026:** the Compass OS and Compass AI register-interest page went up. It was updated on 13 July 2026. [S8]
- **CompassOS:** in a pilot with a small number of schools. Compass plans a phased rollout and says it will eventually be on for every school, with no opt-out once it's generally available. [S8]
- **Coming, no date:** a Compass listing in Anthropic's Connectors Directory, so Claude users can add it without pasting the URL. [S9]
- **July 2026 (UK):** Compass said its AI features are "soon to be released in the UK", to help schools pull inspection evidence with plain-language questions. [S19]

## What we couldn't establish

- **Compass AI's price**, and which contracts include it. [S8] [S9]
- **When Compass AI became available** to Australian schools. The page asks for interest and gives no date. [S8]
- **ChatGPT and Copilot.** Compass names them as examples but documents no setup, so we couldn't confirm either works with the connector. [S10] [S9]
- **Where the connector runs.** Compass says schools are hosted in Australian data centres, but doesn't say which country the connector's servers are in. [S6] [S10]
- **Sign-in permissions.** The addendum says access depends on "the permissions you grant during the OAuth authorisation flow". The connector's public sign-in settings list a single permission, called "compass". We couldn't see the sign-in screen itself. [S10] [S16]
- **The Compass account setting.** The addendum says you can revoke permissions in "your Compass account settings". The setup page doesn't describe that setting. [S10] [S9]
- **What powers Susie**, and what happens to the questions you type. [S17]
- **Whether Australian schools also have Terry**, or whether Terry and Susie are the same service. [S17] [S18]
- **How Griddle's AI uses school data.** [S21] [S22]
- **The 2024 AI security monitoring.** One blog post mentions it, and we found no detail. [S27]
- **Compass's own help articles.** Its public Help Centre shows only parent videos and a parent guide, so we couldn't read staff help on AI. [S26]
- **Gemini Enterprise sign-in details.** Google's guide asks for OAuth details such as a client ID. Compass's page only says to "Confirm the OAuth handshake". [S38] [S9]
- **Dates on Compass's policies.** The privacy policy and the addendum show no date on the page itself. We took their dates from the pages' details. [S11] [S10]
- **OpenAI's in-app plugin directory** needs a login, so we checked OpenAI's public plugin pages only. [S34]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Compass school management software (home page, Australia) | Compass Education | https://www.compass.education/ | No date shown (page metadata 13 Oct 2026) | 17 Oct 2026 |
| S2 | About Compass | Compass Education | https://www.compass.education/about-compass/ | No date shown (page metadata 14 Apr 2026) | 17 Oct 2026 |
| S3 | School management software for Government schools | Compass Education | https://www.compass.education/government-school-management-software/ | No date shown (page metadata 14 Apr 2026) | 17 Oct 2026 |
| S4 | School management software for Catholic schools | Compass Education | https://www.compass.education/catholic-school-management-software/ | No date shown (page metadata 14 Apr 2026) | 17 Oct 2026 |
| S5 | School management software for Independent schools | Compass Education | https://www.compass.education/independent-school-management-software/ | No date shown (page metadata 14 Apr 2026) | 17 Oct 2026 |
| S6 | Compass for Schools | Compass Education | https://www.compass.education/compass-features/compass-for-schools/ | No date shown (page metadata 19 Jun 2026) | 17 Oct 2026 |
| S7 | Features | Compass Education | https://www.compass.education/features/ | No date shown (page metadata 17 Jun 2026) | 17 Oct 2026 |
| S8 | Register your interest in Compass OS & Compass AI | Compass Education | https://www.compass.education/register-your-interest-compass-os-compass-ai/ | No date shown (page metadata: published 9 Jun 2026, updated 13 Jul 2026) | 17 Oct 2026 |
| S9 | Compass Education for AI assistants: connector reference | Compass Education | https://mcp.compass.education/help | No date shown | 17 Oct 2026 |
| S10 | Privacy Policy (AI/MCP): Agent Connector Addendum | Compass Education | https://policies.compass.education/privacy-policy-aimcp | No date shown on the page ("Page details" metadata 14 May 2026) | 17 Oct 2026 |
| S11 | Privacy Policy (Australia, the US and other countries) | Compass Education | https://policies.compass.education/privacy | No date shown on the page ("Page details" metadata 8 Nov 2023) | 17 Oct 2026 |
| S12 | Terms of Use | Compass Education | https://policies.compass.education/ | No date shown on the page ("Page details" metadata 10 Mar 2026) | 17 Oct 2026 |
| S13 | Integration Partners (Approved Integration Partner process) | Compass Education | https://policies.compass.education/integration-partners | No date shown on the page ("Page details" metadata 5 Oct 2023) | 17 Oct 2026 |
| S14 | Integrations | Compass Education | https://www.compass.education/integrations/ | No date shown (page metadata 6 Oct 2026) | 17 Oct 2026 |
| S15 | Compass Public API documentation (version 4.0.0) | Compass Education | https://docs.compass.education/ | No date shown (generated 16 Oct 2026, per page metadata) | 17 Oct 2026 |
| S16 | Compass MCP server sign-in settings (OAuth resource metadata) | Compass Education | https://mcp.compass.education/.well-known/oauth-protected-resource | No date shown | 17 Oct 2026 |
| S17 | Welcome Back to Term 2 (Introducing Susie) | Compass Education | https://www.compass.education/post/welcome-back-to-term-2/ | 24 Apr 2025 | 17 Oct 2026 |
| S18 | Independent School Management Information System (UK) | Compass Education | https://www.compass.education/uk/products/independent-school-management-information-system/ | No date shown (page metadata 25 Jun 2026) | 17 Oct 2026 |
| S19 | Ofsted's new inspection framework explained (UK) | Compass Education | https://www.compass.education/uk/post/ofsted-new-inspection-framework-explained/ | 27 Jul 2026 (page metadata: updated 28 Sep 2026) | 17 Oct 2026 |
| S20 | Griddle launch event | Compass Education | https://www.compass.education/griddle-launch-event/ | No date shown (event on 13 Mar 2024; page metadata 22 Mar 2024) | 17 Oct 2026 |
| S21 | Griddle: Simplified Scheduling (home page) | Griddle (Compass) | https://www.griddle.education/ | No date shown (page metadata 26 Aug 2026) | 17 Oct 2026 |
| S22 | Line Generation | Griddle (Compass) | https://www.griddle.education/features/line-generation/ | No date shown (page metadata 26 Aug 2026) | 17 Oct 2026 |
| S23 | About Griddle | Griddle (Compass) | https://www.griddle.education/about/ | No date shown (page metadata 12 Oct 2026) | 17 Oct 2026 |
| S24 | Compass Secures WA DoE Contract | Compass Education | https://www.compass.education/post/compass-secures-wa-doe-contract/ | 7 Feb 2024 (release dated 22 Aug 2023) | 17 Oct 2026 |
| S25 | PCI DSS Compliance | Compass Education | https://www.compass.education/pcidss/ | No date shown (page metadata 17 Jun 2026) | 17 Oct 2026 |
| S26 | Compass Help Centre | Compass Education | https://support.compass.education/en/ | No date shown | 17 Oct 2026 |
| S27 | Cyber security in schools: insights from EduTECH 2024 | Compass Education | https://www.compass.education/post/cyber-security-in-schools-insights-from-edutech-2024/ | 22 Aug 2024 | 17 Oct 2026 |
| S28 | Claude site map (Connectors Directory pages; 973 connectors listed, none for Compass Education) | Anthropic | https://claude.com/sitemap.xml | No date shown | 17 Oct 2026 |
| S29 | Add a connector that isn't in the directory | Anthropic | https://claude.com/docs/connectors/custom/add-unlisted | No date shown (page metadata 25 Sep 2026) | 17 Oct 2026 |
| S30 | Get started with custom connectors using remote MCP | Anthropic Help Center | https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp | "Updated over 2 weeks ago" (timestamp 1 Oct 2026) | 17 Oct 2026 |
| S31 | Is my data used for model training? (consumer products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | 16 Mar 2026 | 17 Oct 2026 |
| S32 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | 18 Aug 2026 | 17 Oct 2026 |
| S33 | Connecting custom MCP servers in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12584461-connecting-custom-mcp-servers-in-chatgpt | "Updated: 11 hours ago" (timestamp 16 Oct 2026, 23:50 UTC) | 17 Oct 2026 |
| S34 | OpenAI plugin directory pages (13 category site maps, 336 plugin pages, none for Compass) | OpenAI | https://openai.com/sitemap.xml | No date shown | 17 Oct 2026 |
| S35 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Last updated on 16 Oct 2026 | 17 Oct 2026 |
| S36 | Partner-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-partners | Last updated on 27 Apr 2026 | 17 Oct 2026 |
| S37 | Microsoft Marketplace search: "compass education" (no Compass Education listing) | Microsoft | https://appsource.microsoft.com/en-us/marketplace/apps?search=compass%20education | No date shown | 17 Oct 2026 |
| S38 | Set up a custom MCP server (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server | Last updated 16 Oct 2026 (UTC) | 17 Oct 2026 |
| S39 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S40 | Connect & manage custom apps for Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/answer/17209137 | No date shown | 17 Oct 2026 |
