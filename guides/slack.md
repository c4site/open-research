# Slack: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Slack's own AI is built into the app. It can summarise channels and take notes in huddles, which are Slack's audio and video calls. [S4] [S13]
- Slack's AI agent is Slackbot. It comes with Business+ and Enterprise+, while Free and Pro get a limited trial. On Business+ each person can send it 15 messages a week. [S1] [S7]
- Slack says the models behind its AI run inside its own cloud and that customer data is never used to train large language models. Slack also says Slackbot is "powered by Claude". [S19] [S18] [S11]
- Huddle notes come with every paid plan. Everyone in the huddle is told when notes start or stop, and AI notes can't be used when guests or external people are in the huddle. [S13]
- Slack's Australian pricing page shows US dollars, and Slack doesn't list the Australian dollar as a billing currency. [S1] [S2]
- Claude connects through a Slack-built connector that reads Slack and can send messages. Claude Tag, a beta for Claude Team and Enterprise, puts Claude to work inside your channels. [S35] [S38]
- ChatGPT connects through its Slack app, which searches Slack and can act once an admin allows it. Business, Enterprise and Edu workspaces can also set up @ChatGPT inside Slack. [S46] [S47]
- Microsoft hasn't built a Slack connector for Copilot. Its gallery lists two Slack connectors built by partners. [S55] [S56]
- The everyday Gemini app doesn't connect to Slack. Gemini Enterprise, Google's separate business product, has a Slack connector that can read and send messages. [S61] [S63]
- Salesforce's Agentforce agents also work inside Slack on any plan, if you hold Salesforce Agentforce licences. [S25]

## The tool, and the plans that matter

Slack is team chat software from Slack Technologies, a Salesforce company. Work happens in channels, direct messages (DMs) and huddles, which are audio and video meetings with screen sharing. [S1]

These are the plans on Slack's Australian pricing page as read from Perth on 17 October 2026. Prices are shown in US dollars, per user per month. [S1]

| Plan | Price a month (as shown, $US) | AI included | Worth knowing |
|---|---|---|---|
| Free | $US0 | Slackbot as a limited trial only | 90 days of message history. Huddles are one-to-one only. |
| Pro | $US8.75 paying monthly, or $US7.25 paying annually | Conversation summaries, huddle notes, automatic search filters and AI apps from other companies. Slackbot as a limited trial. | Unlimited message history and app integrations. |
| Business+ | $US18 paying monthly, or $US15 paying annually | Everything in Pro, plus Slackbot (15 messages a week each), AI search answers, recaps, file summaries, translations, AI workflow steps and canvas writing. | Data residency is available, including Sydney. |
| Enterprise+ | $US45 paying annually ("Contact sales") | Everything in Business+, plus enterprise search across other apps. No weekly Slackbot cap. | Restrict AI from reading chosen channels, canvases and lists. |

Sources for the table: [S1] [S5] [S7] [S16] [S22]

- The pricing page offers 50% off for three months on Pro and Business+ paid monthly. Slack's terms say you must buy online within seven days of creating the team, and Slack can end the offer at any time. [S1]
- Slack picks your billing currency from your location when the workspace is created. Its supported currencies are British pounds, euros, Indian rupees, Japanese yen and US dollars. [S2]
- None of the Slack pages we read say whether prices include GST. [S1] [S2]
- The separate Slack AI add-on can no longer be bought on Slack's website. Its features moved into the new Business+ and Enterprise+ plans. Existing add-on buyers keep it until their first renewal after 17 August 2025. [S3]
- Slack says turning AI features off doesn't lower the plan price. [S3]
- Slackbot use beyond plan limits can be paid for with Salesforce Flex Credits, which need a connected Salesforce organisation. The help article we read shows no credit prices. [S7]
- Slack's pricing FAQ says Salesforce customers on Free and Pro invoice subscriptions can get Slackbot, and Business+ invoice customers can buy Flex Credits for higher limits. [S1]
- Slack's App Directory lists more than 2,600 apps, including ChatGPT. [S1]

## AI built in

### Slackbot (Slack's personal AI agent)

**What it does**

- Slack calls Slackbot "your personal agent for work". It answers from the same information you can already see in Slack. [S6]
- It can summarise past conversations before a meeting, analyse a spreadsheet or draft a first version of a document. [S6]
- It can also draw on Salesforce, on third-party apps installed in your workspace and on enterprise search sources. [S6]
- Deep research produces a longer report from channels and files, the web, Salesforce data and connected MCP servers. It can take up to ten minutes. [S6]
- Scheduled tasks can send reminders or build meeting agendas. Each task can run at most three times a day. [S6] [S7]
- It can create and edit canvases. When it edits a shared canvas, you click **Confirm** before anything is added, or **Cancel**. [S6]
- Since April 2026 it can connect to Gmail, Google Calendar or Microsoft Outlook for calendar and email actions. [S12]
- Since May 2026 it can create or update Salesforce records and read, create and edit lists, with approval before changes. [S12]
- Since June 2026 it can connect to other apps that include an MCP server. Once a member connects their account, Slackbot can use all of that server's tools. [S12] [S28]
- Slack says Slackbot has "crossed one million monthly active users" and is "powered by Claude". [S11]

**Where to find it**

- On desktop, click **Slackbot** in the top right-hand corner of the screen or at the top of your sidebar. If you can't see it, click **More**. [S6]
- On mobile, go to the **Home** tab and tap **Slackbot** at the top of the screen. [S6]
- For recurring work, open the **Tasks** tab, click **Add task** and select **Create with Slackbot**. Slackbot drafts the task and you click **Create task**. [S6]
- For deep research, click the plus button next to the message field and select **Deep research**. [S6]

**Which plans have it**

- Ongoing access is on Business+ and Enterprise+. Free and Pro get a limited trial or preview. [S1] [S7]
- Business+ members can send 15 messages to Slackbot each week, resetting at midnight on Monday. Enterprise+ members have no weekly or lifetime cap. [S7]
- Slack says it may bring in usage limits or usage-based pricing for advanced capabilities released after June 2026, with 30 days' written notice. [S7]
- The new Slackbot became generally available for Business+ and Enterprise+ on 13 January 2026. [S10]

**What happens to your data**

