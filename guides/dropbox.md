# Dropbox: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

Dropbox's help pages show an "Updated" date, and the Sources table records it. Where a Microsoft page shows no date on screen, we took the date from the page's own publishing data. OpenAI's help pages show a relative date ("8 hours ago"), so we also give the page's timestamp in UTC.

## The short version

- Dropbox's own AI is called Dash. It searches your files and your other work apps and answers questions about them. You open it from a side panel in Dropbox or at dash.ai. [S3] [S5]
- Dash is a paid plan on top of Dropbox. Dash for Teams is $15 per user a month billed yearly, or $19 billed monthly. The page doesn't say which currency. [S2]
- Teams in Australia can start a free Dash for Teams trial. Dropbox's security paper says Dash can't yet store data outside the United States. [S3] [S11]
- Dropbox says it won't build generative AI models from customer content without consent. It lists "No customer data used for third party model training" and a 90-day retention period for the AI models behind its features. [S14] [S12]
- ChatGPT, Claude and Microsoft Copilot each have an official Dropbox connection that Dropbox built. They can find your files and save new ones to Dropbox, all within what your own Dropbox login allows. [S30] [S31] [S32]
- Gemini has one too, but Google lists it for personal Google accounts in the US only. [S73] [S74]
- Dropbox says ChatGPT asks before it changes your files. Its ChatGPT page also says conversations and Dropbox data in ChatGPT "may be used for model training according to OpenAI's policies". [S30]
- Microsoft also makes a Dropbox connector that copies (indexes) a team's files into Copilot search. Its default setting makes every file anyone can open in Dropbox visible to everyone in your Microsoft 365 organisation. [S63] [S64]
- Team admins can block AI apps in the Dropbox admin console. Blocking doesn't disconnect people who've already connected. [S28]

## The tool, and the plans that matter

Dropbox is online file storage and sharing, with e-signatures and other products alongside. Its plans page sums it up as "Store and share files. Sign and send documents." [S1]

These are the prices on Dropbox's plans page as shown to a visitor in Australia on 17 October 2026. [S1]

| Plan | Who it's for | Monthly (AUD) | Yearly (AUD) | Storage and deleted-file recovery |
|---|---|---|---|---|
| Basic | Anyone | Free | Free | 2 GB |
| Plus | 1 person | AU$18.69 | AU$184.67 | 2 TB. Restore deleted files for 30 days |
| Standard | 1 person or more | AU$27.50 a user | AU$277.20 a user | Starts at 3 TB for the team. 180 days to restore |
| Advanced | 3 people or more | AU$43.45 a user | AU$435.60 a user | Starts at 15 TB for the team. 1 year to restore |
| Enterprise | Companies | "Contact us for pricing" | "Contact us for pricing" | Not shown |

Sources for the table: [S1]

- Plus, Standard and Advanced each list "Integrate with leading AI tools" as a feature. [S1]
- The page doesn't say whether these prices include GST. [S1]
- Dash is sold separately. Dropbox's Dash plans page lists Dash for Teams (up to 100 users) and Dash for Business (over 100 users). [S2]
- Dropbox's help centre also names Business and Business Plus plans, which the Australian plans page doesn't show. [S3] [S1]

**Words used in this guide**

- **Dash** is Dropbox's AI tool. Dropbox says "Dropbox Dash and Dash for Business are now referred to as Dash." [S11]
- **Dash in Dropbox** is Dash opened from the side panel of the Dropbox website. Dropbox calls it "AI in Dropbox, powered by Dash". [S3] [S46]
- **Dropbox AI** was Dropbox's 2023 name for summaries and questions inside file previews. It started as an alpha for US customers. [S48] Dropbox's old "Dropbox AI" help address now opens a Dash article, so it appears the feature was folded into Dash. That's our reading. [S6]
- An **MCP server** is a standard plug that lets an AI assistant use another service. Dropbox runs its own. [S35] [S11]

**Where your files live**

- Dropbox's storage servers are in data centres across the United States. [S22]
- Storage is also available in Australia, the European Union, Japan and the United Kingdom for eligible users. [S22]
- A team can ask to move its file data to Australia if it's on Standard, Advanced, Business, Business Plus or Enterprise, has at least 10 licences and pays yearly. [S22]
- Dropbox says requests are "reviewed individually". You can't choose the new server's location, and the move can't be undone. [S22]
- The choice covers team file data "while stored permanently at rest". [S22]
- Dropbox's Australian file storage is hosted on Amazon Web Services in Australia. [S23]
- More broadly, Dropbox's privacy policy says it may store, process and transmit data "in the United States and locations around the world". [S18]

## AI built in

### Dash (Dropbox's AI, in Dropbox and at dash.ai)

**What it does**

- Searches Dropbox and the work apps you connect, using everyday questions. You don't need the exact file name. [S5]
- Summarises documents and conversations and answers questions about your work. [S5]
- Drafts written work and rewrites it for clarity or tone. [S5]
- Groups files, links and conversations into "Stacks" for a project. [S5]
- Image search can match what's in a picture. A "Text in image" filter works on JPG, PDF, PNG and TIFF files. [S6]
- Searches the web too. Web search is on by default and uses OpenAI's web search API (gpt-5-mini). [S6]
- Lets you pick an AI model, or leave it on **Auto** so Dropbox chooses. Dropbox says "Model availability may change over time." [S8]
- The Chrome extension answers questions about any web page. Its buttons include **Summarize & Highlights**, **Next Steps** and **Quick Draft**. [S7]
- Dropbox's help lists 29 sources Dash can search, including Google Drive, Microsoft 365, Microsoft Teams, Slack, Notion, Gmail and Zoom. [S79]

**Where to find it**

- In Dropbox, open Dash from the right-side panel on the Dropbox home page. [S3]
- Or go to dash.ai, or use the Dash desktop and mobile apps. [S3] [S4]
- Ask, Write and Organize work on dash.ai and in the desktop app. They don't work in the mobile app. [S4]
- In Dash Chat, attach a file with the add (**+**) icon and ask about it. Files can be up to 25 MB, and Dash summarises up to 20,000 characters. [S7]
- To choose a model, log in to dash.ai, click **Chats**, then **Model**, and pick from the list. [S8]
- An admin connects the team's Dropbox to Dash in the admin console under **Dash** > **More Apps** > **Add** next to **Dropbox**. Dropbox says this syncs "your organization's entire Dropbox content with Dash". [S26]

