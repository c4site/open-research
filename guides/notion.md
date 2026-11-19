# Notion: the AI inside it, and the AI that connects to it

Researched 18 November 2026 from vendor documentation. Every line is tagged with its source.

Notion's help pages show no "last updated" date, so the Sources table records the day we read each one. OpenAI's help pages show a relative date ("21 days ago"), so we also give the page's timestamp in UTC. Microsoft's dates come from each page's own publishing data.

## The short version

- Notion's AI is called Notion AI. Its main parts are Notion Agent, a chat assistant that can create and edit pages, and Custom Agents, which run on a schedule or a trigger. [S3] [S5]
- Notion AI comes with the Business and Enterprise plans. Free and Plus get a limited trial. [S1] [S3]
- Notion's pricing page shows US dollars to visitors in Australia. Business is US$20 a seat a month billed yearly, or US$24 billed monthly. [S1]
- Since late October 2026, each Business and Enterprise seat includes 1,500 Standard and 500 Select AI credits a month. Existing customers moved to this on 2 November. [S1] [S63]
- Extra use, some high-cost models and workspace-funded Custom Agents run on Notion credits, which cost $10 per 1,000 a month or $13 per 1,000 as annual credits. [S6] [S64]
- Notion says your data isn't used to train AI models by default. Its AI providers keep data for 30 days or less on Free, Plus and Business, and most models keep nothing on Enterprise. [S15]
- Notion has no Australian data region. It offers the US, Europe, Japan and Korea, and AI providers process data outside the chosen region. [S17]
- ChatGPT and Claude connect through Notion's own MCP server. They can read your pages and, within your Notion permissions and approvals, create and update them. [S43] [S38] [S22]
- Claude can also work inside Notion as a teammate ("Claude agents", in beta), paid for in Notion credits. [S20]
- Microsoft Copilot can search Notion through a connector Microsoft built. Each user needs a Microsoft 365 Copilot licence. [S48] [S49]
- We found no Notion connection for the everyday Gemini app. Google's separate business product, Gemini Enterprise, has one. [S52] [S54]

## The tool, and the plans that matter

Notion is a workspace where teams keep pages, wikis and databases, such as project plans and task lists. Notion AI works inside it. [S3]

These are the prices on Notion's pricing page as shown to a visitor in Australia on 18 November 2026. The page says "Price in USD" and offers no other currency. [S1]

| Plan | Monthly (US$ a seat) | Yearly (US$ a seat a month) | Notion AI | Worth knowing |
|---|---|---|---|---|
| Free | US$0 | US$0 | Limited trial of Standard credits | 7-day page history, 10 guests |
| Plus | US$12 | US$10 | Limited trial of Standard credits | 30-day page history, "Basic connections" |
| Business | US$24 | US$20 | 1,500 Standard and 500 Select credits a seat each month. Adds Custom Agents, Enterprise Search (beta) and Workers (beta) | SAML single sign-on, private teamspaces, 90-day page history |
| Enterprise | "Custom pricing" | "Custom pricing" | As Business with "Custom credit amounts", plus "Zero data retention with LLM providers" | Audit log, user provisioning (SCIM), custom page history |

Sources for the table: [S1]

- The pricing page lists AI data retention as "30 day retention" on Free, Plus and Business, and "Zero data retention" on Enterprise. [S1]
- The page says admins can buy Notion credits "to cover additional AI usage". [S1]
- The page notes: "Plans may not be available for every workspace." [S1]
- The page doesn't say whether prices include GST or other tax. [S1]
- The Plus plan, limited to one member, is free for students and educators who sign up with a school email address. It includes only the AI trial. [S1]

**Words used in this guide**

- **Notion Agent** is the chat assistant inside Notion. It "has the same permissions you do." [S4]
- **Custom Agents** are agents a team sets up to run "automatically in the background based on triggers and schedules". [S5]
- **Standard credits** come with each Business and Enterprise seat and cover "work where Notion picks the model". **Select credits** also come with each seat and cover "work where you pick a model yourself, or use a Custom Agent you set up". [S7]
- **Notion credits** are a paid add-on for Business and Enterprise. They pay for Custom Agents, Workers, high credit consumption models and extra AI use beyond your Standard and Select credits. [S6]
- **Notion AI Connectors** let Notion AI search other apps, such as Slack and Google Drive. [S12]
- **Notion MCP** is Notion's own server that lets outside assistants, such as Claude and ChatGPT, read and write in your workspace. MCP is a standard plug for connecting AI assistants to other software. [S22]

**Notion credits and allowances**

- Each Business and Enterprise member gets 1,500 Standard credits and 500 Select credits a month. They reset monthly and don't roll over. [S9]
- Standard and Select credits belong to each person. They can't be pooled, moved between people or swapped for another kind. [S7]
- Notion estimates a simple task uses about 5 credits and a complex one about 25. [S7]
- When your Standard credits run out, features that use them pause until the monthly reset. An owner can let members keep going on Notion credits. That's off by default. [S9] [S7]
- Notion alerts you in Notion Agent chat when your Standard or Select credits are running low or have run out. [S9]
- Notion credits, the paid add-on, are shared across the workspace. Monthly credits cost $10 per 1,000 and reset each month, and unused credits don't carry over. [S6]
- Annual credits cost $13 per 1,000, are paid upfront and expire when your subscription renews. [S6]
- The credits help page shows "$" without naming the currency. The pricing page prices everything in US dollars. [S6] [S1]
- AI Meeting Notes will start using Standard credits on 1 December 2026. Notion estimates about 10 credits for a one-hour meeting. [S64]
- If your Notion subscription is billed through the Apple App Store or Google Play, you get the same monthly credits but can't buy more. [S7] [S6]

## AI built in

Three things apply to every feature in this section.

**Permissions.** Notion says "Notion AI can only ever use content you give it access to", and that it "never widens your access". [S15] Custom Agents are the exception: they have their own permissions (see below). [S56]

**Training and retention.** "By default, neither Notion nor our AI providers use your Customer Data to train any models." Notion's contracts with AI providers forbid it. [S15]
On Free, Plus and Business, the "AI provider retains your data for 30 days or fewer, then deletes it." [S15]
On Enterprise, most models keep nothing. A few don't offer zero data retention; they're off by default and a workspace owner must opt in. [S15]
Notion's thumbs up and thumbs down feedback "isn't used to train Notion AI". [S3]
Workspace owners can turn on **Share data to improve Notion AI** under **Settings** > **Notion AI**. [S3]