- Slackbot's answers come only from what you can view in Slack. It can't see private channels or DMs you aren't part of. [S6]
- Slack says your interactions with Slackbot "remain private to you". [S9]
- Memory is on by default. Slackbot saves your preferences and the topics you work on from your Slack activity, and checks for new activity weekly. [S8]
- To turn memory off, open Slackbot, click the three dots icon, select **Manage memories** and switch off **Generate memory from conversations**. You can edit or remove saved items there too. [S8]
- Slack says dictated messages are transcribed but the audio isn't stored. [S6]
- Admins can decide whether Slackbot may create and edit canvases, use files in its answers or search the web. [S5]
- If web search is allowed, Salesforce's sub-processor list says SuSea, Inc. (trading as You.com) supplies the results and may pass public links and content into Slackbot's answers. [S23]

**In Australia**

- The Slackbot pages we read don't limit it by country. [S6] [S7]
- Salesforce's announcement of general availability didn't list regions or languages. [S10]

### Conversation summaries, recaps and file summaries

**What it does**

- Summarises a channel, DM or thread. You can choose unread messages, the last seven days or a custom date range, which works on desktop only. [S4]
- Recaps are daily summaries of the channels you choose. You can add, remove or mute channels. [S4]
- File summaries are made automatically for shared PDF, Word, PowerPoint and Excel files that everyone can access. [S4]

**Where to find it**

- To see new updates in a recap, select **Refresh recap** at the top of the recap. [S12]
- To translate a file summary, select **View summary** below the file, then click **Translate**. [S12]
- Each person can turn file summaries on or off in their own preferences. [S4]

**Which plans have it**

- Conversation summaries are on Pro, Business+ and Enterprise+. [S5]
- Recaps and file summaries need Business+ or Enterprise+. [S5]
- Older Business+ and Enterprise Grid subscriptions without the Slack AI add-on get only the Pro features. [S4]

**What happens to your data**

- Slack says summaries and search answers are "ephemeral" and aren't stored on devices or servers. [S18]
- "Recap data is stored for 90 days so that you can temporarily revisit past recap history." [S18]
- Channel summaries made by workflows are kept according to your organisation's data retention settings. [S18]

**In Australia**

- The pages we read don't limit these features by country. [S4] [S5]

### Huddle notes (AI notes and transcripts for Slack calls)

**What it does**

- When AI notes are on, Slack uses the live conversation and the messages in the huddle thread to capture key points and action items in a canvas. [S13]
- After the huddle, the notes are posted as a canvas in the huddle thread. They list the people in the huddle, topics discussed and action items. [S13]
- The transcript is embedded in the notes canvas. It doesn't show up in search results. [S13]

**Where to find it**

- On desktop, click **AI notes: Off** at the top left of the huddle, then **Start AI notes and transcription**, then **Start notes**. [S13]
- On mobile, tap the three dots icon at the bottom of the screen, then **Start AI notes**, then **Start notes**. A banner confirms notes are on. [S13]
- To pause on desktop, click **AI notes: On**, then **Stop AI notes**. To remove them, click **Delete AI notes and transcription**, then **Delete and cancel**. [S13]
- To start notes automatically in a channel, click the channel name, then **Settings**. Next to **Always start AI notes**, click **Edit**, tick the box and click **Save**. [S13]

**Which plans have it**

- All paid plans. Members can use it and guests can't. [S13] [S5]

**What happens to your data**

- "Everyone in the huddle will be notified when notes are started, stopped or cancelled." [S13]
- Anyone in a huddle can stop, resume or cancel AI notes at any time. [S13]
- Anyone in the channel or DM where the huddle took place can view the notes, and they can be shared like any canvas. [S13]
- AI notes can't be used in huddles with external people or guests. [S13]
- Admins can stop members changing the automatic huddle notes setting in channels. [S5]
- Canvases follow your workspace's data retention settings. On paid plans, Slack keeps data for the life of the workspace unless you set a shorter period. [S67]
- Salesforce's sub-processor list names Amazon Transcribe for huddle transcripts, with Australia among its listed locations. [S23]

**In Australia**

- The huddle notes article doesn't limit the feature by country. [S13]
- The sub-processor list doesn't say which location handles an Australian workspace's transcripts. [S23]

### Search answers and enterprise search

**What it does**

- Ask a question in your own words and get a short answer, with citations to the messages or files it used. [S14]
- Click **Share** to send an answer to a channel or DM. You review it before it's sent. [S14]
- Enterprise search adds content from other apps to search results, AI answers and Slackbot. Sources include Google Drive, Google Mail, OneDrive and SharePoint, Microsoft Outlook, Microsoft Teams, Box, Dropbox and Salesforce. [S15]

**Where to find it**

- Type a question in the Slack search bar. [S1]
- Org owners and admins turn on enterprise search: click your organisation name, then **Tools & settings**, then **Organisation settings**. Click **Settings**, select **Enterprise search**, click **Edit** and tick **Enable enterprise search for the entire organisation**. [S15]

**Which plans have it**

- Search answers need Business+ or Enterprise+. Pro gets automatic search filters. [S5] [S14]
- Enterprise search is on Enterprise+ only. [S15]

**What happens to your data**

- "AI search answers will only include results that you could also find in a standard search." [S19]
- Enterprise search results only include content the person searching can access in the other app. [S15]
- Enterprise search is off by default, but it may already be on if you use the Google Drive or OneDrive and SharePoint apps in Slack. [S15]
- Admins can stop files being used for answers and stop people sharing answers. [S5]
- Slack's privacy principles say admins can disable all file results, or results from externally hosted files. [S20]

**In Australia**

- The pages we read don't limit search answers by country. [S14] [S15]

### Translations, message explanations, canvas writing and workflows

**What it does**

- Translations turn messages into your chosen language. Only you see the translation. [S4]
- Message explanations explain acronyms, projects or jargon, drawing on your team's conversations. [S1]
- Canvas content generation uses AI to write or edit content in a canvas. [S4]
- AI workflow generation builds a Slack workflow from a single prompt. AI steps can add things like channel summaries to a workflow. [S1] [S4]

**Where to find it**

- AI steps are added inside Workflow Builder. The pages we read don't give menu paths for translations or explanations. [S1] [S4]

**Which plans have it**

- Business+ and Enterprise+. [S5]

**What happens to your data**

- Admins choose whether files and third-party connectors can be used in AI workflow steps. [S5]
- Slack's content safety filters cover canvas writing and workflow creation, as well as Slackbot and search. [S17]

**In Australia**

- The pages we read don't limit these features by country. [S4] [S5]

### Agentforce agents in Slack (from Salesforce)

**What it does**

- Agentforce agents are AI agents your company builds in Salesforce for a purpose such as IT help or benefits questions. They answer questions and complete tasks. [S26]
- Slack's templates include a Customer Insights Agent, an Employee Help Agent and an Onboarding Agent. [S25]

**Where to find it**