**Which plans have it**

- Dropbox describes Dash for Teams and Dash for Business as "two plans that make Dash, our AI-powered productivity tool, available directly in Dropbox." [S3]
- Dash for Teams costs $15 per user a month billed yearly, or $19 billed monthly. Dash for Business is $35 per user a month, billed yearly only. [S2]
- Viewed from Australia, the Dash plans page still shows a plain "$" with no currency. The main Dropbox plans page shows AU$. [S2] [S1]
- A banner offers "50% off" to Dropbox Standard, Advanced, Business and Business Plus customers. It doesn't say for how long. [S2]
- Dropbox says future plans "may include a limit on how many items each member can use with Dash". It will email you at least 30 days before a limit starts. [S2]
- Teams on Basic, Standard, Business, Advanced or Business Plus can start a free Dash for Teams trial. Only team admins can enrol a team. [S3]
- Dropbox's Dash page says the free trial for small teams lasts 30 days. [S49]
- Individual users on Plus, Professional or Essentials can't start a trial, and nor can managed teams. [S3]
- Dropbox's Trust Center says many Dropbox for Teams plans "include intelligent features powered by Dropbox Dash". We couldn't match that to a list of plans. [S13]

**What happens to your data**

- Dropbox's AI principles say: "We will not build generative AI models using customer content without consent." [S14]
- Dropbox's Trust Center lists two controls for every model behind its AI features: "No customer data used for third party model training" and a "90 day data retention period". [S12]
- The model table lists OpenAI models such as GPT-5.4 and GPT-4.1, mostly run in a Dropbox-managed environment on Microsoft Azure. Some also run through OpenAI itself, and GPT OSS 20B runs on Groq. [S12]
- The same table lists Anthropic's Claude Opus 4.7, Claude Opus 4.6 and Claude Sonnet 4.6, run through AWS Bedrock. [S12]
- Dash's sub-processor list, updated 29 April 2026, names Google, OpenAI, Amazon Web Services, Microsoft, Groq and Parallel Web Systems for "Large Language Model Processing". All are located in the United States. [S15]
- Dropbox says it "may manually review snippets of the questions you ask and the responses you receive", de-identifying them where possible. [S11]
- Dropbox may also use data about how you use Dash to improve and fine-tune it. It says Dash has controls to opt out of that. [S11]
- Dash stores the content it indexes and creates "temporary embeddings" (number codes that help it compare text). These stay until the document is deleted or its source is disconnected. [S11]
- When an admin disconnects an app from Dash, Dash starts purging that app's content. [S11]
- Admins can keep specific files, folders, drives or sites out of Dash for some connected apps. Changes take 6 to 24 hours. [S11]
- Dash only shows content each person is allowed to see in the original app. [S11] [S34]
- If a trial ends without a paid plan, connected apps are removed 30 days later. Search and chat history are deleted too. [S2]
- Dropbox's privacy FAQ, last updated in April 2024, says Dash imports your browser history "starting with the previous 90 days", including the pages' content, when you use the Dash browser extension and desktop app. [S17]
- It adds that Dropbox may share this data with trusted third parties to power Dash's search. [S17]
- The same FAQ says models that improve search "may be trained on your documents and metadata". [S17]
- Admin settings live under **Admin console** > **Dash** > **Settings**. They cover single sign-on, domain verification, an email domain allowlist for some apps, and public sharing of Stacks. [S24]
- We found no single switch that turns Dash off for a whole team while keeping a paid Dash plan. See "What we couldn't establish". [S24] [S25]

**In Australia**

- To start a Dash for Teams trial, your team must be located in the United States, the United Kingdom or Australia, with English as the account's primary language. [S3]
- Dropbox's Dash security paper says "currently Dash does does not offer an option for data storage outside of the US" (Dropbox's typo). [S11]
- So a team whose Dropbox files are stored in Australia should expect Dash's copy of them to sit in the US. That's our inference from those two Dropbox statements. [S22] [S11]
- Dash isn't offered to accounts that need HIPAA compliance (a US health-privacy setting) or that use managed encryption keys. [S3]
- The Dash mobile app is only available "in select countries" and in English. [S4]

## Outside AI that connects

Dropbox builds its own app for each of the four big assistants and lists them on one help page, "AI integrations". [S29] Each one works within the Dropbox permissions of the person who connects it. [S30] [S31] [S32] [S33]

There are two kinds of connection. The **Dropbox** app works with your Dropbox files. The **Dropbox Dash** app is separate: it brings in what Dash has indexed from your other work apps, for teams that pay for Dash. [S34] [S40]

### Claude and Dropbox

**Official?**

- Yes. The Dropbox connector in Claude's directory is "Made by Dropbox", marked "Anthropic verified" and was added in June 2026. [S51]
- Dropbox also publishes a Dropbox plugin for Claude Cowork and Claude Code, also marked Anthropic verified. [S31] [S52]
- Dropbox announced the connector and plugins on 25 June 2026. [S39]

**What it can see and do**

- Find files and folders and check the details of supported files. [S31]
- Organise folders, and create Dropbox links and file requests (a link others use to upload files to you). [S31]
- Save text that Claude writes back to Dropbox as a new file. [S31]
- The connector's tool list also includes copy, move and delete. [S51]
- When you connect, Dropbox asks for permission to view and edit your files and folders, sharing information and file requests, and to view your account details. [S31]
- Claude can only save text-based files, such as .txt, .md, .html and .py. It can't save images or PDFs this way. [S31]
- People who receive a link made through Claude have to request access to it. [S38]
- Dropbox says "Claude can only use content and complete actions that your connected Dropbox account already has permission to access." [S38]
- If your team pays for Dash, the separate Dropbox Dash connection brings in content from your other work apps. Type **@** and pick **Dropbox Dash**. [S34]

**What you need**

- An active Dropbox account, on any plan. The Dropbox app or plugin must be allowed for your organisation. [S31]
- Anthropic says directory connectors are available on Claude, Cowork, Claude Desktop and Claude mobile. [S53]
- Plugins need a paid Claude plan: Pro, Max, Team or Enterprise. [S54]
- On Claude Team and Enterprise, an owner turns the connector on for the organisation first. Each person then signs in to Dropbox. [S53]