**Who runs it.** Notion AI "runs on a mix of large language models". Notion keeps the current list of AI providers on its sub-processor page. [S15]
That list names Anthropic, OpenAI, Google, Fireworks, Baseten, Cerebras, Modal and X.AI for hosting AI models. Most are listed as "Global" and the rest as the USA (X.AI also lists the UK). [S16]
Exa and Parallel Web Systems provide web search, and AssemblyAI provides transcription. [S16]

### Notion Agent (the chat assistant)

**What it does**

- Creates and edits pages and databases, using context from your workspace and connected apps. [S4]
- Answers questions about your workspace and connected apps such as Slack. It can query databases, read comments and search version history. [S4]
- Reads files you upload, including PDF, CSV, Excel, Word, PowerPoint and ZIP files, and can produce new files such as spreadsheets and slide decks. [S4]
- Once you connect your own Slack account, it can post messages, reply in threads and add reactions as you. [S4]
- With Gmail connected, it can search, draft and send email. Write actions such as sending ask you to confirm first. [S4]
- It can schedule meetings once you connect a calendar. [S4]
- On Business and Enterprise it can also use other apps' MCP servers. Each person connects their own, from **All sources** > **MCP servers** > **Add MCP server** or **Settings** > **Connections** > **Discover**. [S27]
- Admins can limit members to an approved list of MCP servers, and choose whether members can add their own. [S27]
- It can't share pages or change page permissions, create comments, start AI Meeting Notes or change workspace settings. [S4]
- Notion AI can also translate pages, fill in database fields (Autofill) and write in AI blocks. [S3]
- Since 19 October 2026, Notion says its agents have "their own computer and browser" and can work on a task for up to 24 hours. A new "Review for me" mode uses a separate model to check an action is safe first. [S62] [S63]
- Image generation is in beta, with limits of 10 images or edits per 24 hours and 30 per 30 days for each person. [S3]

**Where to find it**

- Click the face at the bottom of Notion to open a chat. [S4]
- Or use the shortcut shift + cmd/ctrl + J, which works even when you're not in Notion. [S3]
- Leave the model on **Auto** to let Notion choose. On Business and Enterprise, Auto uses your Standard credits and picking a model yourself uses your Select credits. [S4]

**Which plans have it**

- "Notion AI is available on Business and Enterprise Plans." Free and Plus get "a limited number of complimentary AI responses". [S3]
- High credit consumption models, which Notion's blog says include Fable and Astra, need Notion credits. They stay off "until a workspace owner turns them on". [S8] [S63]
- If your workspace is on Business or Enterprise, you can pay for GPT models in Notion Agent with your own ChatGPT Plus, Pro, Business or Go plan (see "ChatGPT and Notion"). [S28]

**What happens to your data**

- The shared rules at the start of this section apply. [S15]
- Owners can cap how many Notion credits a person, group or agent can spend. [S8]
- Owners can turn web search off for the whole workspace under **Settings** > **Notion AI** > **AI Web Search** > **Enable web search for workspace**. **Require confirmation for web requests** makes the AI ask before visiting websites. [S3]
- Notion warns that in Enterprise Search, "depending on the model you choose, Notion AI may look only at information from the web". [S11]

**In Australia**

- The Notion AI pages we read don't mention any country limits. [S3] [S4]
- Data residency doesn't keep AI processing in one region; see "What to watch for". [S17]

### Custom Agents (agents that run on their own)

**What it does**

- Reads from Notion pages, databases and some connected apps. [S5]
- Runs on a schedule (daily, weekly, monthly and more) or when something happens, such as a database change, a new comment or a Slack message. [S5]
- Takes actions "such as posting reports, filing bugs, updating records, or sending messages". [S5]
- Hands parts of a job to other Custom Agents. [S5]
- Can use outside apps through MCP connections, such as Linear, Ramp and Figma. Write tools ask for confirmation by default. [S57]
- Can browse the web if you turn on its **Web access** toggle. [S5]

**Where to find it**

- Go to **Agents** in the sidebar and select **+**, then create with AI chat, from a template or from scratch. [S5]
- Each agent has **Chat**, **Activity** and **Settings** tabs. **Activity** logs every run. [S5]
- **Version history** lets you restore an earlier set-up. [S5]

**Which plans have it**

- Business and Enterprise only, on desktop or web. [S5]
- Custom Agents were free until 3 May 2026, then used Notion credits from 4 May 2026. [S34]
- Under the new credit system, a Custom Agent uses its owner's Select credits first, even when it's shared with the team. After that it uses any extra credits an owner has given, then the workspace's Notion credits if an owner allows it. [S65] [S2]
- If no credits are left, the agent pauses until credits reset or are added. Owners can also fund any agent with a monthly budget of Notion credits. [S65]
- Agents made before 2 November 2026 keep drawing on the workspace's shared credits. [S65]

**What happens to your data**

- A Custom Agent has its own access. Notion says: "When you share a Custom Agent, you're giving your team access to everything the agent can see." [S56]
- People using a shared agent "can retrieve information from resources they lack access to". [S56]
- New agents don't get access to all pages by default. A creator has to turn that on and accept a warning. [S56]
- Owners can choose who can create agents under **Settings** > **Notion AI** > **Agents** > **Control who can create agents**. The choices are **All workspace members** (the default), **Workspace owners only** and **Workspace owners + added groups only**. [S56]
- The Agent Directory in the same place lets admins see every agent and switch off editing, chatting and triggers. [S56]
- On Enterprise, the audit log records agent changes, and admins can change permissions on any agent. [S5] [S56]
- Notion says that when an agent uses Claude Fable 5, "Anthropic may store your prompts and responses for a period of time". An admin has to turn that model on. [S5]

**In Australia**

- The pages we read don't mention country limits. [S5]

### AI Meeting Notes

**What it does**

- Transcribes a meeting and writes a summary with key points and action items. [S10]
- You can upload an audio recording (AAC, M4A, MP3 or WAV) to be transcribed. [S10]
- It can label speakers, which works best in one-on-one video calls in the desktop app. Notion's page now lists 22 languages for speaker labels, but its FAQ still says English only. [S10]
- Since 31 July 2026, a finished meeting note can trigger a Custom Agent. [S29]

**Where to find it**