- On desktop, click **Tools** (or **More**), then **Agents**, and pick one under **Installed agents**. On mobile, tap **Agentforce**. [S26]
- To add one to a channel, click the channel name, open the **Agents & apps** tab and choose **Add Agentforce agent**. [S24]

**Which plans have it**

- "Available on all Slack subscriptions" with a Salesforce Agentforce licence. [S25] [S26]
- People in Slack who don't have a Salesforce account need a provisional Salesforce licence. [S25] [S27]
- Agents for Slack must be built with the Agentforce Employee Agent type. [S25]

**What happens to your data**

- Slack says agents use your Slack and Salesforce permissions and "will never reply with information that you don't have access to". [S26]
- Salesforce says "Your customer data is never used to train large language models" and that LLM providers don't have access to it. [S27]

**In Australia**

- The pages we read don't list regions. Salesforce's Australian Agentforce for Slack page shows no price and doesn't mention availability by market. [S25] [S27]

### Admin controls and the Slack AI guardrails

**What it does**

- Owners and admins can restrict each AI feature or turn it off entirely. [S5]
- Slack's AI guardrails add checks on top of the models' own safety. One reduces made-up answers. Another filters links to stop phishing, and another aims to reduce prompt injection, where hidden instructions try to steer the AI. [S17]
- A content safety filter has three levels. **Maximum** aims to block "targeted employee profiling such as performance and protected class information". **Default** targets prompt attacks and harmful content. **None** removes the extra filters. [S17]
- On Enterprise+, admins can stop AI from reading chosen channels, canvases and lists. This only limits what AI can read. Members can still use Slackbot to post to a restricted channel. [S16]

**Where to find it**

- Pro and Business+: click **Admin** in the sidebar, select **Workspace settings**, then **Roles & permissions**. Click **Feature access**, select **AI**, then click **Edit** next to a feature and choose **Everyone** or **No one**. [S5]
- Enterprise: click your organisation name, then **Tools & settings**, then **Organisation settings**. Click **Roles & permissions**, then **Feature access**, then **AI**. You can choose specific people and groups. [S5]
- The content safety filter sits on the same **AI** page, next to **Content safety filters**. [S17]
- To block new AI features by default, a primary owner opens **Future AI feature releases**, clicks **Edit** and unticks **Always allow access to new AI features**. [S5]
- To restrict a channel on Enterprise+, go to **Organisation settings**, click **Channels**, then **All channels**, then the three dots next to the channel, and select **Restrict AI use**. For a canvas or list, click **Share**, then **Advanced settings**, and untick **Allow AI use**. [S16]

**Which plans have it**

- AI feature controls apply on paid plans. [S5]
- The content safety filter can be changed by workspace owners and admins on Free, Pro and Business+, and by org owners and admins on Enterprise plans. [S17]
- Restricting AI access to channels, canvases and lists needs Enterprise+. [S16]

**What happens to your data**

- "Your customer data (like messages and files) is never used to train any LLMs." [S19]
- Slack says the large language models it uses are "deployed inside Slack's cloud environment, so model providers do not have access to your data". [S19]
- Slack's pricing FAQ says its models are "hosted directly within Slack's AWS virtual private cloud". [S1]
- Slack's privacy principles say it won't use customer data to train generative AI models "unless Customer provides affirmative opt-in consent". [S20]
- Slack's other machine learning models, which aren't generative, do analyse customer data. You can opt out by emailing feedback@slack.com with the subject "Slack global model opt-out request". [S20]
- Slack's blog says AI answers use the requesting person's access rights, and that summaries and search answers aren't stored on disk. [S21]
- Members' feedback on AI responses is blocked by default in some workspaces. Owners and admins can allow it. [S5]
- Salesforce's sub-processor list for Slack names Google LLC and Microsoft (Azure) as providers of "generative artificial intelligence services", both in the United States. [S23]

**In Australia**

- Data residency in Sydney, backed up in Melbourne, covers messages, canvases, files, the search index and bot-generated messages. It needs Business+ or Enterprise, and only the primary owner can turn it on. [S22]
- Member profiles, membership information and some analytics data can be stored outside your chosen region. Flagged content may be stored in the United States. [S22]
- Without data residency, Slack says your data is stored in the US. [S22]
- The data residency article doesn't mention the AI features. [S22]

## Outside AI that connects

A quick translation of the jargon. **MCP** (Model Context Protocol) is a standard way for an AI assistant to use another app's tools. Slack runs its own MCP server, and several AI assistants plug into it. [S30]

Connections run in two directions. An outside AI can read Slack from its own app, or the AI can have its own app inside Slack that people talk to. [S47] [S39]

### Claude and Slack

**Official?**

- Yes. The "Slack" connector in Claude's directory is made by Slack, marked "Anthropic verified", and was added in November 2025. [S35]
- Claude Tag puts Claude inside your Slack channels for teams. It's a beta, and the earlier Claude in Slack app switched over to it on 3 August 2026. [S38] [S39]
- Slack lists Claude.ai and Claude Code among the partner apps for its MCP server. [S30]

**What it can see and do**

- The Slack connector can search public and private channels, read channels and threads, look up people and read canvases. [S35]
- It can also send messages and create or update canvases. [S35]
- Claude can ask for your approval before using a tool. You can set each tool to **Always allow**, **Needs approval** or **Blocked**. [S45]
- Anthropic says Claude only searches the Slack channels you have access to. [S37]
- With Claude Tag, anyone in a channel can tag @Claude and hand it work. It posts a checklist in the thread as it goes, and the whole exchange stays visible to the channel. [S39]
- By default, Claude Tag can read and post in channels it's been added to and search public channels by keyword. It can't reach your other systems until an Owner adds connectors. [S41]
- In channels, Claude Tag acts under its own service accounts. Whatever a connected account can read or write is available to everyone in those channels. [S41]
- Claude Tag can also run scheduled jobs and watch channels. [S39]

**What you need**

- For the connector, a Claude account. Anthropic's Slack page says Team and Enterprise, and its blog says Pro and Max were added on 26 January 2026. [S36] [S37]
- Slack's developer docs say your Slack workspace admin must approve the MCP integration. [S31]
- On Team and Enterprise, an Owner adds the connector for the organisation first. Each person then signs in with their own account. [S44]
- Slack Enterprise+ organisations on Claude Team or Enterprise can manage access through Okta. Slack says Okta is currently the only identity provider supported for this. [S32]
- For Claude Tag, a Claude Team or Enterprise plan, an Owner to run setup and a Slack workspace admin to install the app and run the pairing command. [S40]
- Claude Tag isn't available on Free, Pro or Max plans. It also isn't available to organisations with Zero Data Retention. [S39] [S40]
- Claude Tag adds no per-seat charge. Channel work draws on a usage balance, up to a monthly spend limit an Owner sets. On Team plans nothing runs until credits are loaded. [S39] [S40]