**Steps to connect** (Dropbox Help Center, updated 17 September 2026)

1. On claude.ai, click the add (**+**) icon in the search bar, then **Add connectors**. [S31]
2. Click the add (**+**) icon next to Dropbox. [S31]
3. Log in to Dropbox, review the permissions and click **Continue**. [S31]
4. In the Claude desktop app, use the **Chat**, **Cowork** or **Code** tab instead: **Customize** > **Connectors** > **Add** > **Browse connectors**, then search for Dropbox. [S31]
5. For the plugin, click **Browse plugins** on claude.ai, or **Customize** > **Plugins** > **Add** in the desktop app, and add Dropbox. [S31]
6. In a chat, click **+** (or type **/**), go to **Connectors** and switch Dropbox on. [S53]

Dropbox says you only need to connect once, and the connector then works in claude.ai, Cowork and Code. [S31]

**For Claude Team and Enterprise owners**

- Dropbox's steps: in Claude's Organizational Settings, go to **Connectors**, click **Add+** and save. To block it, open the more options menu next to Dropbox and click **Delete**. [S31]
- For the plugin, Dropbox lists the choices **Not available**, **Installed by Default**, **Available to Install** and **Required**. [S31]
- Anthropic's own path is **Organization settings** > **Connectors** > **Browse connectors** > **Add to your team**. Owners can then set each tool to **Always allow**, **Needs approval** or **Blocked**. [S53]

**To disconnect**

- In Claude, go to **Customize** > **Connectors**, select Dropbox and disconnect it. [S53]
- Dropbox's Claude page doesn't give steps for disconnecting from the Dropbox side. Its pages for the other assistants use **Settings** > **Apps** on dropbox.com. [S31] [S32]

**Limits**

- Anthropic's listing warns that Anthropic "does not control which tools developers make available and cannot verify that they will work as intended." [S51]
- On Claude's Free, Pro and Max plans, Anthropic doesn't train on raw content from connectors unless you copy it into the chat. Your chats are used for training only if you allow it. [S55]
- On Claude's work plans, Anthropic doesn't use inputs or outputs for training by default. [S56]

### ChatGPT and Dropbox

**Official?**

- Yes. OpenAI's plugin directory lists **Dropbox**, with Dropbox as the developer (version 6.0.0). [S58] [S57]
- Dropbox launched its ChatGPT apps on 16 April 2026: a Dropbox app, a Dropbox Dash app and a Reclaim AI calendar app. [S40]
- Since 10 September 2026, you can browse, search and @mention Dropbox files from ChatGPT's Library on the web. [S43]
- On 8 September 2026 Dropbox joined OpenAI's Small Business collection in the ChatGPT plugin directory. [S42]

**What it can see and do**

- Browse, search and preview Dropbox files, and add them to a conversation. [S30]
- Summarise, analyse and compare files such as PDFs, Word documents, spreadsheets and presentations. [S30]
- Move, copy, delete and restore files and folders, and list a file's revisions. [S30]
- Save ChatGPT's work to Dropbox, create and list shared links, and create and manage file requests. [S30]
- Send and manage Dropbox Sign signature requests. [S30]
- OpenAI's listing names six Dropbox skills, including **organize-dropbox-folder**, **share-dropbox-content** and **clean-up-dropbox-content**. [S57] [S58]
- Dropbox says ChatGPT "will request your permission before making any changes to your data". [S30]
- Dropbox says the plugin "follows your existing Dropbox permissions and team policies." [S30]
- The separate **Dropbox Dash** app pulls in context from the work apps your team has connected to Dash, and respects their permissions. [S59] [S60]

**What you need**

- Dropbox says the plugin is "available to customers on all Dropbox plans using ChatGPT". [S30]
- OpenAI says app availability depends on the app, your ChatGPT plan, region, workspace, role, model and the ChatGPT version you use. [S61]
- In ChatGPT Business, many apps are on by default. New Enterprise and Edu workspaces start with a selected set, and admins can change access. [S61]
- The Dash app needs a Dash plan or trial. When Dropbox announced it, it said the Dash app would reach existing Dash customers "in the coming weeks". [S40]

**Steps to connect** (Dropbox Help Center, updated 30 September 2026)

1. Open ChatGPT and click **Plugins** in the left sidebar. [S30]
2. Select **Dropbox** and click **Install plugin**. [S30]
3. Click **Sign in with Dropbox**. [S30]
4. Log in to Dropbox. If you have paired personal and work accounts, choose the one you want to connect. [S30]
5. In a chat, enter **@Dropbox** in your prompt, or click the add button in the prompt box and choose Dropbox. [S30]

**To disconnect**

- In ChatGPT, users disconnect apps from **Settings** > **Plugins**. [S61]
- In Dropbox, log in to dropbox.com, click your avatar in the bottom-left corner, then **Settings** > **Apps**. Click the arrow next to ChatGPT, then **Disconnect**. [S30]
- Dropbox says "Team admins can also block the app for their organization." [S30]

**Limits**

- Dropbox's page says: "Conversations and other Dropbox data in ChatGPT may be used for model training according to OpenAI's policies." [S30]
- OpenAI says that on Free, Plus, Go and Pro, information from apps may be used for training if your "Improve the model for everyone" setting is on. On Business, Enterprise and Edu it isn't used for training by default. [S61]
- Dropbox says data that appears in a ChatGPT conversation is stored unless you delete the conversation. [S30]
- OpenAI's listing says ChatGPT may share relevant chats and memories with the Dropbox app, under Dropbox's terms and privacy policy. It also says "Use of apps may come with elevated risk." [S58]

### Microsoft Copilot and Dropbox

**Official?**

- Yes, by two routes. **Dropbox for Copilot** is Dropbox's own plugin, listed free in Microsoft's Marketplace by Dropbox.com for Microsoft 365 Copilot. [S67] [S32]
- Microsoft also builds a **Dropbox** connector that an admin deploys. It indexes Dropbox content into Microsoft 365 Copilot and Microsoft Search. [S63] [S66]

**What it can see and do: Dropbox for Copilot**

- Find files and folders, and open and summarise supported content. [S32]
- Organise folders, create shared links and save text that Copilot writes. [S32]
- Saved files must be new UTF-8 text files up to 5 MB, in formats such as .txt, .md, .csv, .json and .html. [S32]
- Dropbox says "Copilot can only access Dropbox content you have permission to access." [S32]
- Copilot Cowork, where the plugin runs, asks for your go-ahead before important actions. A dropdown lets you skip future prompts for similar actions. [S68]

**What it can see and do: Microsoft's Dropbox connector**

- It indexes files in team folders, shared folders and private folders, and shows them in Copilot answers and Microsoft Search. [S63]
- "Currently, only Dropbox Advanced and Enterprise plans are supported." [S63]
- It doesn't index folders, comments, Dropbox Paper or Google Docs, Sheets and Slides. Permissions that come from shared links aren't supported. [S63]
- By default it indexes files updated in the past three years. It checks for changes every 4 hours and does a full crawl every day. [S64]
- The default access setting is: "All files accessible to anyone in Dropbox are visible to all Microsoft 365 users in your tenant." [S64]
- To limit results to people who can open the file in Dropbox, choose **Custom setup** and then **Only people with access to this data source**. [S64]

**What you need**

- Dropbox for Copilot works on any Dropbox plan, for customers "using Microsoft Copilot". [S32]
- Microsoft says Cowork for work and school accounts is generally available to Microsoft 365 Copilot tenants worldwide "in tier-1 languages". Cowork for personal accounts is in preview. [S70] [S68]
- If you don't see a plugin, Microsoft says your organisation might need to approve it first. [S69]
- Microsoft's connector needs a Microsoft 365 admin, and a Dropbox admin to set up an app in the Dropbox App Console. [S64] [S65]

**Steps to connect: Dropbox for Copilot** (Dropbox Help Center, updated 30 September 2026)

1. Log in to Microsoft Copilot at copilot.com or in the Copilot desktop app. [S32]
2. Go to **Copilot Cowork** and click **Customize** in the left navigation bar. [S32]
3. Search for **Dropbox for Copilot**, click **Install**, then **Connect**. [S32]
4. Log in to Dropbox in the window that opens and click **Allow**. [S32]
5. Click **New task** and mention Dropbox in your prompt. [S32]

Microsoft's own steps for Cowork plugins start from the **+** button and **Customize**. [S69] Microsoft gives copilot.cloud.microsoft as the web address for Cowork, while Dropbox's page says copilot.com. [S68] [S32]

**Steps for admins: Microsoft's Dropbox connector** (Microsoft Learn)

1. The Dropbox admin opens the Dropbox App Console, selects **Create app**, and sets it up with scoped access and full Dropbox access. [S65]
2. They add Microsoft's redirect address and the listed permissions (scopes), then copy the app key and app secret from the **Settings** tab. [S65]
3. In the Microsoft 365 admin center, the Microsoft admin chooses **Copilot** > **Connectors**, the **Gallery** tab, then **Dropbox**. [S64]
4. They enter the app key and secret. **Rollout to limited audience** can limit who gets it at first. [S64]
5. Before choosing **Create**, use **Custom setup** to pick **Only people with access to this data source**. The connector starts indexing straight away. [S64]

**To disconnect**

- Dropbox for Copilot: on dropbox.com, click your avatar, then **Settings** > **Apps**, the arrow next to Copilot, then **Disconnect**. [S32]
- In Cowork, select **+** > **Customize**, find the plugin and select **Remove from Cowork**. Plugins your admin deployed can only be removed by the admin. [S69]
- Microsoft's connector: admins review it in the **Connectors** section of the Microsoft 365 admin center. The pages we read don't give steps to remove it. [S64]

**Limits**

- Microsoft says prompts, responses and data accessed through Microsoft Graph "aren't used to train foundation LLMs". It tells you to check each agent's privacy statement and terms. [S72]
- Dropbox's page points to Microsoft for how data and training work, and says it depends on the Copilot product and account. [S32]
- Microsoft says customers outside the EU may have their queries processed in the US, the EU or other regions. [S72]
- Microsoft says Cowork keeps task history, and some interactions get automated and human review. That page covers personal accounts in preview. [S71]

### Google Gemini and Dropbox

**Official?**

- Yes, but it isn't offered in Australia. Dropbox announced its connected app for Gemini on 17 September 2026. [S44]
- Google's availability table lists Dropbox for personal Google accounts only, aged 18 or over, "US only", in English only. [S74]

**What it can see and do**

- Find and summarise files and pull information out of them. [S73]
- Create, rename, copy, move and delete files and folders. [S73]
- View a file's version history and restore an earlier version. [S73]
- You must confirm sensitive actions, including deleting, sharing or changing permissions, and bulk actions. [S73]
- Dropbox says Gemini can save its output to Dropbox only as .csv or .txt files. [S33]
- Dropbox says Gemini asks for permission before making changes. [S33]

**What you need**

- A personal Google account (work and school accounts aren't supported yet), aged 18 or over, in the US, with Keep Activity turned on. [S73]
- It works in the Gemini web app and the Gemini app for Windows. [S74]
- Gemini Spark, Google's tool for multi-step tasks, can also use Dropbox, for Google AI Pro and Ultra subscribers in the US. [S45] [S76]
- Google's general Spark rollout from 17 June 2026 excluded Australia, among other countries. [S76]

**Steps to connect** (Dropbox Help Center, updated 21 September 2026)

1. Log in to Gemini and click **Settings**. [S33]
2. Click **Personal Intelligence**, then **Connected apps**. [S33]
3. Click **Other** and switch Dropbox **On**. [S33]
4. Click **Allow**, then **Continue**. [S33]
5. Click **Agree and continue**, then **Allow**. [S33]
6. In a chat, type **@Dropbox**. [S33]

Google's general path for connected apps is **Customize** > **Connectors** > **Add**. [S75] Google's Dropbox page adds that you can ask Gemini to do something in Dropbox and it will offer to connect. [S73]

**To disconnect**

- In Gemini, disconnect Dropbox in your Connected Apps settings at any time. [S73]
- In Dropbox, click your avatar, then **Settings** > **Apps**, the arrow next to Gemini, then **Disconnect**. [S33]

**Limits**

- Dropbox's page says Gemini app conversations may be used for model training under Google's policies. [S33]
- Google says Connected Apps availability varies by location, language, device and Gemini app. [S75]
- Google's separate business product, Gemini Enterprise, has its own Dropbox connector, marked "For Organizations and Teams only". Its actions include creating folders and uploading or downloading files up to 50 MB. [S77] [S78]

### Dropbox's MCP servers (the developer route)

**Official?**

- Yes. Dropbox runs a remote MCP server at https://mcp.dropbox.com/mcp. Dropbox says it's "now in beta". [S35]
- A separate Dash MCP server at https://mcp.dropbox.com/dash searches what Dash has indexed. Dropbox describes its connector actions as read-only. [S36]
- Dash's release notes list the Dash MCP server in October 2025. [S9]
- DocSend, another Dropbox product, has its own MCP server, in open beta for Advanced Data Rooms users since August 2026. [S10]

**What it can see and do**

- Read and browse files, folders, revisions and your storage use. [S35]
- Create folders and text files up to 5 MB. [S35]
- Copy, move and delete. Delete moves items to Deleted files, which you can recover within your plan's window. [S35]
- Restore folders and earlier file versions, create shared links and manage file requests. [S35]
- Dropbox Sign tools can send a document for signature, send reminders and cancel requests. You review and confirm those actions before they happen. [S37]

**What you need**

- Supported clients are Claude Code, Claude Web, ChatGPT Codex, ChatGPT Web and Cursor. [S35]
- Dropbox says Claude custom connectors are "available on select Claude plans" and ChatGPT Developer Mode is "available on certain plans". [S35]
- Your Dropbox admin may control whether you can register or connect apps. [S35]
- For Dropbox Sign tools, your Dropbox account must be connected to your Dropbox Sign account. [S37]

**Steps to connect** (Dropbox Help Center, updated 30 September 2026)

1. In Claude on the web or desktop, go to **Settings** > **Connectors** > **Add custom connector**. Name it "Dropbox MCP", enter https://mcp.dropbox.com/mcp and click **Add**. [S35]
2. Dropbox's ChatGPT steps turn on **Developer mode** under **Settings** > **Apps & Connectors** > **Advanced settings**, then use **Settings** > **Apps** > **Create app** with OAuth sign-in. [S35]
3. OpenAI's current page says Enterprise and Edu users can add a custom MCP server directly from **Plugins** and "don't need to turn on Developer Mode first". On Business, only admins and owners can create them. [S62]
4. Sign in to Dropbox when asked, and approve the access. [S35]

**Limits**

- OpenAI says Pro users can connect custom MCP servers with read and fetch permissions only. Full MCP, including write actions, is for Business, Enterprise and Edu. [S62]
- Dropbox's business agreement says beta services "have not been subjected to the same Security Measures and auditing" and are used at your own risk. [S21]
- Listing a folder returns up to 100 items per call, and reading a file works up to 5 MB. [S35]
- If you change your Dropbox app settings, such as adding a permission, you must reconnect. [S35]

### Automation tools Dropbox documents

- Dropbox's help centre has a Zapier guide for "all customers on a paid Dropbox plan". Zapier links Dropbox with other apps to automate tasks. [S50]

## Jobs it's good for

- **Finding the right version.** Ask Dash for the latest copy of a document across Dropbox and your other apps, without knowing the file name. [S5]
- **A long PDF before a meeting.** Attach it in Dash Chat and ask for a summary, or ask ChatGPT to summarise it from Dropbox. [S7] [S30]
- **Checking a clause.** OpenAI's example asks ChatGPT to find a contract's renewal notice period, quote it and link the document so someone can check it. [S57]
- **Collecting files from clients.** Ask Claude or ChatGPT to create a Dropbox file request, which people can use to upload files to you. [S31] [S30]
- **Tidying a folder.** Dropbox's ChatGPT skills can organise folders. [S41] [S57] Ask it to list what it plans to move before it starts. That's our advice.
- **A project brief from your files.** Ask Copilot Cowork to draft one from Dropbox files and save it back as a text file. [S32]
- **Chasing a signature.** Through the MCP server, send a Dropbox Sign reminder and confirm it before it goes. [S37]

## What to watch for

**The AI sees what the login sees**

- All four official connections work within the Dropbox permissions of the person who connects. [S30] [S31] [S32] [S33]
- Dash shows only content each person can see in the original app. [S34]
- So an admin who connects with an admin login will reach everything that login can reach. That's our inference from the above.

**Microsoft's connector shares widely by default**

- Its default setting makes every file anyone can open in Dropbox visible to all Microsoft 365 users in your organisation. [S64]
- Change it under **Custom setup** before you create the connection. [S64]
- It doesn't support permissions that come from shared links. [S63]

**These connections can change and delete files**

- ChatGPT can move, copy, delete and restore files. Dropbox says it asks first. [S30]
- Gemini can delete files and folders, and you confirm each sensitive action. [S73]
- Claude's connector tool list includes move and delete. [S51]
- Deleted items go to Deleted files. You can restore them for 30 days on Plus, 180 days on Standard and a year on Advanced. [S35] [S1]
- Blocking an app in the admin console "doesn't disconnect team members who are already connected". [S28]

**Training and who keeps what**

- Dropbox says it won't build generative AI models from your content without consent, and its AI providers don't train on your data. [S14] [S12]
- Dropbox may review snippets of Dash questions and answers by hand. [S11]
- Your chat history on the AI side follows that company's settings. Dropbox's ChatGPT page warns ChatGPT data may be used for training under OpenAI's policies. [S30] [S61]
- Claude's consumer plans train on chats only if you allow it, and its work plans don't by default. [S55] [S56]

**Where your data goes**

- Dash can't yet store data outside the US. [S11]
- Its AI sub-processors are all listed in the US. [S15]
- Dropbox can keep a team's files in Australia, but that covers file storage at rest. [S22]
- Microsoft says queries from outside the EU may be processed in the US, the EU or elsewhere. [S72]

**Untrusted text**

- Dropbox says it treats image metadata as untrusted, and uses a tool called Lakera Guard to detect attempts to extract personal data from training sets. [S11]
- Dropbox's Trust Center says its AI features include protections against prompt injection. That's an attack where instructions hidden in content try to steer the AI. [S12]
- A shared folder from outside your business can carry text like that. Keep a person checking before files are moved, shared or deleted. That's our advice.

**Beta and preview**

- The Dropbox MCP server is in beta, and Dropbox's agreement says beta services are used at your own risk. [S35] [S21]
- Cowork for personal Microsoft accounts is in preview. [S68]

**Cost surprises**

- Dash is an extra charge per user, and Dropbox may add item limits later. [S2]
- When a Dash trial ends without a paid plan, connected apps and search and chat history are deleted after 30 days. [S2]
- Microsoft bills Cowork by usage. Admins can set limits per user or group. [S70]

## Announced changes

Dropbox's blog posts say timing and features may change from what's described. [S39] [S44]

- **21 June 2023:** Dropbox announced Dropbox AI for file previews (alpha, US) and Dash (beta, by waitlist). [S48]
- **27 September 2025:** Dropbox launched its AI Transparency resource in the Trust Center. [S13]
- **23 October 2025:** Dash in Dropbox reached "a small group of existing customers". Dash opened to teams of all sizes, and the Dash MCP server launched. [S46] [S9]
- **January 2026:** Dash added a model picker and web search, with notice when web search runs. [S9]
- **March 2026:** The Dropbox app in ChatGPT added file previews and saving to Dropbox. [S10]
- **16 April 2026:** Dropbox launched its Dropbox, Dropbox Dash and Reclaim AI apps in ChatGPT. [S40]
- **29 April 2026:** Dropbox updated both its Dash and Dropbox sub-processor lists. [S15] [S16]
- **May 2026:** Dropbox Protect launched as a separate product, with features "previously available in Dropbox Dash as Protect and Control". [S10]
- **25 June 2026:** The Claude connector and plugins launched. [S39]
- **12 July 2026:** ChatGPT, ChatGPT Work and Codex gained tools to organise files, make links and file requests, and run Dropbox skills. [S41]
- **August 2026:** DocSend's MCP server entered open beta. [S10]
- **10 September 2026:** Dropbox files appeared in ChatGPT's Library on the web. Dropbox said mobile is coming soon. [S43]
- **17 September 2026:** The Dropbox app for Gemini launched in the US. [S44]
- **Later, no date:** Dash plans may add a limit on items per member, with at least 30 days' email notice. [S2]
- **1 January 2027:** New Dropbox Terms of Service take effect. They were posted on 1 September 2026, and we found no AI clauses in them. [S20] [S19]
- Dropbox's product updates page still lists Dash in Dropbox and the remote MCP server as "Coming soon". Other Dropbox pages say both are now available, so that page appears out of date. [S47] [S3] [S35]

## What we couldn't establish

- **The currency of Dash prices.** The Dash plans page shows "$" with no currency, even from Australia. [S2]
- **Which Dropbox plans include Dash features without a Dash plan.** The Trust Center says many team plans include them, while the help centre describes Dash plans as the way to get Dash in Dropbox. [S13] [S3]
- **A team-wide off switch for Dash.** The admin help we read covers security settings, licences and cancelling a trial, but no single switch for a paid team. [S24] [S25] [S27]
- **Where Dash's opt-out for usage data sits.** Dropbox says the control exists but the pages we read don't say where. [S11]
- **Dropbox's AI FAQ.** It's a PDF in the Trust Center that we didn't open. [S12]
- **How long Dash keeps chat history.** The pages we read don't say, apart from deletion after a trial ends. [S2] [S11]
- **Whether the 90-day retention also covers web search through OpenAI.** The Trust Center states it for "all models used to power Dropbox AI features". [S12] [S6]
- **Dropbox Paper and Microsoft's connector.** Microsoft's overview says Paper isn't crawled, while its setup page says the connector indexes Paper documents. [S63] [S65]
- **One Microsoft setup permission.** The Dropbox-side setup asks for a permission named team_data.governance.write. Microsoft doesn't explain what it writes. [S65]
- **Which Copilot accounts Dropbox for Copilot supports.** Dropbox's page says copilot.com, Microsoft's Marketplace lists Microsoft 365 Copilot, and the pages don't say whether a paid Microsoft 365 Copilot licence is required. [S32] [S67] [S70]
- **How to remove Microsoft's Dropbox connector.** Not in the pages we read. [S64]
- **Which ChatGPT plans can use the Dropbox plugin.** Neither Dropbox nor OpenAI names them. [S30] [S61]
- **OpenAI's Dropbox article.** OpenAI's plugin page links to a "Dropbox - app with sync" article, which now opens OpenAI's general connected apps page. [S57] [S61]
- **Disconnecting Claude from the Dropbox side.** Dropbox's Claude page doesn't cover it. [S31]
- **GST on Australian prices.** The plans page doesn't say. [S1]
- **The Dropbox Make listing.** Dropbox's App Center page for Make wouldn't load for us.

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Find your Dropbox plan (as shown in Australia) | Dropbox | https://www.dropbox.com/plans | No date shown | 17 Oct 2026 |
| S2 | Get Dropbox Dash (plans) | Dropbox | https://dash.dropbox.com/plans | No date shown | 17 Oct 2026 |
| S3 | How to try Dash for Teams | Dropbox Help Center | https://help.dropbox.com/plans/try-dropbox-dash-in-dropbox | Updated Apr 22, 2026 | 17 Oct 2026 |
| S4 | Restrictions and limitations for team deployments of Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/account-access/dash-deployment | Updated May 12, 2026 | 17 Oct 2026 |
| S5 | What can I do with Dropbox Dash? | Dropbox Help Center | https://help.dropbox.com/view-edit/what-can-i-do-with-dropbox-dash | Updated Apr 15, 2026 | 17 Oct 2026 |
| S6 | How to search and explore your content in Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/view-edit/dropbox-ai-how-to | Updated May 6, 2026 | 17 Oct 2026 |
| S7 | How to summarize and ask questions about your content in Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/view-edit/summarize-and-ask-questions-in-dash | Updated May 5, 2026 | 17 Oct 2026 |
| S8 | How to choose a chat model in Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/view-edit/dropbox-dash-chat-model-picker | Updated Jan 23, 2026 | 17 Oct 2026 |
| S9 | Dropbox Dash release notes | Dropbox | https://dash.dropbox.com/release-notes | Monthly entries, latest March 2026 | 17 Oct 2026 |
| S10 | Dropbox release notes | Dropbox | https://www.dropbox.com/release-notes | Monthly entries, latest August 2026 | 17 Oct 2026 |
| S11 | Dropbox Dash Security Whitepaper | Dropbox | https://aem.dropbox.com/cms/content/dam/dropbox/warp/en-us/dash/Dash-Security-Architecture-Overview_Whitepaper.pdf | Version V2026.3 (no date) | 17 Oct 2026 |
| S12 | AI Transparency: AI FAQ, AI principles and model information | Dropbox Trust Center | https://trust.dropbox.com/?itemUid=6fe99d99-2326-4013-8eab-e79467fcfe56&source=click | No date shown | 17 Oct 2026 |
| S13 | Dropbox Trust Center (overview and updates) | Dropbox | https://trust.dropbox.com/ | Update posts dated 1 Jul 2025 to 13 Mar 2026 | 17 Oct 2026 |
| S14 | Dropbox's AI Principles | Dropbox | https://www.dropbox.com/ai-principles | Last updated Apr 4, 2025 | 17 Oct 2026 |
| S15 | Dash Sub-processor List | Dropbox | https://www.dropbox.com/privacy/subprocessor/dash | Last updated Apr 29, 2026 | 17 Oct 2026 |
| S16 | Dropbox Sub-processor List | Dropbox | https://www.dropbox.com/privacy/subprocessor/dropbox | Last updated Apr 29, 2026 | 17 Oct 2026 |
| S17 | The Dropbox Privacy Policy: frequently asked questions | Dropbox Help Center | https://help.dropbox.com/security/privacy-policy-faq | Updated Apr 8, 2024 | 17 Oct 2026 |
| S18 | Privacy Policy | Dropbox | https://www.dropbox.com/privacy | Posted and effective May 30, 2025 | 17 Oct 2026 |
| S19 | Terms of Service | Dropbox | https://www.dropbox.com/terms | Posted and effective Jan 7, 2025 | 17 Oct 2026 |
| S20 | Terms of Service (from 1 January 2027) | Dropbox | https://www.dropbox.com/terms2026 | Posted Sep 1, 2026; effective Jan 1, 2027 | 17 Oct 2026 |
| S21 | Dropbox Services Agreement | Dropbox | https://www.dropbox.com/business_agreement | Posted and effective Dec 5, 2024 | 17 Oct 2026 |
| S22 | Where is my Dropbox data stored? | Dropbox Help Center | https://help.dropbox.com/security/physical-location-data-storage | Updated Aug 31, 2026 | 17 Oct 2026 |
| S23 | Data transfers between Asia-Pacific and the United States | Dropbox Help Center | https://help.dropbox.com/security/data-transfers-asia-pacific | Last updated Dec 12, 2024 | 17 Oct 2026 |
| S24 | How to manage team security in Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/security/manage-team-security-in-dropbox-dash | Updated Sep 29, 2025 | 17 Oct 2026 |
| S25 | How to manage your team in Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/organize/manage-team-dash | Updated Sep 29, 2025 | 17 Oct 2026 |
| S26 | How to connect Dropbox to Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/integrations/connect-dropbox-to-dash | Updated Dec 3, 2025 | 17 Oct 2026 |
| S27 | How to disconnect and delete Dropbox Dash | Dropbox Help Center | https://help.dropbox.com/installs/delete-dropbox-dash | Updated Mar 6, 2026 | 17 Oct 2026 |
| S28 | How to manage apps for your Dropbox team | Dropbox Help Center | https://help.dropbox.com/integrations/app-integrations | Updated Oct 22, 2025 | 17 Oct 2026 |
| S29 | AI integrations | Dropbox Help Center | https://help.dropbox.com/ai_integrations | No date shown | 17 Oct 2026 |
| S30 | How to connect Dropbox to ChatGPT | Dropbox Help Center | https://help.dropbox.com/integrations/chatGPT-app | Updated Sep 30, 2026 | 17 Oct 2026 |
| S31 | How to connect Dropbox to Claude | Dropbox Help Center | https://help.dropbox.com/integrations/connect-dropbox-to-claude | Updated Sep 17, 2026 | 17 Oct 2026 |
| S32 | How to connect Dropbox to Microsoft Copilot | Dropbox Help Center | https://help.dropbox.com/integrations/copilot-app | Updated Sep 30, 2026 | 17 Oct 2026 |
| S33 | Connect Dropbox to Gemini | Dropbox Help Center | https://help.dropbox.com/integrations/gemini-app | Updated Sep 21, 2026 | 17 Oct 2026 |
| S34 | Using Dropbox Dash in ChatGPT and Claude | Dropbox Help Center | https://help.dropbox.com/integrations/dash-in-chatgpt-and-claude | Updated Sep 17, 2026 | 17 Oct 2026 |
| S35 | How to connect the Dropbox remote MCP server | Dropbox Help Center | https://help.dropbox.com/integrations/connect-dropbox-mcp-server | Updated Sep 30, 2026 | 17 Oct 2026 |
| S36 | How to connect the Dropbox Dash remote MCP server | Dropbox Help Center | https://help.dropbox.com/integrations/set-up-MCP-server | Updated Aug 31, 2026 | 17 Oct 2026 |
| S37 | How to use Dropbox Sign with Dropbox MCP remote server | Dropbox Help Center | https://help.dropbox.com/integrations/dropbox-sign-mcp-remote-server | Updated Sep 30, 2026 | 17 Oct 2026 |
| S38 | How to use the Claude Dropbox integration without losing project context | Dropbox | https://www.dropbox.com/resources/claude-dropbox-integration | Aug 30, 2026 | 17 Oct 2026 |
| S39 | Work seamlessly with Dropbox in Claude | Dropbox Blog | https://blog.dropbox.com/topics/news/work-seamlessly-with-dropbox-in-claude | Published Jun 25, 2026 | 17 Oct 2026 |
| S40 | Move your work forward with new Dropbox apps in ChatGPT | Dropbox Blog | https://blog.dropbox.com/topics/news/move-your-work-forward-with-new-dropbox-apps-in-chatgpt | Apr 16, 2026 | 17 Oct 2026 |
| S41 | The context layer for AI: Bringing trusted Dropbox content into OpenAI workflows | Dropbox Blog | https://blog.dropbox.com/topics/news/trusted-dropbox-content-into-openai-workflows | Jul 12, 2026 | 17 Oct 2026 |
| S42 | Small businesses can move faster with Dropbox in ChatGPT | Dropbox Blog | https://blog.dropbox.com/topics/company/dropbox-chatgpt-small-business-collection | Sep 8, 2026 | 17 Oct 2026 |
| S43 | Dropbox brings trusted project context directly into the ChatGPT Library | Dropbox Blog | https://blog.dropbox.com/topics/company/dropbox-into-chatgpt-library | Sep 10, 2026 | 17 Oct 2026 |
| S44 | Put your Dropbox context to work in Google Gemini | Dropbox Blog | https://blog.dropbox.com/topics/company/bring-dropbox-context-into-google-gemini-experiences | Sep 17, 2026 | 17 Oct 2026 |
| S45 | Dropbox Integration for Google Gemini | Dropbox | https://www.dropbox.com/app-integrations/gemini | No date shown | 17 Oct 2026 |
| S46 | Fall 2025 release: Try the new Dropbox Dash, your context-aware AI teammate | Dropbox Blog | https://blog.dropbox.com/topics/news/fall-2025-release-dropbox-dash-context-aware-ai-teammate | Oct 23, 2025 | 17 Oct 2026 |
| S47 | Dropbox Product Updates | Dropbox | https://www.dropbox.com/product-updates | No date shown (headed "Fall '25 release") | 17 Oct 2026 |
| S48 | Introducing Dropbox Dash, AI-powered universal search, and Dropbox AI | Dropbox Blog | https://blog.dropbox.com/topics/product/introducing-AI-powered-tools | Jun 21, 2023 | 17 Oct 2026 |
| S49 | AI Universal Search & Knowledge Workspace | Dropbox | https://dash.dropbox.com/ai-info-page | No date shown | 17 Oct 2026 |
| S50 | Zapier + Dropbox | Dropbox Help Center | https://help.dropbox.com/integrations/zapier | Updated Aug 13, 2026 | 17 Oct 2026 |
| S51 | Dropbox (connector) | Anthropic | https://claude.com/connectors/dropbox | "Added June 2026" | 17 Oct 2026 |
| S52 | Dropbox (plugin) | Anthropic | https://claude.com/marketplace/plugins/dropbox | No date shown | 17 Oct 2026 |
| S53 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (17 Oct 2026) | 17 Oct 2026 |
| S54 | Use plugins in Claude | Anthropic Help Center | https://support.claude.com/en/articles/13837440-use-plugins-in-claude | "Updated over a week ago" | 17 Oct 2026 |
| S55 | Is my data used for model training? (consumer products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | Mar 16, 2026 | 17 Oct 2026 |
| S56 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | Aug 18, 2026 | 17 Oct 2026 |
| S57 | Dropbox plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/dropbox/ | No date shown | 17 Oct 2026 |
| S58 | ChatGPT plugin listing: Dropbox | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69b31dc2110c8191b8b47dc98fe5a052 | Version 6.0.0; no date shown | 17 Oct 2026 |
| S59 | Dropbox Dash plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/dropbox-dash/ | No date shown | 17 Oct 2026 |
| S60 | ChatGPT plugin listing: Dropbox Dash | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69ca45719b948191999f401a2108740b | Version 2.0.0; no date shown | 17 Oct 2026 |
| S61 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 8 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S62 | Connecting custom MCP servers in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12584461-connecting-custom-mcp-servers-in-chatgpt | "Updated: 12 hours ago" (timestamp 16 Oct 2026, UTC) | 17 Oct 2026 |
| S63 | Dropbox connector overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/dropbox-overview | 24 Nov 2025 (page metadata; updated 25 Sep 2026) | 17 Oct 2026 |
| S64 | Deploy the Dropbox connector | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/dropbox-deployment | 16 Dec 2025 (page metadata) | 17 Oct 2026 |
| S65 | Set up the Dropbox service for Dropbox connector ingestion | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/dropbox-admin-setup | 21 Nov 2025 (page metadata) | 17 Oct 2026 |
| S66 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 30 Sep 2026 (page metadata) | 17 Oct 2026 |
| S67 | Dropbox for Copilot | Microsoft Marketplace | https://marketplace.microsoft.com/en-us/product/wa200012324 | No date shown | 17 Oct 2026 |
| S68 | Copilot Cowork overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/ | 29 Sep 2026 (page metadata) | 17 Oct 2026 |
| S69 | Use plugins with Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugins | 27 Aug 2026 (page metadata) | 17 Oct 2026 |
| S70 | What's new in Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/whats-new | 14 Sep 2026 (page metadata) | 17 Oct 2026 |
| S71 | What Microsoft Copilot Cowork uses and stores (Preview) | Microsoft Support | https://support.microsoft.com/en-us/microsoft-365-copilot/cowork-uses-stores | No date shown | 17 Oct 2026 |
| S72 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy | 9 Jul 2026 (page metadata; updated 8 Oct 2026) | 17 Oct 2026 |
| S73 | Manage files & folders in your Dropbox in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/answer/17211088?hl=en | No date shown | 17 Oct 2026 |
| S74 | Check the availability & requirements of Connected Apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 17 Oct 2026 |
| S75 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S76 | What's new for Gemini Spark | Google Gemini Apps Help | https://support.google.com/gemini/answer/17171264?hl=en | Dated entries; Dropbox entry 7 Jul 2026 | 17 Oct 2026 |
| S77 | Connect your Google apps and third-party data (Gemini Enterprise, Business edition) | Google | https://support.google.com/g/answer/16550932?hl=en | Last updated Oct 15, 2026 | 17 Oct 2026 |
| S78 | Dropbox data store (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/dropbox | Last updated 2026-10-14 UTC | 17 Oct 2026 |
| S79 | What content can I search in Dropbox Dash? | Dropbox Help Center | https://help.dropbox.com/organize/dash-supported-content-types | Updated Jul 24, 2026 | 17 Oct 2026 |