- Type **/meet** in a page in the desktop app, then select **Start transcribing**. [S10]
- Notion says that by selecting **Start transcribing** "you're confirming that everyone in the meeting has given their consent". [S10]
- A consent message can be played aloud or pasted into the meeting chat. Owners can switch on **Enforce consent for all workspace members**. [S10]

**Which plans have it**

- Business and Enterprise, and eligible mobile subscriptions that include Notion AI. [S10]
- It's limited to 10 hours a day per person. [S10]
- From 1 December 2026 it will use Standard credits, about 10 for a one-hour meeting by Notion's estimate. [S64] [S7]

**What happens to your data**

- Notion names OpenAI, Anthropic, Baseten, X.AI and AssemblyAI as the sub-processors for meeting notes. Fireworks is no longer on that list. [S10]
- Notion says its sub-processors don't store audio. If live transcription fails, Notion keeps uploaded audio for up to 3 days to retry. [S10]
- Saving audio on the recorder's computer is off by default. [S10]
- Meeting notes take on the permissions of the page they're saved on. [S10]
- Enterprise owners can set an automatic deletion schedule for transcripts. [S10]
- Owners can switch the feature off under **Settings** > **Meeting notes** by turning off **Enable Meeting notes for workspace**. [S10]

**In Australia**

- Notion lists English among 16 supported languages. [S10]
- Notion's consent advice discusses US and EU laws and recommends following "the strictest consent laws". It doesn't mention Australia. [S10] Check the rules where you and the other people in the meeting are before recording. That's our advice, and it isn't legal advice.

### Enterprise Search and Notion AI Connectors

**What it does**

- Searches your workspace, connected apps and the web in one go, and always cites its sources. [S11]
- Connectors cover Slack, Microsoft Teams, Google Drive, Microsoft SharePoint and OneDrive, Jira (beta), GitHub, Linear, Salesforce, Gmail, Microsoft Outlook and Google Calendar. [S12]
- Notion has replaced its SharePoint and OneDrive connector. If you hadn't moved by 31 October 2026, SharePoint access in Notion AI stays off until you set up the new one. Each person connects their own Microsoft account under **Settings** > **Connections** > **Browse**. [S14]
- You can pick GPT, Claude or Gemini models for a search. [S11]

**Where to find it**

- Open the **Home** tab and type your question in the search window. [S11]
- Use **All sources** to turn web search or connected apps on or off for a search. [S11]
- Owners set up connectors under **Settings** > **Notion AI**. [S12]

**Which plans have it**

- Enterprise Search and AI connectors need Business or Enterprise. The pricing page labels Enterprise Search as beta. [S11] [S12] [S1]
- The personal Gmail connector is free to connect on all plans. [S12]
- Setting one up needs a Notion workspace owner who is also an admin in the other app. [S12]
- The Outlook connector needs someone who is both a Microsoft 365 admin and a Notion workspace owner. [S13]

**What happens to your data**

- Notion only brings in content according to each app's permissions. [S12]
- Connectors generally reach content from one year before set-up, and new content can take up to 3 hours to appear. [S12]
- If you disconnect, the content becomes unsearchable and Notion deletes it within a day. [S12]
- The Outlook connector "can read all Microsoft Outlook emails associated with the connected account", but not attachments. [S13]

**In Australia**

- No country limits are stated. [S12]

## Outside AI that connects

Most outside assistants reach Notion through **Notion MCP**, Notion's hosted server at https://mcp.notion.com/mcp. [S24] Notion's help names Claude, ChatGPT and Cursor among the apps that use it. [S22]

Notion's warning: "MCP tools act with your full Notion permissions. They can access everything you can access." [S22]

On 19 October 2026 Notion said it had overhauled Notion MCP so outside agents can use Notion as shared memory. It also offers a setup prompt that saves your preferences to a private Memories database. [S62] [S22]

### Claude and Notion

**Official?**

- Yes. The **Notion connector** in Claude's directory is made by Notion, marked "Anthropic verified", and was added in November 2025. Its address is https://mcp.notion.com/mcp. [S38]
- Notion also runs **Claude agents in Notion**, where you work with Claude inside Notion. Notion added it as one of its first "External Agents" on 1 July 2026. [S20] [S31]
- Notion's Claude page says Claude agents are "Now available in public beta." [S21]
- Notion publishes a Notion plugin for Claude Code. Claude's marketplace now marks it "Anthropic verified". [S39]

**What it can see and do: the Notion connector**

- Claude's listing now shows 69 tools. Besides searching, reading and editing pages and databases, they cover comments, files, calendars, memories, Skills and handing work to Custom Agents. [S38]
- The list includes tools that move pages and databases to Trash and restore pages from Trash. [S38] [S59] [S60]
- Notion says the connector works with your full Notion permissions. [S22]
- On Business and Enterprise with Notion AI, an assistant connected through Notion MCP can also search your connected apps, such as Slack and Google Drive. Notion says that content goes to the assistant, under that app's own terms. [S22]

**What it can see and do: Claude agents in Notion (beta)**

- Claude agents chat with you and your team in Notion, work from shared docs and task boards, and create or update content if they have edit access. [S20]
- They "see only what you share with them". Their permissions are set per agent. [S20]
- They can't browse the web or call other agents. [S20]
- They're "hosted by Notion via Anthropic's infrastructure". You don't need an Anthropic account, and you can't use your own. [S20]

**What you need**

- Anthropic says directory connectors are available on Claude, Cowork, Claude Desktop and Claude mobile. On Team and Enterprise an owner turns a connector on first. [S40]
- Notion MCP "works on every plan", though some features vary. Workspace guests can't connect. [S24]
- Claude agents in Notion need a Notion Business or Enterprise plan and run on Notion credits. [S20]
- Claude agents are off by default for Enterprise and HIPAA workspaces. Notion says it's "rolling this out gradually". [S20]
- Plugins in Claude need a paid Claude plan. [S58]

**Steps to connect: the Notion connector** (Anthropic Help Center, "Updated today" when read on 18 November 2026)