**Steps to connect** (Anthropic's docs, not dated)

1. In Claude, go to **Customize > Connectors** and select **Discover**. [S45]
2. Search for Slack, open it and select **Connect to Claude**. On Team or Enterprise, an Owner sees **Connect for your team**. [S45]
3. Sign in to your Slack workspace, review the access Claude asks for and approve it. [S45] [S31]
4. Back in Claude, Slack shows under **Your connectors** as **Connected**. [S45]
5. In a chat, select **+**, then **Connectors**, and switch Slack on. [S45]
6. Ask something like "What did the team decide about the launch date in #product-planning last week?" [S36]

Claude Tag setup, for a Claude Owner working with a Slack admin (Anthropic's docs, not dated):

1. Go to claude.ai/admin-settings/claude-tag and click **Start setup**. [S40]
2. Click **Add the Claude app**, then **Add to Slack**, and approve the permissions. [S40]
3. In Slack, a workspace admin runs `/invite @Claude` in a channel, then sends `@Claude connect`. Claude replies with a pairing code that only they can see. It expires after 15 minutes. [S40]
4. Paste the code into **Paste the pairing code** and click **Pair workspace**. [S40]
5. Set a monthly spend limit, choose at least one public channel and click **Launch Claude Tag**. [S40]
6. Test it by tagging Claude in that channel and asking it to summarise what the channel decided this week. [S40]

**To disconnect**

- Connector: go to **Customize > Connectors**, select Slack and select **Disconnect**. [S45] [S36]
- Claude Tag: an Owner can switch off **Enable Claude Tag in Slack**. That keeps Claude's data. [S40] [S42]
- Disconnecting the workspace under **Connected workspaces** permanently deletes that workspace's Claude data. A Slack admin uninstalling the Claude app does the same. [S40] [S42]

**Limits**

- Anthropic's listing warns: "Only use connectors from developers you trust." [S35]
- During the beta, Claude Tag has no automatic retention period. Transcripts and memory are kept until the workspace is disconnected or the app is uninstalled. [S42]
- Editing or deleting a message in Slack doesn't remove it from a Claude Tag transcript that already includes it. Messages from guests become part of the transcript as well. [S42]
- Your organisation's custom data retention setting doesn't apply to Claude Tag transcripts or memory. [S42]
- In a channel shared with another company through Slack Connect, Claude Tag can use that channel's connectors for the other company's people too. [S41]
- Notes Claude Tag saves from a public channel are read by sessions in every channel of the workspace. [S41]
- With the earlier Claude in Slack app, conversations stayed out of your claude.ai history and were deleted within 30 days of disconnecting. [S36]
- Anthropic's landing page says Claude gets "its own account in your systems, not a borrowed login", and that every credential's use is logged. [S43]

### ChatGPT and Slack

**Official?**

- Yes, two ways. The Slack app in ChatGPT, now listed as the "Slack" plugin, lets ChatGPT search Slack and take some actions there. [S46] [S52]
- @ChatGPT is an assistant your ChatGPT admin sets up inside Slack. It replaces the older ChatGPT app in Slack's sidebar. [S47]
- OpenAI's business page names OpenAI as the plugin's developer, while the ChatGPT directory names Slack. [S51] [S52]

**What it can see and do**

- The Slack app searches messages, threads and channels you can already access, including DMs. It can summarise discussions and build recaps or briefs. [S46]
- Keyword search works on every Slack plan. Search by meaning needs Business+ or Enterprise+ with Slack's AI search turned on. [S46]
- Where an admin enables them, it can take Slack actions for you, such as joining a channel, creating a reminder, uploading a file or updating your profile. [S46]
- The permissions it requests include writing messages and writing canvases. [S46]
- Your ChatGPT permission setting decides when it asks first. **Allow read actions** reads without asking but asks before making changes. [S53]
- OpenAI lists sending a message as the kind of action that may need extra review. [S53]
- @ChatGPT answers people who mention it in a channel or DM. It runs on a service account with company connections an admin sets up, and doesn't inherit each person's access. [S48] [S49]
- ChatGPT team tasks can watch a Slack channel and start when a new message arrives, or post a weekly project update to an approved channel. [S50] [S46]

**What you need**

- For the Slack app, a paid ChatGPT plan: Plus, Pro, Business, Enterprise or Edu. You don't need a paid Slack plan. [S46]
- In Business workspaces the Slack app is on by default. In Enterprise and Edu it must be enabled for your workspace. [S46]
- If your Slack requires admin approval for app permissions, a Slack admin may need to approve or reinstall the ChatGPT app. [S46]
- For @ChatGPT, a ChatGPT Business, Enterprise or Edu workspace with credits. A ChatGPT workspace admin sets it up and a Slack admin approves the app. [S49]

**Steps to connect** (OpenAI's help centre, updated 11 October 2026)

1. In ChatGPT, open **Settings** and find Slack under **Apps** or **Plugins**. [S46]
2. Select **Connect**. [S46]
3. Sign in to the Slack workspace you want and approve access. ChatGPT connects to one Slack workspace at a time. [S46]
4. In a chat, mention Slack with **@** or pick it from the **+** menu. ChatGPT can also use Slack automatically when it's relevant. [S54] [S46]

@ChatGPT setup, for admins (OpenAI's help centre, updated 17 October 2026):

1. In the OpenAI admin console, select the ChatGPT workspace. [S49]
2. Open **Agents**, select **@ChatGPT agents**, select **Add** and choose **Slack**. [S49]
3. Connect the Slack workspace and review the permissions. A Slack owner or app manager approves the app if required. [S49]
4. In **New agent**, choose the Slack workspace, give it a name and select **Create agent**. [S49]
5. To limit channels, open the agent, select **Selected channels only**, add channels and select **Save channel restrictions**. [S49]
6. Add @ChatGPT to a test channel, mention it in a new thread, then test a DM separately. [S49]

**To disconnect**

- Slack app: open **Settings > Plugins**, select the app, then **Disconnect**. [S54]
- Disconnecting stops future access but doesn't delete past chats, saved files or memories. [S54]
- @ChatGPT: in the agent's **Overview**, turn off @ChatGPT to pause it, or select **Delete**. Deleting removes its settings and service account but leaves the Slack app installed. [S49]

**Limits**

- When connected, ChatGPT may share relevant chats and memories with the Slack app. Slack's terms and privacy policy then apply. [S52]
- OpenAI says information sent to Slack follows Slack's own storage, retention, privacy and data-residency terms. [S46]
- Channel restrictions for @ChatGPT don't restrict DMs. [S49]
- @ChatGPT doesn't respond to Slack guests and isn't supported in Slack Connect channels. [S48]
- In Slack, **Allow for a week** remembers the access level you approved for seven days. [S48]
- Replies from @ChatGPT in shared conversations are visible to everyone in them. [S47]
- At launch, @ChatGPT doesn't record or use memory. [S48]
- Heavy use with deep research or agent mode can use up your own Slack API quota. [S46]

### Microsoft Copilot and Slack

**Official?**

- No connection built by Microsoft or Slack found. Microsoft's own gallery of Copilot connectors has no Slack entry, and neither does its list of federated (live) connectors. [S55] [S57]
- Microsoft's partner gallery lists two Slack connectors built and supported by partners: one from RheinInsights and a "Slack external content connector" from ServiceNow. [S56]

**What it can see and do**

- RheinInsights' connector indexes public and private channels, messages, threads and attached files, following Slack's permission model. [S56]
- ServiceNow's connector indexes messages, threads and shared files from all public channels. [S56]
- Indexing connectors copy content into your Microsoft 365 search index so Copilot can use it. Copilot Chat can't write back to the other app by default. [S60]
- For builders, Microsoft publishes a Slack connector for Copilot Studio and Power Automate. Its actions include posting a message and listing the messages in a conversation. [S58]
- A Copilot Studio agent can be placed in Slack through Azure Bot Service. Microsoft says this needs considerable developer expertise. [S59]

**What you need**

- A Microsoft 365 admin sets up indexing connectors in the Microsoft 365 admin center. [S60]
- Microsoft says partner connectors are supported by the partner, and support models vary. [S56]
- Microsoft's Slack connector is a Standard connector in Copilot Studio and Power Automate. [S58]

**Steps to connect**

- Not documented on the Microsoft pages we read. The partner gallery links to each partner's own setup guide. [S56]

**To disconnect**

- Not covered for these partner connectors. Microsoft says that when a user disconnects or an admin disables a self-serve synced connector, its indexed content is removed. [S60]

**Limits**

- These are partner products. We didn't review the partners' own pages. [S56]
- Microsoft's Slack connector limits each connection to 100 calls a minute. [S58]

### Google Gemini and Slack

**Official?**

- Not in the everyday Gemini app. Google's lists of connected apps for personal accounts and for work or school accounts don't include Slack. [S61] [S62]
- Yes in Gemini Enterprise, Google's separate business product. Its Slack data store became generally available on 27 May 2026. [S65] [S66]
- Google also offers the Gemini Enterprise app for Slack, which answers questions inside Slack. It became generally available on 17 June 2026. [S64] [S65]

**What it can see and do**

- The connector lets Gemini Enterprise search and read Slack conversations, files and messages in plain language. [S63]
- It can send or schedule a Slack message, send a message draft and create a Slack canvas. [S63] [S66]
- The Gemini Enterprise app for Slack answers in DMs and when it's mentioned in a channel. Channel replies are shown privately to you first. [S64] [S65]
- Google warns that with federated search, "your query string is sent to all enabled third-party search backends". [S63]

**What you need**

- A Gemini Enterprise subscription. Google's Slack pages cover the Standard, Plus, Pay-as-you-go and Frontline editions, and point Business edition customers to a separate help centre. [S63]
- For the Slack app, Google lists "Access to the Slack AI add-on" as a prerequisite. [S64]
- A Google Cloud admin creates OAuth credentials, and each person grants one-time access. [S64]

**Steps to connect** (Google Cloud docs, last updated 14 October 2026)

1. In Google Cloud, go to **APIs & Services > Credentials** and create an OAuth client ID for a web application. [S64]
2. In Gemini Enterprise, open the app and go to **Integration > Slack**. Enter the Slack workspace ID, client ID and client secret, then click **Save**. [S64]
3. Install the app in Slack and click **Allow**. A Slack owner or admin can check it under **Manage > Installed Apps**. [S64]
4. Each person grants one-time access so Gemini Enterprise can search their data. [S64]

**To disconnect**

- Not described on the pages we read. [S63] [S64]

**Limits**

- Slack data stores can only be placed in Google's global, US or EU locations. [S63]
- Each Gemini Enterprise app links to one Slack workspace. [S64]
- Google says Slack allows about 10 requests a minute for the connector. [S63]
- Chat histories aren't synced between Slack and Gemini Enterprise. [S64]

### Slack's MCP server (the route most AI assistants use)

**Official?**

- Yes. Slack's MCP server and its Real-Time Search API became generally available on 17 February 2026. [S33]
- Slack names Claude.ai, Claude Code, Perplexity and Cursor as partner apps that need no coding. [S30]
- Slack's help centre also lists ChatGPT among the outside AI tools that use it. [S29]

**What it can see and do**

- Search messages, files, people and channels, and read channels and threads. [S30]
- Send, schedule or draft messages, and add reactions. [S30]
- Create, update and read canvases and lists, and upload files. [S30] [S12]
- Slack says agents with access can "take actions in Slack on your behalf". It doesn't describe a confirmation step on Slack's side. [S29]

**What you need**

- An app that is published in Slack's directory or built internally. Workspace admins approve and manage these integrations. [S30]
- On Enterprise Grid and Enterprise+, admins can grant MCP access to specific people and groups. [S12]

**Steps to connect**

- Through each AI's own connector, such as Claude's Slack connector above. [S31]

**To disconnect**

- Not described on the developer pages we read. Slack says MCP activity can be checked in audit logs. [S30]

**Limits**

- Each tool has its own rate limit, in tiers of 20, 50 or 100 or more calls a minute. [S30]
- Slack says the Real-Time Search API lets apps retrieve only what they need "without storing customer data on external servers". [S33]
- Slack says the server "respects user permissions". [S33]

### AI apps and automation inside Slack

**Official?**

- Yes. Slack lets you install apps with AI agents or assistants from its Marketplace, under the **Agents & tools** tab. [S24]

**What it can see and do**

- An app can read your messages with it. Adding it to a channel or DM gives it access to that conversation too. [S24]
- Slack says Marketplace apps must follow a "zero-copy and zero LLM training policy", and that no customer data is used or retained to train third-party LLMs. [S24]
- Workflow Builder has connectors to other services, including Google, Microsoft and Zoom. [S34]

**What you need**

- AI apps work on all plans, but guests can't use them. [S24]
- By default members can install apps with agents. Owners and admins can turn on app approval so apps are reviewed first. [S24]
- Workflow Builder connectors need approval before they appear if your workspace requires app approval. [S34]

**Steps to connect**

1. Click **Agents & tools**, then **AgentExchange**, and search for an app. [S24]
2. Click **Add to Slack**, then **Allow**. If you need permission, add a note for your admin and click **Submit request**. [S24]

**To disconnect**

- Not covered in the article we read. [S24]

**Limits**

- Slack warns: "Because agents use AI, they can be wrong." [S24]

## Jobs it's good for

- **Catching up after leave.** Summarise a busy channel for the last seven days, or set up daily recaps on Business+. [S4]
- **Meeting notes without a note-taker.** Turn on huddle notes and share the canvas afterwards. Tell people first. [S13]
- **Finding a decision.** Ask the question in search, then open the cited messages to check the answer. [S14]
- **Preparing for a client meeting.** Ask Slackbot to summarise recent discussions and draft an agenda. [S6]
- **A weekly status update.** ChatGPT team tasks can post a weekly project update to an approved Slack channel. [S50]
- **Pulling Slack into a document.** Claude or ChatGPT can search a channel and turn the discussion into a brief. [S36] [S46]
- **A shared helper in one channel.** Claude Tag can turn a settled discussion into a decision document or tickets. [S39]
- **Messages in another language.** Business+ translations show a message in your language, and only you see it. [S4]

## What to watch for

**Notes and transcripts are records**

- Huddle notes include a transcript, and anyone in the channel or DM can open it. [S13]
- Slack tells everyone in the huddle when notes start. People who join the channel later can still read old notes. That's our reading of who can view them. [S13]
- Claude Tag keeps the original text of messages even after they're edited or deleted in Slack. [S42]

**Shared accounts reach further than people**

- Slack's own AI and Agentforce answer from what each person can already see. [S6] [S26]
- Claude Tag and @ChatGPT work through service accounts. Whatever those accounts can reach is open to everyone who can talk to them in a channel. [S41] [S49]

**Actions as well as answers**

- Slack's MCP server, Claude's Slack connector and ChatGPT's Slack app can all send messages. [S30] [S35] [S46]
- Our suggestion: in Claude, set send tools to **Needs approval**. In ChatGPT, keep the permission on **Always ask** or **Allow read actions**. [S45] [S53]

**Training and where data goes**

- Slack says customer data isn't used to train LLMs and its models run inside its own cloud. [S19] [S1]
- Slack's other machine learning analyses customer data unless you opt out by email. [S20]
- Salesforce's sub-processor list names Google and Microsoft (Azure) as generative AI providers for Slack, located in the United States. [S23]
- Sydney data residency covers messages and files, but some data, like member profiles, can be stored elsewhere. [S22]
- When ChatGPT uses the Slack app, it may share relevant chats and memories with Slack, under Slack's terms. [S52]
- Google warns that Gemini Enterprise's federated search sends your query to every enabled third-party search backend. [S63]

**Costs**

- Slackbot on Business+ is capped at 15 messages a week per person. [S7]
- Claude Tag and @ChatGPT bill by usage. Set a spend limit before you launch. [S39] [S49]
- Turning AI features off doesn't reduce your Slack bill. [S3]

**Who switches things on**

- New AI features turn on automatically unless a primary owner unticks **Always allow access to new AI features**. New Slackbot features always roll out if Slackbot is on. [S5]
- Members can install AI apps unless app approval is on. [S24]
- Claude's Team and Enterprise Owners add connectors and set tool permissions. Members can't override them. [S44]
- In ChatGPT Business, the Slack app is on by default. [S46]

**Guests and other companies**

- Guests can't use AI apps or huddle notes. [S24] [S13]
- @ChatGPT doesn't answer guests or work in Slack Connect channels. Claude Tag can work in Slack Connect channels if an admin turns it on there. [S48] [S41]

**Beta labels**

- Claude Tag is a public beta, and Anthropic says its features may change before general release. [S39] [S41]

## Announced changes

- **1 October 2025:** Anthropic launched Claude in Slack and the Slack connector for Claude. [S37]
- **13 January 2026:** Slackbot became generally available for Business+ and Enterprise+, rolling out through January and February. [S10]
- **26 January 2026:** Anthropic made the Slack connector available to Claude Pro and Max subscribers. [S37]
- **17 February 2026:** Slack's MCP server and Real-Time Search API became generally available. [S33]
- **April to August 2026:** Slackbot gained skills, scheduled tasks, web search, Salesforce record updates, memory, an MCP client, deep research and a full-screen "big mode". [S12]
- **May 2026:** Slack's "Today" landing page opened as an open beta. [S12]
- **27 May 2026:** Google's Slack data store for Gemini Enterprise became generally available. [S65]
- **17 June 2026:** The Gemini Enterprise app for Slack became generally available. Channel mentions followed on 10 September 2026. [S65]
- **3 August 2026:** Claude in Slack switched over to Claude Tag. [S38]
- **15 September 2026 (Dreamforce):** Slack said Slackbot in channels is in early pilot, with two-way voice and video generation "coming later this year". [S11]
- **October 2026:** Workflows can start a conversation with Slackbot or an agent. [S12]
- **Coming soon, no date:** Slack's pricing FAQ says Salesforce CRM customers who connect to Slack will get ongoing Slackbot access. [S1]
- **After June 2026:** Slack says advanced Slackbot features may get usage limits or usage-based pricing, with 30 days' notice. [S7]
- **Microsoft:** write actions through Copilot connectors start "early October 2026". [S60]
- **OpenAI:** @ChatGPT replaces the older ChatGPT app in Slack. Existing installations don't stop immediately. [S47]

## What we couldn't establish

- **Australian prices.** Slack's Australian page shows US dollars, and Slack's billing currencies don't include AUD. No page we read said whether GST is included. [S1] [S2]
- **Free and Pro AI on the pricing cards.** The plan cards list AI items under Free and Pro without saying which are included. We relied on the help centre's table, which puts search answers, recaps and file summaries on Business+ and up. [S1] [S5]
- **Which Claude plans get the Slack connector.** Anthropic's Slack page says Team and Enterprise and that the Claude in Slack app must be installed first. Its blog says Pro and Max were added in January 2026. Neither mentions Free. [S36] [S37]
- **Who built ChatGPT's Slack plugin.** OpenAI's business page says OpenAI and the ChatGPT directory says Slack. [S51] [S52]
- **Which models Slack uses.** Slack says Slackbot is powered by Claude and that its models run in its own AWS cloud. Salesforce's sub-processor list names Google and Microsoft Azure for generative AI and doesn't name Anthropic. We couldn't match features to providers. [S11] [S1] [S23]
- **Where Slack's AI runs for Australian workspaces.** The data residency article doesn't mention AI features, and we found no page saying AI processing stays in Australia. [S22] [S18]
- **How long huddle transcripts are kept.** The huddle notes article doesn't say. Canvases follow workspace retention, but no page we read says the embedded transcript does too. [S13] [S67]
- **Whether "Restrict AI use" covers outside AI.** The article doesn't say whether it applies to third-party AI apps or the MCP server. [S16]
- **Agentforce in Australia.** No page we read gave regions, languages or prices for Agentforce in Slack. Salesforce's help pages need JavaScript and wouldn't load for us. [S25] [S27]
- **Which Slack plans can use the MCP server.** Slack's developer page doesn't say. [S30]
- **Gemini Enterprise Business edition.** Google's Slack pages cover the other editions and send Business customers elsewhere. We didn't read that help centre. [S63]
- **Microsoft's partner connectors.** We didn't read RheinInsights' or ServiceNow's own pages, because they're third parties. [S56]
- **Dates on Slack's help centre.** Slack's help articles show no published or updated dates. [S4]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Slack pricing for subscriptions (Australia) | Slack | https://slack.com/intl/en-au/pricing | No date shown (©2026). Read from Perth in a browser, prices shown in $US | 17 Oct 2026 |
| S2 | Supported billing currencies | Slack Help Centre | https://slack.com/help/articles/115004062808-Supported-billing-currencies | No date shown | 17 Oct 2026 |
| S3 | Updates to feature availability and pricing for Slack plans | Slack Help Centre | https://slack.com/help/articles/39264531104275-Updates-to-feature-availability-and-pricing-for-Slack-plans | No date shown | 17 Oct 2026 |
| S4 | Guide to AI features in Slack | Slack Help Centre | https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack | No date shown | 17 Oct 2026 |
| S5 | Manage access to AI features in Slack | Slack Help Centre | https://slack.com/help/articles/28244420881555-Manage-access-to-AI-features-in-Slack | No date shown | 17 Oct 2026 |
| S6 | How to work with Slackbot | Slack Help Centre | https://slack.com/help/articles/202026038-How-to-work-with-Slackbot | No date shown | 17 Oct 2026 |
| S7 | Slackbot limits and credit usage | Slack Help Centre | https://slack.com/help/articles/53579676130195-Slackbot-limits-and-credit-usage | No date shown | 17 Oct 2026 |
| S8 | Build your Slackbot memory | Slack Help Centre | https://slack.com/help/articles/52916888307091-Build-your-Slackbot-memory | No date shown | 17 Oct 2026 |
| S9 | Introducing Slackbot, your context-aware AI agent for work | Slack blog | https://slack.com/blog/news/slackbot-context-aware-ai-agent-for-work | 13 Mar 2026 (the text describes a January and February rollout) | 17 Oct 2026 |
| S10 | Salesforce Announces the General Availability of Slackbot | Salesforce (press release) | https://www.salesforce.com/news/press-releases/2026/01/13/slackbot-announcement/ | 13 Jan 2026 | 17 Oct 2026 |
| S11 | Slack's newest innovations turn AI into a true teammate (Dreamforce 2026) | Slack blog | https://slack.com/blog/news/ai-powered-interface-for-work | 15 Sep 2026 | 17 Oct 2026 |
| S12 | Slack updates and changes | Slack Help Centre | https://slack.com/help/articles/115004846068-Slack-updates-and-changes | Monthly entries, latest October 2026 | 17 Oct 2026 |
| S13 | Use AI to take huddle notes in Slack | Slack Help Centre | https://slack.com/help/articles/31377193680019-Use-AI-to-take-huddle-notes-in-Slack | No date shown | 17 Oct 2026 |
| S14 | Search with AI in Slack | Slack Help Centre | https://slack.com/help/articles/31739993134867-Search-with-AI-in-Slack | No date shown | 17 Oct 2026 |
| S15 | Set up and manage Slack enterprise search | Slack Help Centre | https://slack.com/help/articles/39044407124755-Set-up-and-manage-Slack-enterprise-search | No date shown | 17 Oct 2026 |
| S16 | Restrict AI access to certain channels, canvases and lists | Slack Help Centre | https://slack.com/help/articles/47421816860947-Restrict-AI-access-to-certain-channels-canvases-and-lists | No date shown | 17 Oct 2026 |
| S17 | Guide to the Slack AI Guardrails | Slack Help Centre | https://slack.com/help/articles/53359847722131-Guide-to-the-Slack-AI-Guardrails | No date shown | 17 Oct 2026 |
| S18 | Security for AI features in Slack | Slack Help Centre | https://slack.com/help/articles/28310650165907-Security-for-AI-features-in-Slack | No date shown | 17 Oct 2026 |
| S19 | AI Principles | Slack | https://slack.com/trust/ai-principles | No date shown | 17 Oct 2026 |
| S20 | Privacy Principles: Search, Learning and Artificial Intelligence | Slack | https://slack.com/trust/data-management/privacy-principles | No date shown | 17 Oct 2026 |
| S21 | How we built Slack AI to be secure and private | Slack blog | https://slack.com/blog/news/how-we-built-slack-ai-to-be-secure-and-private | 16 Jul 2025 | 17 Oct 2026 |
| S22 | Data residency for Slack | Slack Help Centre | https://slack.com/help/articles/360035633934-Data-residency-for-Slack | No date shown | 17 Oct 2026 |
| S23 | Salesforce Infrastructure and Sub-processors (Slack section) | Salesforce | https://slack.com/slack-subprocessors | Published 2 Oct 2026 (the link opens a Salesforce PDF) | 17 Oct 2026 |
| S24 | Work with AI agents in Slack | Slack Help Centre | https://slack.com/help/articles/33076000248851-Understand-AI-apps-in-Slack | No date shown | 17 Oct 2026 |
| S25 | Set up and manage Agentforce in Slack | Slack Help Centre | https://slack.com/help/articles/36218109305875-Set-up-and-manage-Agentforce-in-Slack | No date shown | 17 Oct 2026 |
| S26 | Use Agentforce in Slack | Slack Help Centre | https://slack.com/help/articles/36218786859667-Use-Agentforce-in-Slack | No date shown | 17 Oct 2026 |
| S27 | Agentforce for Slack (Australia) | Salesforce | https://www.salesforce.com/au/slack/agentforce-in-slack/ | No date shown | 17 Oct 2026 |
| S28 | Connect Slackbot to other apps with MCP | Slack Help Centre | https://slack.com/help/articles/52414744085139-Connect-Slackbot-to-other-apps-with-MCP | No date shown | 17 Oct 2026 |
| S29 | Guide to Model Context Protocol in Slack | Slack Help Centre | https://slack.com/help/articles/48855576908307-Guide-to-Model-Context-Protocol-in-Slack | No date shown | 17 Oct 2026 |
| S30 | Slack MCP server overview | Slack Developer Docs | https://docs.slack.dev/ai/slack-mcp-server/ | No date shown | 17 Oct 2026 |
| S31 | Connect to Claude (Slack MCP server) | Slack Developer Docs | https://docs.slack.dev/ai/slack-mcp-server/connect-to-claude/ | No date shown | 17 Oct 2026 |
| S32 | Manage access to the Slack MCP server through your identity provider | Slack Help Centre | https://slack.com/help/articles/54548358406419-Manage-access-to-the-Slack-MCP-server-through-your-identity-provider | No date shown | 17 Oct 2026 |
| S33 | Slack Securely Powers Your Third-Party Agents With Your Business Context (MCP server and Real-Time Search API now generally available) | Slack blog | https://slack.com/blog/news/mcp-real-time-search-api-now-available | 17 Feb 2026 | 17 Oct 2026 |
| S34 | Slack connectors for Workflow Builder | Slack Help Centre | https://slack.com/help/articles/20155812595219-Slack-connectors-for-Workflow-Builder | No date shown | 17 Oct 2026 |
| S35 | Slack connector (Claude directory listing) | Anthropic | https://claude.com/connectors/slack | "Added November 2025" | 17 Oct 2026 |
| S36 | Slack integration (earlier Claude in Slack app and Slack connector) | Anthropic (Claude docs) | https://claude.com/docs/connectors/slack | No date shown | 17 Oct 2026 |
| S37 | Claude and Slack | Anthropic | https://claude.com/blog/claude-and-slack | 1 Oct 2025; update note dated 26 Jan 2026 | 17 Oct 2026 |
| S38 | What is Claude Tag? | Anthropic Help Center | https://support.claude.com/en/articles/15594475-what-is-claude-tag | "Updated over 3 weeks ago" (no date) | 17 Oct 2026 |
| S39 | Work with Claude Tag | Anthropic (Claude docs) | https://claude.com/docs/claude-tag/overview | No date shown; marked Public Beta | 17 Oct 2026 |
| S40 | Set up Claude Tag | Anthropic (Claude docs) | https://claude.com/docs/claude-tag/admins/setup-overview | No date shown | 17 Oct 2026 |
| S41 | Security and data handling (Claude Tag) | Anthropic (Claude docs) | https://claude.com/docs/claude-tag/concepts/security-and-data | No date shown | 17 Oct 2026 |
| S42 | Data lifecycle and deletion (Claude Tag) | Anthropic (Claude docs) | https://claude.com/docs/claude-tag/concepts/data-lifecycle | No date shown | 17 Oct 2026 |
| S43 | Claude in Slack | Anthropic | https://claude.com/claude-for-slack | No date shown (©2026) | 17 Oct 2026 |
| S44 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (17 Oct 2026) | 17 Oct 2026 |
| S45 | Get started with connectors | Anthropic (Claude docs) | https://claude.com/docs/connectors/getting-started | No date shown | 17 Oct 2026 |
| S46 | Using Slack in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12525822-using-slack-in-chatgpt | "Updated: 6 days ago" (timestamp 11 Oct 2026, UTC) | 17 Oct 2026 |
| S47 | ChatGPT with Slack and Microsoft Teams | OpenAI Help Center | https://help.openai.com/en/articles/20001536-chatgpt-with-slack-and-microsoft-teams | "Updated: 10 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S48 | Using @ChatGPT in Slack and Microsoft Teams | OpenAI Help Center | https://help.openai.com/en/articles/20001537-using-chatgpt-in-slack-and-microsoft-teams | "Updated: 11 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S49 | Setting up and managing @ChatGPT in Slack and Microsoft Teams | OpenAI Help Center | https://help.openai.com/en/articles/20001538-setting-up-and-managing-chatgpt-in-slack-and-microsoft-teams | "Updated: 11 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S50 | Creating and managing team tasks in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001540-creating-and-managing-team-tasks-in-chatgpt | "Updated: 13 days ago" (timestamp 4 Oct 2026, UTC) | 17 Oct 2026 |
| S51 | Slack plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/slack/ | No date shown | 17 Oct 2026 |
| S52 | ChatGPT plugin listing: Slack | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69a1d78e929881919bba0dbda1f6436d | No date shown (version 0.1.8) | 17 Oct 2026 |
| S53 | Managing app permissions in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001495-managing-app-permissions-in-chatgpt | "Updated: 15 days ago" (timestamp 2 Oct 2026, UTC) | 17 Oct 2026 |
| S54 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 8 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S55 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 30 Sep 2026 (page metadata) | 17 Oct 2026 |
| S56 | Partner-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-partners | Updated 25 Sep 2026 (page metadata) | 17 Oct 2026 |
| S57 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Updated 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S58 | Slack (connector reference for Copilot Studio, Power Automate, Logic Apps and Power Apps) | Microsoft Learn | https://learn.microsoft.com/en-us/connectors/slack/ | Updated 2 Oct 2026 (page metadata) | 17 Oct 2026 |
| S59 | Publish an agent to Azure Bot Service channels (Copilot Studio) | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-connect-bot-to-azure-bot-service-channels | Updated 3 Aug 2026 (page metadata) | 17 Oct 2026 |
| S60 | Microsoft 365 Copilot connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview | Updated 12 Oct 2026 (page metadata) | 17 Oct 2026 |
| S61 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S62 | Use apps connected to Gemini with a work or school Google Account | Google Gemini Apps Help | https://support.google.com/gemini/answer/14959807?hl=en | No date shown | 17 Oct 2026 |
| S63 | Slack connector overview (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/slack | "Last updated 2026-10-14 UTC" | 17 Oct 2026 |
| S64 | Configure the Gemini Enterprise app for Slack | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/configure-slack-app | "Last updated 2026-10-14 UTC" | 17 Oct 2026 |
| S65 | Gemini Enterprise release notes | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/release-notes | "Last updated 2026-10-14 UTC" | 17 Oct 2026 |
| S66 | Connect a third-party data source (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/connect-third-party-data-source | "Last updated 2026-10-15 UTC" | 17 Oct 2026 |
| S67 | Customise data retention in Slack | Slack Help Centre | https://slack.com/help/articles/203457187-Customize-data-retention-in-Slack | No date shown | 17 Oct 2026 |