1. In Claude, go to **Customize** > **Connectors** and click **+** next to **Connectors**. [S40]
2. Choose Notion, review it and click **Connect**. [S40]
3. Sign in to Notion and approve the access. [S40]
4. In a chat, click **+** (or type **/**), hover over **Connectors** and switch Notion on. [S40]

**Steps: Claude agents in Notion** (Notion Help Center)

1. In Notion, go to **Agents** in the sidebar > **New Agent** > **Claude**. [S20]
2. Start from a template or from scratch. Some templates connect to GitHub using your personal access token. [S20]
3. Share the agent only with the pages and databases it needs, then set its triggers. [S20]

On Enterprise, a workspace owner first turns Claude agents on under **Settings** > **Notion AI** > **Agent** > **Manage external agents**. [S20]

**For larger organisations**

- Notion Enterprise customers that sign in with Okta can set up an "enterprise-managed connection" for Claude, so "Members won't see a Notion approval screen." [S26]
- The Claude admin adds the Notion connector at https://mcp.notion.com/mcp and turns on "Enterprise managed authentication". [S26]
- Removing someone in Okta blocks new connections, but an active connection can last up to eight hours unless it's disconnected in Notion. [S26]
- There's now a second way, Claude auto-connect (beta), that works with any SAML single sign-on provider. The Claude admin goes to **Organization settings** > **Connectors** > **Notion** > **Managed authorization**, chooses **Claude-issued**, and a Notion owner clicks **Trust Claude**. [S26]
- Members can connect this way only if their email domain is verified by your Notion organisation and their Claude and Notion emails match. [S26]
- Notion says this route checks membership of your Claude organisation by email. It "doesn't check a sign-in at your identity provider or multi-factor authentication". [S26]

**To disconnect**

- In Claude, go to **Customize** > **Connectors**, select Notion and disconnect it. [S40]
- Workspace admins can switch Claude agents off under **Settings** > **Notion AI** > **Agents** > **Manage external agents**. [S20]

**Limits**

- Notion says its zero data retention commitments "don't extend to Claude agents in Notion". Anthropic stores session data between requests. [S20]
- Anthropic's listing says Anthropic "cannot verify that they will work as intended" for the tools developers provide. [S38]
- On Claude's Free, Pro and Max plans, raw content from connectors isn't used for training unless you copy it into the chat. [S41]
- On Claude's work plans, Anthropic doesn't train on your inputs or outputs by default. [S42]

### ChatGPT and Notion

**Official?**

- Yes. OpenAI's plugin directory lists **Notion** (version 3.0.9), described as "Create docs, tasks, databases", and it uses Notion's MCP server at https://mcp.notion.com/mcp. [S47]
- OpenAI's business page names Notion as the developer and now lists 12 Notion skills, such as **Meeting prep** and **Knowledge capture**. [S46] [S47]

**What it can see and do**

- "The Notion app lets ChatGPT search and read content from Notion pages that your connected account is allowed to access." [S43]
- OpenAI says ChatGPT "may be able to create or update Notion pages", depending on the plugin, your Notion permissions, workspace settings and approvals. [S43]
- OpenAI's examples include creating a roadmap database and filling it in from a list. [S46]
- OpenAI's listing now also names saving memories, managing your calendar and handing work to Notion Custom Agents among the plugin's capabilities. [S46] [S47]
- Notion no longer supports "individual sync". ChatGPT searches Notion directly, with no first sync to wait for. [S43]
- A ChatGPT workspace admin "cannot grant access to a Notion page that your Notion account is not allowed to view." [S43]

**What you need**

- OpenAI says availability depends on your ChatGPT plan, workspace settings and Notion permissions. [S43]
- In ChatGPT Business, many apps are on by default. Enterprise and Edu workspaces start with a selected set, and admins can change access. [S44]
- Notion guests can't connect through Notion MCP. [S24]

**Steps to connect** (OpenAI Help Center, "Updated: 26 days ago" when read; timestamp 23 October 2026, UTC)

1. Open **Settings** > **Plugins**. [S43]
2. Find and select **Notion**. [S43]
3. Select **Connect**. If Notion is listed as a plugin, select **Install plugin** and finish the connection prompt. [S43]
4. Sign in to the Notion account you want to use. [S43]
5. Review the Notion workspace and content in the request, then approve. [S43]

**To disconnect**

- Open **Settings** > **Plugins**, select Notion and use the disconnect option. [S43]
- If you use Notion through a plugin, open its settings and select **Disconnect** on an account's row to remove just that account. OpenAI warns that uninstalling the plugin can disconnect all your Notion accounts. [S43]

**The other way round: your ChatGPT plan inside Notion**

- If your Notion workspace is on Business or Enterprise and you have ChatGPT Plus, Pro, Business or Go, you can connect your ChatGPT account so GPT models in Notion Agent use your ChatGPT plan. [S28]
- It only applies when you pick a specific GPT model, and it doesn't work with Custom Agents. On Auto or a non-GPT model, it uses your Standard or Select credits instead. [S28]
- On ChatGPT Business, your ChatGPT admin decides whether Notion can use the plan and sets the limits. [S28]
- Notion says its own agreements with its AI sub-processors still apply, including no training. The conversations aren't saved to ChatGPT's history or memory. [S28]
- To connect: **Settings** > **Notion AI** > **Me**, then **Connect** next to ChatGPT under **Connected subscriptions**. [S28]
- To stop, go to **Settings** > **Notion AI** > **Usage** and turn off **Use your ChatGPT plan**, or select **Disconnect**. [S28]
- Notion announced this in Notion 3.8 on 13 October 2026. [S30]

**Limits**

- OpenAI says that on Free, Plus, Go and Pro, information from apps may be used for training if "Improve the model for everyone" is on. Business, Enterprise and Edu aren't used for training by default. [S44]
- OpenAI's listing says ChatGPT may share relevant chats and memories with the Notion app, and "Use of apps may come with elevated risk." [S47]

### Microsoft Copilot and Notion

**Official?**

- Yes, built by Microsoft. Microsoft's gallery lists **Notion**, published by Microsoft, to "Search your docs, wikis, notes, tasks, and databases." [S49]
- It's a "federated" connector, which means Copilot fetches Notion content live through MCP and doesn't copy it into Microsoft 365. [S48]

**What it can see and do**

- Copilot uses your own Notion sign-in and permissions, so you only see what your Notion account can see. [S48]
- It works in Microsoft 365 Copilot Chat, agents, Cowork, Copilot in Word, Excel, PowerPoint and Outlook, and the Researcher agent. [S48]
- Microsoft now says that where a connector provides the tools, Copilot can create, update or delete data with your approval. The Researcher agent stays read-only. [S48]
- Those actions need your approval, with the choices **Allow once**, **Allow for conversation**, **Always allow** and **Cancel**. [S48]
- Microsoft's pages don't say whether the Notion connector has write tools. Its gallery describes searching. [S49] [S48]
- You can check for yourself in Copilot under **Settings** > **Sources**. Select the connector, and its **Write/Delete tools** are listed apart from its **Read tools**. [S48]

**What you need**

- A Microsoft 365 Copilot licence. Microsoft says a user only sees a federated connector if "The user has a Microsoft 365 Copilot license." [S48]
- Microsoft-built connectors are available by default when an admin allows **Allow agents and plugins built by Microsoft** and includes the user. [S48]

**Steps to connect** (Microsoft Learn, 16 November 2026)

1. Open **Microsoft 365 Copilot Chat**. [S48]
2. Select the **...** menu, then **Settings**. [S48]
3. Select **Sources** in the left pane. [S48]
4. Find Notion, select **Connect** and sign in to Notion. [S48]
5. Ask your question in Copilot Chat. [S48]

**For admins**

- Manage the connector in the Microsoft 365 admin center under **Copilot connectors** > **Your connections**. You can switch it off or roll it out to chosen groups. [S48]
- **Agents** > **Settings** > **Agent and plugin access** allows or blocks connectors by who built them. **Agents** > **Settings** > **User access** sets the most people who can use any connector. [S48]

**To disconnect**

- Turn the source off in Researcher, or manage it in Copilot Chat settings. [S48]

**Limits**

- Microsoft says prompts, responses and Microsoft Graph data "aren't used to train foundation LLMs". It tells admins to check each agent's privacy statement and terms. [S50]
- Microsoft says customers outside the EU may have queries processed in the US, the EU or other regions. [S50]
- Microsoft's connector catalogue for Power Automate also has a "Notion (Independent Publisher)" connector. Microsoft lists two individuals as its publishers, and it signs in with an API key. We found nothing from Notion about it. [S51]

### Google Gemini and Notion

**Official?**

- No official connection found for the everyday Gemini app. Google's table of Connected Apps has no Notion entry. [S52]
- Google's separate business product, Gemini Enterprise, has a Notion connector that Google documents. [S54] [S53]
- Inside Notion, Notion AI can use Google's Gemini models. That's Notion choosing a model, which is different from the Gemini app connecting to Notion. [S4] [S11]

**What Gemini Enterprise's connector can see and do**

- Search Notion through "federated search", where your query goes to Notion live. Google's set-up page labels federated search as public preview. [S54] [S55]
- Actions to create comments, create and update databases, and create and update pages, plus "Additional read-only actions". [S54]
- Google warns that your query string is sent to the connected services, which "can link the query with your identity". [S54]
- The Notion data store "is supported only in Global, US, and EU locations." [S54]

**What you need**

- Gemini Enterprise, a Notion OAuth integration with its client ID and secret, and the Discovery Engine Editor role in Google Cloud. [S55]

**Steps to connect** (Google Cloud, last updated 10 November 2026)

1. In the Google Cloud console, open **Gemini Enterprise** and choose a project. [S55]
2. Click **Data stores**, then **Create data store**. [S55]
3. Search for "Notion" and click **Select** on the Notion card. [S55]
4. Set **Connector mode** to **Federated search** and click **Continue**. [S55]
5. Enter the **Client ID** and **Client Secret** from your Notion integration, click **Login**, then **Continue**. [S55]
6. Choose what to search, pick any Notion actions, set the location and name, and wait for the data store to show **Active**. [S55]

**Limits**

- Google's preview terms apply to federated search, which "might have limited support". [S55]

### Notion MCP (the developer route)

**Official?**

- Yes. Notion hosts its MCP server at https://mcp.notion.com/mcp. The older https://mcp.notion.com/sse address retires on 23 February 2027. [S24]
- Notion moved to a hosted server in 2025, after starting with a downloadable package in April 2025. [S35]
- Its open-source local server "is no longer actively maintained". [S24]

**What it can see and do**

- Notion now groups its MCP tools by job: search, pages, databases, files, comments, Skills and agents, and calendars. [S25]
- Search, read, create and update pages and databases, and add comments or suggest edits. [S23] [S60]
- Move pages to Trash and recover them from Trash. [S59] [S60]
- Hand tasks to Custom Agents and send them follow-up messages, if you have access to Custom Agents. [S61]
- Save and search private memories, on every plan, and use Skills shared across the workspace. [S61] [S23]
- Search connected apps such as Slack and Google Drive, on Business or Enterprise with Notion AI. [S24]
- Notion says everyday read and write actions through Notion MCP don't use credits. Running Notion Agent or a Custom Agent through a connected app does. [S64] [S7]

**What you need**

- Notion says MCP works on every plan, with some features varying by plan. [S24]
- MCP tokens are for Business and Enterprise workspace owners. Enterprise-managed sign-in needs Enterprise with SAML single sign-on. [S24]
- Searching connected apps through MCP needs Business or Enterprise with Notion AI. Plain Notion search works on every plan. [S24]

**Steps to connect** (Notion developer docs, no date shown)

1. Claude Code: run `claude mcp add --transport http notion https://mcp.notion.com/mcp`, then run `/mcp` in Claude Code and finish the sign-in. [S24]
2. Codex (ChatGPT): add the server address to `~/.codex/config.toml`, then run `codex mcp login notion`. [S24]
3. Other apps: add https://mcp.notion.com/mcp as a remote MCP server and complete the sign-in when prompted. [S24]

**For Enterprise admins**

- Admins can limit which AI apps members connect. Go to **Settings** > **Notion MCP** > **Manage workspace clients**, add apps with **Add approved MCP client**, then under **Which clients members can connect** choose **Approved MCP clients only**. [S22]
- Notion warns that unapproved apps stop working straight away, and asks you to confirm with **Switch anyway**. [S22]
- Under **All MCP clients**, admins can see which members connected each app. An app's ••• menu has **Disconnect all members**, and **View members** lets you disconnect one person. [S22]
- **Disconnect all users** disconnects every AI app connected through Notion MCP. People then have to sign in again. [S22]
- The **Open Notion pages in MCP clients** setting, on by default, lets apps such as ChatGPT open and edit Notion pages. Admins can turn it off. [S22]

**Limits**

- Notion suggests starting with "single-player use cases". [S22]
- OpenAI says full MCP in ChatGPT, including write actions, is for Business, Enterprise and Edu. Pro users can connect custom MCP servers that only read and fetch. [S45]

### Automation routes Notion documents

- Notion's webhook actions send data from buttons and database automations to tools like "Zapier, Make, and more". They're on paid plans. [S36]
- Enterprise owners can switch webhooks off under **Settings** > **Connections** with **Allow webhooks in automations**. [S36]
- Notion's connection gallery includes many apps that Notion doesn't make. Notion says: "Unless specifically designated as Made by Notion, connections are not supported or maintained by Notion." [S37]

## Jobs it's good for

- **Meeting notes that turn into tasks.** Record with AI Meeting Notes after everyone agrees, then let a Custom Agent file the action items. [S10] [S29]
- **A weekly project update.** Set a Custom Agent on a weekly schedule to pull from a project database and post a summary to a Slack channel. [S5]
- **Questions across the wiki and Slack.** Ask Enterprise Search, which cites the pages and messages it used. [S11]
- **New-starter questions.** Embed a Custom Agent in your onboarding page so people can ask it. Share only the pages it should use. [S5] [S56]
- **Finding a decision.** OpenAI's example asks ChatGPT to find the latest pricing decision for a project and summarise it with page links. [S46]
- **Keeping docs current.** Ask ChatGPT for a list of outdated pages to fix first, another of OpenAI's examples. [S46]
- **Working from Word or Outlook.** With the Notion connector switched on in Microsoft 365 Copilot, look up a Notion page without leaving the document. [S48]

## What to watch for

**Custom Agents can share what people can't otherwise see**

- A Custom Agent answers with its own access. Notion says people using it "can retrieve information from resources they lack access to". [S56]
- Give each agent only the pages it needs, and check its **Tools and access** before sharing it. [S56]
- Database row permissions don't protect you here: "if the agent can see more rows than the end user, the agent may expose information the end user can't access directly." [S56]

**Outside assistants act with your full access**

- Notion MCP works with everything the connected person can see and do in Notion. [S22]
- It can move pages to Trash. Deleted pages can be restored within 30 days. [S59] [S15]
- Write tools in Custom Agent MCP connections ask first by default, but **Always allow** removes the prompts for a whole server. [S57]
- The Notion MCP admin controls in Notion's help are for Enterprise. [S22] Notion's 3.8 release says admins can now allow only Notion-verified or chosen tools, without naming plans. [S30]
- When an assistant searches your connected apps through Notion MCP, that content goes to the assistant and its terms apply. [S22]

**Hidden instructions**

- Notion warns about prompt injection, where hidden text in a file or web page tries to steer the AI. [S19]
- Notion says smaller models "may be more vulnerable to prompt injection". It suggests a larger model for untrusted content. [S19]
- For agents connected to outside tools, Notion advises read-only access where possible, human confirmation for write tools and only trusted MCP servers. [S19]

**Training and who keeps what**

- Notion doesn't train on your data by default, and its providers keep data for up to 30 days on Free, Plus and Business. [S15]
- Claude agents in Notion aren't covered by zero data retention. [S20]
- When a Custom Agent uses Claude Fable 5, Anthropic may store prompts and responses for a time. [S5]
- Your chat history on the assistant's side follows that company's rules. [S44] [S41] [S42]

**Where your data goes**

- Notion's data regions are the US, Europe, Japan and Korea, for Enterprise only. Everyone else's data is hosted in the United States. [S17]
- Even with data residency, Notion says customer data can be processed outside the region by "Notion subprocessors, including LLM providers". [S17]
- Notion's AI model providers are listed as "Global", the USA or the UK. [S16]
- Microsoft says Copilot queries from outside the EU may be processed in the US, the EU or elsewhere. [S50]

**Costs**

- Picking a model yourself, or running your own Custom Agent, spends your Select credits. High credit consumption models and Claude agents spend Notion credits. [S64] [S8] [S20]
- When credits run out, Custom Agents pause until credits reset or are added. [S65]
- High credit consumption models are off until a workspace owner turns them on. [S8]
- Notion says an AI Command Center is "coming soon", with usage by person, feature and agent, and spending limits and alerts. [S62] [S63]

**Who can switch things on and off**

- Most AI settings sit under **Settings** > **Notion AI**: web search, model controls, usage limits, AI Meeting Notes and AI connectors. [S3]
- Who can create Custom Agents: the **Agents** tab under the same settings. [S56]
- Which outside AI apps can connect through Notion MCP: **Settings** > **Notion MCP** (Enterprise). [S22]
- Which MCP servers Notion Agent can use: **Settings** > **Connections**. [S27]
- We found no single switch that turns all of Notion AI off. [S3]

**Beta and preview**

- Claude agents in Notion, Enterprise Search, AI Meeting Notes, image generation and Workers are labelled beta. [S20] [S1] [S3]
- The Claude-issued enterprise-managed connection is in beta, and Bring Your Own Key is in private alpha for Enterprise. [S26] [S62]
- Notion says it "may update how you use Notion AI, including how Standard and Select credits work and the usage limits". [S9]

## Announced changes

- **13 May 2025:** Notion 2.51 brought AI Meeting Notes, Enterprise Search and Research Mode. Business and Enterprise plans "now include unlimited usage of Notion AI". [S32]
- **15 July 2025:** Notion described its new hosted MCP server, which replaced the downloadable package. [S35]
- **18 September 2025:** Notion 3.0 introduced Notion Agent. [S33]
- **24 February 2026:** Custom Agents launched, free until 3 May 2026. [S34]
- **4 May 2026:** Custom Agents started using Notion credits. [S34]
- **1 July 2026:** Notion 3.6 added Claude and Cursor as "External Agents". [S31]
- **31 July 2026:** AI Meeting Notes can trigger Custom Agents. [S29]
- **9 September 2026:** Owners can choose which AI models Notion Agent and Custom Agents use. [S29]
- **15 September 2026:** Notion 3.7 added shared skills for agents. [S29]
- **13 October 2026:** Notion 3.8 added ChatGPT plan support, more than 150 MCP connections and seven new models. Notion says admins can now see who connected each AI tool and revoke one person's access. [S30]
- **19 October 2026:** Notion rebuilt its agents and its Auto model router, overhauled Notion MCP and announced a new credit system. Bring Your Own Key went into private alpha for Enterprise. [S62] [S63]
- **31 October 2026:** Notion's deadline to move to its new SharePoint and OneDrive connector. Each person must connect their own Microsoft account. [S14]
- **2 November 2026:** Existing customers moved to the new Standard and Select credits. [S63]
- **By 16 November 2026:** Microsoft's page describes write actions through federated connectors as available, where a connector provides them. [S48]
- **1 December 2026:** AI Meeting Notes starts using Standard credits. [S64]
- **23 February 2027:** Notion's older SSE address for Notion MCP retires. [S24]
- **Coming soon, no date:** Notion's AI Command Center, and Skills through Notion MCP. [S62]

## What we couldn't establish

- **Prices in AUD and GST.** The pricing page shows US dollars only and doesn't mention tax. [S1]
- **The currency of Notion credits.** The credits page shows "$" without a currency. [S6]
- **A switch to turn off all of Notion AI.** We found switches for individual features only. [S3]
- **Whether Microsoft's Notion connector can make changes.** Microsoft's pages describe write actions for federated connectors in general but not for Notion. [S48] [S49]
- **Meeting notes on Free and Plus.** The pricing page's comparison table ticks meeting notes for every plan, while the meeting notes help says you need Business or Enterprise. [S1] [S10]
- **Custom Agents after a downgrade.** Notion's credit pages no longer say what happens to Custom Agents if a workspace moves to Free or Plus. [S7] [S65]
- **Notion's sub-processor list.** The page came back blank on 18 November 2026, so its row keeps the 17 October read date and the provider lines rest on that earlier read. [S16]
- **Claude agents in Australia.** Notion says it's rolling them out gradually and doesn't name countries. [S20]
- **A Notion app for the everyday Gemini app.** None found on Google's list. [S52]
- **Notion Mail's AI.** We didn't research Notion Mail or Notion Calendar's AI features in depth.
- **Dates on Notion's pages.** Notion's help pages and sub-processor list show no update dates. [S16]
- **Enterprise Search security.** Notion's "Enterprise Search security & privacy practices" address now opens its general security page. [S18]
- **Australian recording law.** Notion's AI Meeting Notes guidance doesn't cover Australian consent rules. [S10]

## Sources

Sources were read on 18 November 2026, except where a row shows an earlier date.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Notion Pricing Plans: Free, Plus, Business and Enterprise (as shown in Australia) | Notion | https://www.notion.com/en-gb/pricing | No date shown | 18 Nov 2026 |
| S2 | Meet your 24/7 AI team (Notion AI) | Notion | https://www.notion.com/product/ai | No date shown | 18 Nov 2026 |
| S3 | What is Notion AI? FAQs | Notion Help Center | https://www.notion.com/help/notion-ai-faqs | No date shown | 18 Nov 2026 |
| S4 | Notion Agent | Notion Help Center | https://www.notion.com/help/notion-agent | No date shown | 18 Nov 2026 |
| S5 | What are Custom Agents? | Notion Help Center | https://www.notion.com/help/custom-agents | No date shown | 18 Nov 2026 |
| S6 | What are Notion credits? | Notion Help Center | https://www.notion.com/help/what-are-notion-credits | No date shown | 18 Nov 2026 |
| S7 | Notion credits (help category and FAQs) | Notion Help Center | https://www.notion.com/help/category/notion-credits | No date shown | 18 Nov 2026 |
| S8 | Manage AI models & member credit spend | Notion Help Center | https://www.notion.com/help/manage-ai-models-and-member-credit-spend | No date shown | 18 Nov 2026 |
| S9 | Manage your AI credits (formerly "Manage your usage allowance for Notion AI") | Notion Help Center | https://www.notion.com/help/manage-your-ai-credits | No date shown | 18 Nov 2026 |
| S10 | Take AI Meeting Notes in Notion | Notion Help Center | https://www.notion.com/help/ai-meeting-notes | No date shown | 18 Nov 2026 |
| S11 | Enterprise Search | Notion Help Center | https://www.notion.com/help/enterprise-search | No date shown | 18 Nov 2026 |
| S12 | Notion AI Connectors overview | Notion Help Center | https://www.notion.com/help/notion-ai-connectors | No date shown | 18 Nov 2026 |
| S13 | Notion AI connector for Microsoft Outlook | Notion Help Center | https://www.notion.com/help/microsoft-outlook-ai-connector | No date shown | 18 Nov 2026 |
| S14 | Connect SharePoint and OneDrive to Notion Agents (replaces the legacy connector page) | Notion Help Center | https://www.notion.com/help/connect-sharepoint-and-onedrive-to-notion-agents | No date shown | 18 Nov 2026 |
| S15 | Notion AI security & privacy practices | Notion Help Center | https://www.notion.com/help/notion-ai-security-practices | No date shown | 18 Nov 2026 |
| S16 | Notion's List of Subprocessors | Notion | https://notion.notion.site/Notion-s-List-of-Subprocessors-268fa5bcfa0f46b6bc29436b21676734 | No date shown | 17 Oct 2026 |
| S17 | Data residency for Notion | Notion Help Center | https://www.notion.com/help/data-residency | No date shown | 18 Nov 2026 |
| S18 | Security @ Notion | Notion | https://www.notion.com/security | No date shown | 18 Nov 2026 |
| S19 | How Notion 3.0 protects against prompt injection risks | Notion Help Center | https://www.notion.com/help/how-notion-protects-against-prompt-injection-risks | No date shown | 18 Nov 2026 |
| S20 | Use Claude agents in Notion (beta) | Notion Help Center | https://www.notion.com/help/use-claude-agents-in-notion | No date shown | 18 Nov 2026 |
| S21 | Notion + Claude | Notion | https://www.notion.com/partners/claude | No date shown | 18 Nov 2026 |
| S22 | Connect AI tools with Notion MCP | Notion Help Center | https://www.notion.com/help/notion-mcp | No date shown | 18 Nov 2026 |
| S23 | Notion MCP | Notion Docs (developers) | https://developers.notion.com/guides/mcp/overview | No date shown | 18 Nov 2026 |
| S24 | Connect to Notion MCP | Notion Docs (developers) | https://developers.notion.com/guides/mcp/get-started-with-mcp | No date shown | 18 Nov 2026 |
| S25 | Supported tools (Notion MCP) | Notion Docs (developers) | https://developers.notion.com/guides/mcp/mcp-supported-tools | No date shown | 18 Nov 2026 |
| S26 | Set up enterprise-managed connections for Notion MCP | Notion Help Center | https://www.notion.com/help/set-up-enterprise-managed-connections-for-notion-mcp | No date shown | 18 Nov 2026 |
| S27 | Connect MCP servers to your Notion Agent | Notion Help Center | https://www.notion.com/help/connect-mcp-servers-to-your-notion-agent | No date shown | 18 Nov 2026 |
| S28 | Use your ChatGPT plan with Notion Agent | Notion Help Center | https://www.notion.com/help/use-your-chatgpt-plan-with-notion-agent | No date shown | 18 Nov 2026 |
| S29 | What's New (release notes) | Notion | https://www.notion.com/releases | Dated entries; latest 19 Oct 2026 | 18 Nov 2026 |
| S30 | Notion 3.8: Context for your agents | Notion | https://www.notion.com/releases/2026-10-13 | Oct 13, 2026 | 18 Nov 2026 |
| S31 | Notion 3.6: External Agents, HTML blocks, and more | Notion | https://www.notion.com/releases/2026-07-01 | Jul 1, 2026 | 18 Nov 2026 |
| S32 | Notion 2.51: AI Meeting Notes, Enterprise Search & more | Notion | https://www.notion.com/releases/2025-05-13 | May 13, 2025 | 18 Nov 2026 |
| S33 | Introducing Notion 3.0 | Notion Blog | https://www.notion.com/blog/introducing-notion-3-0 | Sep 18, 2025 | 18 Nov 2026 |
| S34 | Introducing Custom Agents | Notion Blog | https://www.notion.com/blog/introducing-custom-agents | Feb 24, 2026 | 18 Nov 2026 |
| S35 | Notion's hosted MCP server: an inside look | Notion Blog | https://www.notion.com/blog/notions-hosted-mcp-server-an-inside-look | Jul 15, 2025 | 18 Nov 2026 |
| S36 | Webhook actions in Notion automations | Notion Help Center | https://www.notion.com/help/webhook-actions | No date shown | 18 Nov 2026 |
| S37 | Context Link (Notion connection gallery listing) | Notion | https://www.notion.com/connections/ai-context-link | No date shown | 18 Nov 2026 |
| S38 | Notion connector | Anthropic | https://claude.com/marketplace/connectors/notion | "Added November 2025" | 18 Nov 2026 |
| S39 | Notion (plugin) | Anthropic | https://claude.com/marketplace/plugins/notion | No date shown | 18 Nov 2026 |
| S40 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (18 Nov 2026) | 18 Nov 2026 |
| S41 | Is my data used for model training? (consumer products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | Mar 16, 2026 | 18 Nov 2026 |
| S42 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | Aug 18, 2026 | 18 Nov 2026 |
| S43 | Notion app and setup in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12532955-notion-app-and-setup-in-chatgpt | "Updated: 26 days ago" (timestamp 23 Oct 2026, UTC) | 18 Nov 2026 |
| S44 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: yesterday" (timestamp 17 Nov 2026, UTC) | 18 Nov 2026 |
| S45 | Connecting custom MCP servers in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12584461-connecting-custom-mcp-servers-in-chatgpt | "Updated: 22 days ago" (timestamp 28 Oct 2026, UTC) | 18 Nov 2026 |
| S46 | Notion plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/notion/ | No date shown | 18 Nov 2026 |
| S47 | ChatGPT plugin listing: Notion | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69c18c28f1188191bf5b8445c4ab0a2e | Version 3.0.9; no date shown | 18 Nov 2026 |
| S48 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | 16 Nov 2026 (page metadata) | 18 Nov 2026 |
| S49 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 16 Nov 2026 (page metadata) | 18 Nov 2026 |
| S50 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/plan/microsoft-365-copilot-privacy | 9 Jul 2026 (page metadata; updated 4 Nov 2026) | 18 Nov 2026 |
| S51 | Notion (Independent Publisher) | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/notionip/ | 1 Mar 2024 (page metadata) | 18 Nov 2026 |
| S52 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 18 Nov 2026 |
| S53 | Connect your Google apps and third-party data (Gemini Enterprise, Business edition) | Google | https://support.google.com/g/answer/16550932?hl=en | Last updated Oct 15, 2026 | 18 Nov 2026 |
| S54 | Notion data store (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/notion | Last updated 2026-11-10 UTC | 18 Nov 2026 |
| S55 | Set up a Notion data store (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/notion/data-store | Last updated 2026-11-10 UTC | 18 Nov 2026 |
| S56 | Custom Agents sharing & permissions | Notion Help Center | https://www.notion.com/help/custom-agents-sharing-and-permissions | No date shown | 18 Nov 2026 |
| S57 | MCP connections for Custom Agents | Notion Help Center | https://www.notion.com/help/mcp-connections-for-custom-agents | No date shown | 18 Nov 2026 |
| S58 | Use plugins in Claude | Anthropic Help Center | https://support.claude.com/en/articles/13837440-use-plugins-in-claude | "Updated over 2 weeks ago" | 18 Nov 2026 |
| S59 | Create and organize pages (Notion MCP tools) | Notion Docs (developers) | https://developers.notion.com/guides/mcp/tools-pages | No date shown | 18 Nov 2026 |
| S60 | Work together in Notion (Notion MCP tools) | Notion Docs (developers) | https://developers.notion.com/guides/mcp/tools-comments | No date shown | 18 Nov 2026 |
| S61 | Reuse instructions and delegate work (Notion MCP tools) | Notion Docs (developers) | https://developers.notion.com/guides/mcp/tools-skills-agents | No date shown | 18 Nov 2026 |
| S62 | Agents, rebuilt to do more for less (release notes) | Notion | https://www.notion.com/releases/2026-10-19 | Oct 19, 2026 | 18 Nov 2026 |
| S63 | Agents, rebuilt to do more for less | Notion Blog | https://www.notion.com/blog/notion-ai-more-for-less | Published Oct 20, 2026 | 18 Nov 2026 |
| S64 | Standard, Select & Notion credits: eligible features | Notion Help Center | https://www.notion.com/help/standard-select-and-notion-credits-eligible-features | No date shown | 18 Nov 2026 |
| S65 | How AI credits work for Custom Agents | Notion Help Center | https://www.notion.com/help/how-ai-credits-work-for-custom-agents | No date shown | 18 Nov 2026 |
