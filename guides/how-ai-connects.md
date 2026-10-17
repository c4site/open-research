# How AI connects to the tools you already use

Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

Most AI chat tools can now link to other software you use, such as your email or your customer records. The AI can then look things up there, and sometimes make changes for you. [S1][S23][S42][S61]

Each company names these links differently. ChatGPT calls them apps, and now groups them into plugins. Claude and Microsoft say connectors, while Google says Connected Apps. [S1][S2][S23][S41][S61]

Many of these links now run on one open standard, the Model Context Protocol, usually shortened to MCP. [S5][S24][S42][S62][S70]

To connect, you normally sign in to the other service on its own page and approve what the AI may do. The AI can then reach only what your own account can reach, unless the connection uses a shared login. [S3][S23][S42][S63]

At work, an administrator decides which connections are switched on. Administrators can also block risky actions such as sending or deleting. [S6][S23][S42][S63]

OpenAI, Anthropic, Microsoft and Google all say they don't train their AI on business customers' work data by default. Personal plans each have their own rules, and data fetched through a connection has its own rules again. [S9][S37][S47][S66][S1][S36][S11][S60]

Anything the AI sends to a connected service is then handled under that service's terms. That can mean storage in another country. [S1][S6][S17][S23][S60]

OpenAI and Anthropic warn that a connected service can carry hidden instructions aimed at the AI. Google says it doesn't control or secure custom connected apps. All three advise connecting only services you trust. [S14][S24][S62]

Automation services like Zapier, Make, n8n and Power Automate can sit in the middle, so one connection reaches many apps. [S80][S88][S96][S55]

This area changes monthly. On 15 October 2026, Zapier's ChatGPT guide still described a developer mode step that OpenAI's newer page says is no longer needed. Check the date on any setup guide before you follow it. [S5][S83]

## The words you'll see

**Connector.** A link between an AI tool and another app or service, so the AI can find information there and act for you. [S31] Microsoft uses the same word for links that let its tools use another service's actions and triggers. [S55]

**App, Connected App and plugin.** In ChatGPT, an app links ChatGPT to an outside service such as Google Drive, and a plugin is a bundle that can hold apps, written instructions called skills, or both. [S1][S2] Google calls its links Connected Apps. [S61]

**MCP server.** A program that gives an AI tool a set of actions and information from one service, using MCP. [S71] It can run on your own computer (local) or on the internet (remote). [S71]

**Signing in with another account (OAuth).** You sign in on the other service's own page and approve the access it asks for. The AI then gets a pass, called a token, to act for you without ever seeing your password. [S24][S58]

**API key.** A long secret code that software sends to prove which account a request comes from. Zapier says to treat its similar connection token like a password, and Anthropic notes that a key shared by a team gives everyone that key's access. [S81][S24][S69]

**Admin consent.** An administrator approves an app's access for everyone in the organisation in one step. Microsoft calls this a sensitive operation and says not to grant it unless you trust the app and its publisher. [S57]

**Permission or scope.** The specific access an app asks for, such as reading your files. Microsoft describes scopes as permissions that say what an app may do on a user's behalf. [S56]

**Read-only and read-write.** Read tools look things up, while write tools create, change, send or delete. OpenAI, Anthropic and Microsoft let administrators allow or block these two groups separately. [S4][S6][S23][S42]

**Agent.** An AI set up to work through several steps on its own toward a goal, picking which tools to use as it goes. [S94][S90] Microsoft says agents can take actions like sending emails or updating records. [S44]

**Prompt injection.** Hidden instructions planted in something the AI reads, such as a web page, a file or a tool's reply, meant to make it act against your wishes. [S21][S24] OpenAI says it's the most common risk behind its "Elevated risk" labels. [S22]

**Desktop extension.** Anthropic's one-click package for running an MCP server on your own computer inside the Claude desktop app. [S25]

## ChatGPT

### What it's called now

- OpenAI's help centre calls these links apps. Its examples are Google Drive and Slack. [S1]
- The word connectors still appears in places, including that page's answer about training. [S1]
- Plugins are a newer layer. A plugin can include skills, connected apps, app templates for administrators and extensions. [S2]
- Very old versions of the iOS and Android apps may say Apps where newer versions say Plugins. [S1]
- Some apps show interactive content in the chat, such as maps or cards. [S1]
- OpenAI's release notes date the switch to 18 December 2025, when connectors began appearing as apps in a new app directory. On 9 July 2026 a Plugin Directory replaced that App Directory, and existing app connections carried on. [S98]

### Which plans have it

OpenAI says availability depends on the app, your plan, region, workspace, role, model and where you use ChatGPT. [S1] Its pricing pages list these rows. The Free to Pro columns come from the individual pricing page, and the Business and Enterprise columns from the business pricing page. [S7][S8]

| OpenAI's label | Free | Go | Plus | Pro | Business | Enterprise | Source |
|---|---|---|---|---|---|---|---|
| Discover & use Plugins | Yes | Yes | Yes | Yes | Yes | Yes | [S7][S8] |
| Interactive apps | Yes | Yes | Yes | Yes | Yes | Yes | [S7][S8] |
| Apps connecting to internal tools | No | No | Yes | Yes | Yes | Yes | [S7][S8] |
| Apps for deep research | Limited | Limited | Yes | Yes | Yes | Yes | [S7][S8] |
| Developer mode (beta) | No | No | Yes | Yes | Yes | Yes | [S7][S8] |
| Company knowledge | No | No | No | No | Yes | Yes | [S7][S8] |
| Workspace agents | No | No | No | No | Yes | Yes | [S7][S8] |
| Connector registry | No | No | No | No | No | Yes | [S7][S8] |

- Edu isn't on either pricing page. OpenAI's help pages group Edu with Enterprise for apps and admin controls. [S5][S6]
- Agent mode is listed for Plus, Pro, Business, Enterprise and Edu. OpenAI says Free doesn't have it. Go isn't named. [S14]

### Connecting an app

1. Open Settings, select Plugins, then select the app or the plugin that includes it. [S3]
2. Select Install plugin if you see it. This may start the sign-in. [S3]
3. Select Connect if asked, and sign in to the account that already holds the information you want. [S3]
4. Read the services and permissions on the other company's screen, then approve. [S3]
5. In a chat, type @ and pick the app, or select + and choose it. Then say what you want. [S1][S3]

- Some apps need no sign-in, or use a connection your administrator set up. [S3]
- Connecting a personal account won't reach files that only your work account can see. [S3]
- Google's screen may ask you to choose Select all. To connect fewer Google apps, choose Select fewer apps in ChatGPT. [S3]
- To disconnect, go to Settings > Plugins, select the app, then Disconnect. [S3]

### When ChatGPT asks before acting

- Always ask: ChatGPT asks before reading or changing anything. [S4]
- Allow read actions: it reads without asking, and asks before changes. [S4]
- Allow low-risk actions: low-risk actions run automatically, and higher-risk ones may need confirming or be refused. [S4]
- Allow all actions: no further prompts. OpenAI says this carries elevated risk, and the account-wide and workspace-wide settings don't offer it. [S4]
- If you haven't changed your own Plugins settings, OpenAI's release notes say the default is Allow low-risk actions. [S98]
- OpenAI's examples of actions that may need extra review include sending an email, deleting a file, changing sharing settings and making a purchase. [S4]
- An approval card may offer Deny, Allow once, Allow low-risk actions or Always allow. Always allow is offered only to eligible personal accounts. [S4]
- Changing these settings doesn't cancel the access an app already has. To stop an app, disconnect it. [S4]

### What workspace administrators control

- In Business, apps are on by default and administrators can change that. [S6]
- In Enterprise and Edu, new workspaces start with a selected set of apps, and new plugins and apps are generally off until an administrator reviews them. [S6]
- Enterprise and Edu administrators can choose which roles may use which apps. [S6]
- Administrators switch read actions and write actions on separately. For actions an app adds later, they choose Enable all new actions, Only enable new read actions or Disable new actions. [S6]
- The workspace's default approval level sits under Workspace settings > General > Plugin permissions. [S6]
- Manage domains limits which email domains members can connect to an app. [S6]
- Enterprise organisations can ask OpenAI Support to block work accounts on their verified domain from being connected to personal ChatGPT accounts. Covered apps include Gmail, Google Drive, Outlook Email, SharePoint, Slack and Teams. [S6][S1]
- Some Outlook, Teams and SharePoint actions need a Microsoft Entra administrator to grant organisation-wide consent. Microsoft's screen has no per-permission boxes, so Accept grants the whole request. [S6]
- App calls are logged, and Enterprise and Edu customers can retrieve conversations, including those using apps, through the Compliance API. [S1][S5][S6]
- Business administrators don't automatically get access to members' ordinary private conversations. [S6]
- Administrators can switch off the thumbs feedback buttons under Workspace settings > Allow response feedback. [S9]
- Lockdown Mode is an optional setting that limits outbound network requests to reduce data theft through prompt injection. It turns off deep research and agent mode. On personal and self-serve Business accounts, it also blocks live access to outside services and connector write actions where they conflict with its protections. [S21]

### Custom MCP servers and developer mode

- Custom MCP server connections and full MCP support are for Business, Enterprise and Edu, on ChatGPT for the web. [S5]
- In Business, only admins and owners can create and publish them. In Enterprise and Edu, admins can give selected members the "Create plugins with MCPs" permission, and only admins and owners can publish. [S5][S2]
- That permission is off by default for Enterprise. [S2]
- In the current Plugins screen you don't turn on Developer Mode first. You tick a risk warning for each server instead. [S5]
- Pro users can build with OpenAI's Apps SDK and connect custom MCP servers that only read and fetch. Full MCP, including write actions, is for Business, Enterprise and Edu. [S5]
- ChatGPT connects to remote servers. A server on a private network can be reached through OpenAI's Secure MCP Tunnel. [S5]
- Separately, a plugin can include local MCP apps that run in the ChatGPT desktop app. [S2]
- Custom MCP connections are web only, and OpenAI says there are no geographic restrictions. [S5]
- After approval, ChatGPT uses a frozen copy of the server's tool list. Later changes wait for an administrator, and administrators aren't alerted when a tool starts failing. [S5]
- OpenAI says custom apps aren't verified by OpenAI, and the workspace is responsible for vetting them. [S6][S5]
- If the server's sign-in isn't set up to renew itself, people may have to sign in again later. [S5]

### Deep research, agent mode and ChatGPT Work

- Deep research can use connected apps that support it, and uses their read actions only. [S13][S5]
- Agent mode can use apps as data sources. OpenAI asks for extra caution, because an agent with access to email or files is exposed to prompt injection. [S14]
- OpenAI's tips for agent mode: enable only the apps the task needs, and avoid open-ended requests like "Check my email and handle everything". [S14]
- Agent mode asks you to confirm high-impact actions and monitors for prompt injection. OpenAI says these measures don't eliminate all risk. [S14]
- In Enterprise workspaces, agent mode is off until an owner turns it on, and it can only use apps the workspace has enabled. [S14]
- ChatGPT Work is OpenAI's agent for longer, multi-step jobs, and it can use connected apps. [S15]
- Workspace agents, for Business and Enterprise, are shared agents that builders can give apps and custom MCP servers. Each agent's builder decides which app actions need a user's approval. [S16][S6]
- Eligible users can set a task to run when a connected app receives a matching event, such as a new Gmail message. [S1]

### Memory, and what ChatGPT shares with apps

- With Memory on, ChatGPT may remember information it read through an app, unless the app blocks that. [S1]
- It also works the other way. An app you enable may receive relevant parts of your conversation and, with Memory on, your saved memories. [S1]
- Apps may also see your IP address, device and browser type, language and approximate location. [S1]
- What you share with an app is handled under that app's terms, which ChatGPT shows before you enable it. [S1]
- Disconnecting an app doesn't delete past chats, saved files or memories. [S3]
- A temporary chat can be started without memories, custom instructions or plugins. [S10][S12]

### Australia

- Australia is on OpenAI's list of supported countries. [S19]
- Agent mode is offered in all supported countries. [S14]
- Eligible API customers and new Enterprise and Edu customers can have their content stored in Australia. [S17][S8]
- OpenAI offers in-region AI processing (it calls this inference residency) only for Europe, the United States and the UAE. Australia isn't on that list. [S17]
- Data sent to apps or MCP servers can be stored outside the chosen region. [S17][S6]
- Administrator-managed Google Drive sync works for workspaces set to Australian data residency. [S18]

## Claude

### What Anthropic calls it

- Connectors let Claude reach your apps, retrieve data and take actions there. [S23]
- Claude inherits each person's permissions. If you can't open a file in the original service, Claude can't reach it either. [S23]
- A connector that uses a shared credential reaches whatever that credential can reach. [S23]
- Remote connectors work wherever you use Claude. Desktop extensions run on your own computer, in Claude Desktop and Claude Code only. [S26]
- Plugins can bundle remote or local MCP servers. [S26]
- Some connectors are interactive and show things like dashboards or task boards inside the chat. [S23][S24]

### The Connectors Directory

- One directory serves Claude on the web, desktop and mobile, plus Claude Code and Cowork. [S33]
- Verified means Anthropic tested the connector's tools for quality and compatibility. [S32]
- Community means Anthropic screened it before listing but didn't review it in depth. [S32]
- Custom means you added it yourself and Anthropic hasn't reviewed it. [S32]
- Anthropic says verification isn't a security audit, and the developer can change the tools after review. [S32]
- Ranking is based on usage. Anthropic says Claude takes no payment to suggest an app. [S33][S29]
- On Team plans, members who can't enable connectors see a Request button that notifies the Owners. [S33]
- If a provider moves its server address, your old connection keeps working but shows as Custom. [S33]

### Which plans have it

- Directory connectors are available to all users of the Claude apps. [S23]
- The pricing page lists connectors and desktop extensions for Free, Pro and both Max tiers. [S35]
- Custom connectors work on Free, Pro, Max, Team and Enterprise. Free accounts can add one. [S23][S24][S34]
- On Team and Enterprise, an Owner enables a connector first. Each member then signs in with their own account, unless the connector uses a shared credential. [S23][S24]
- Installing connectors on mobile is in beta. [S23]

### Connecting a connector

1. Go to Customize > Connectors and select Discover. [S31]
2. Search for the service or browse the categories, then open its page. [S31]
3. Select Connect to Claude. Some connectors first ask for a server address or region. [S31]
4. Sign in on the service's page, review the access Claude asks for, and approve. [S31]
5. Back on the Connectors page, it shows under Your connectors as Connected. [S31]

- To use it, select + in the message box, then Connectors, and switch it on for that chat. [S31]
- Claude may ask before using a tool. Allow once runs it this time, and Always allow skips the question for that tool from then on. [S31]
- For each connector you can set groups of tools to Always allow, Needs approval or Blocked. [S31]
- Anthropic's pages use slightly different menu names. Most say Customize > Connectors, and one says Settings > Connectors. [S31][S26]
- With 10 or more connectors, Anthropic suggests the On demand tool access mode so they don't crowd the conversation. [S23][S30]
- Claude can suggest a connected app on its own. Before it books or buys anything, it checks with you. [S29]

### Custom connectors (remote MCP)

1. Go to Customize > Connectors and click Add custom connector. [S34]
2. Enter the server's https address. [S34]
3. Choose how people sign in: Sign in now, Sign in when needed or No sign-in. [S34]
4. If you chose a sign-in option, choose how Claude identifies itself. Anthropic recommends Use Claude's published identity. [S34]
5. Put any fixed credential, such as an API key, under Request headers. This is in beta for a limited set of organisations. [S34]
6. Click Add, then connect as you would with a directory connector. [S34][S24]

- Claude reaches custom connectors from Anthropic's cloud, even in the desktop app, so the server must be reachable from the public internet. [S24]
- A server behind a firewall needs Anthropic's IP addresses allowed through, or an MCP tunnel. [S24][S34]
- Anthropic reviews each custom header name before Claude will send it to a third-party server. [S34]

### Desktop extensions (local MCP)

1. In Claude Desktop, go to Settings > Extensions. [S25]
2. Click Browse extensions, choose an Anthropic-reviewed extension, and click Install. [S25]
3. Fill in any settings it needs, such as an API key. [S25]

- Extensions from outside the directory install from a .mcpb file, under Advanced settings and then Install Extension. [S25]
- Settings marked sensitive are encrypted in your computer's own secure storage, such as Credential Manager on Windows. [S25]
- Directory extensions update automatically. Privately shared ones must be updated by hand. [S25]
- Claude's Research feature can't use tools from local MCP servers. [S24]

### What Team and Enterprise owners control

- Enable a connector for the organisation under Organization settings > Connectors > Browse connectors > Add to your team. [S23]
- Limit actions for everyone, such as letting Claude search and summarise email while blocking sending. Each tool group can be Always allow, Needs approval or Blocked, and members can't override it. [S23]
- Add custom connectors. On Team only Owners and Primary Owners can, and on Enterprise so can custom roles with library management rights. [S24]
- Enterprise-managed auth: authorise a connector once through the organisation's identity provider, then choose which roles get it and which permissions it may request. Okta is supported at launch. [S27]
- Enterprise only: stop work accounts on the company's verified domains being connected from personal Claude accounts. Covered services include Gmail, Google Drive, HubSpot, Canva, Microsoft 365 and Slack. [S28]
- Desktop extensions: switch public extensions on or off, keep an allowlist and upload the organisation's own. Device-level policies override the in-app settings. [S25]
- Switch off interactive connector tools. [S24]
- Switch off the thumbs feedback buttons under Organization settings > Data and Privacy. [S37]
- On Team and Enterprise, connectors only work in private projects, and chats with synced content can't be shared. [S23]

### Anthropic's warnings

- Connecting a service lets Claude read and possibly change data there, within your permissions. Anthropic says to connect only services you trust and need. [S23]
- Custom connectors reach services Anthropic hasn't verified. [S24]
- Malicious MCP servers may hide instructions meant to make Claude do things you didn't intend. Claude has protections, but Anthropic asks you to watch what tools receive and return. [S24]
- Developers can change how a tool behaves after you connect it. [S24][S32]
- Anthropic says to use Always allow only for tools you trust to run unsupervised. [S24]
- During Research, Claude can call connector tools without asking each time. Anthropic suggests switching off write tools first. [S24]
- Malicious servers can be reported through Anthropic's vulnerability disclosure program. [S24]

### Training

- Consumer plans: Anthropic's training data doesn't include raw content from connectors, including local and remote MCP servers, unless it's copied into the conversation. [S36]
- Anthropic's page on connected apps says data from a connected app isn't used to train Claude's models, and the app can't see your other conversations. [S29]
- Work plans and the API: not used for training by default. [S37]

### Australia

- Australia is on Anthropic's Supported Regions Policy, effective 12 May 2026. [S38]
- Connected services run on their own infrastructure under their own terms, which may be outside the United States. Settings that keep Claude's own processing in the US don't change where those services run. [S23]
- Anthropic's regional compliance page covers Claude through AWS Bedrock, Google Vertex and Microsoft Foundry, with an Asia-Pacific row. It doesn't cover connectors in the Claude apps. [S39]

## Microsoft Copilot

Another researcher covers Microsoft 365 in depth. This is the short version.

### Copilot Chat and the paid licence

- Copilot Chat comes with eligible Microsoft 365 licences. It's mainly grounded on the web, plus files you upload or paste and some in-app context. [S40]
- In Outlook, Copilot Chat can also search your mail, calendar, meetings and chats without the paid licence. [S40]
- The paid Microsoft 365 Copilot licence adds reasoning across your organisation's emails, meetings, chats, documents and sites, and fuller access to agents. [S40]
- Both respect existing Microsoft 365 permissions. [S40]

### Copilot connectors

- Copilot connectors bring outside data into Copilot. Synced connectors copy and index it into Microsoft Graph. Federated connectors fetch it live through MCP and store nothing in Microsoft 365. [S41][S43]
- Microsoft offers more than 100 prebuilt synced connectors. [S41]
- Federated connectors currently listed include Xero, HubSpot, Canva, Gmail, Google Calendar, Notion, Asana, Box, monday.com and Make. [S42]
- They work in Copilot Chat, agents, Cowork, Word, Excel, PowerPoint, Outlook and the Researcher agent. [S42]
- To connect one, go to Copilot Chat, select the ... menu, then Settings > Sources. Find the service, select Connect and sign in. [S42]
- Copilot sees only what your account can see, and can change only what you're allowed to change. [S42]
- Microsoft's pages also use the name Microsoft Graph connectors in places. The API is the "Microsoft Graph connectors API", and the privacy page refers to "Microsoft Graph connectors". [S41][S47]

### Write actions through connectors

- Federated connectors have been read-only. Microsoft says write, update and delete actions begin rolling out in early October 2026. [S41][S42]
- Write tools ask for approval by default. The choices are Allow once, Allow for conversation, Always allow and Cancel. [S42]
- If a publisher adds or changes a write tool, it goes back to needing approval. [S42]
- The Researcher agent stays read-only. [S42]

### Agents and Copilot Studio

- Agents are specialised assistants that add knowledge and actions to Copilot. Declarative agents use Copilot's own model, and custom engine agents bring their own. [S44]
- Copilot Studio agents can use tools and resources from MCP servers. Microsoft says you're responsible for the tools you use from a non-Microsoft server. [S45]
- When Copilot calls an agent, it sends a query built from your prompt, your Copilot history and Microsoft 365 data you can access. [S47]

### Admin controls

- Microsoft-published federated connectors are on by default. Partner connectors need an administrator's approval. [S42]
- Administrators manage them in the Microsoft 365 admin center under Copilot connectors > Your connections, and can roll a connector out to chosen groups first. [S42]
- A setting called Allowed agent types can keep federated connectors off by default, including future ones. [S42]
- Microsoft asks administrators to check a connector's capabilities, privacy terms and third-party agreements before enabling one that has write tools. [S42]
- The Agent Registry (Agents > All agents) lets administrators install, block or delete agents. Installing one includes a Grant admin consent step. [S46]
- Microsoft says users can only use agents their administrator allows, and tells administrators to check each agent's privacy statement and terms. [S47]

### Australia

- Copilot's AI calls go to the nearest data centres but can go to other regions when busy. Outside the EU, queries may be processed in the US, the EU or elsewhere. [S47]
- Microsoft expects to offer local processing of Microsoft 365 Copilot interactions in Australia by the end of 2026. [S48]

## Gemini

Another researcher covers Google Workspace in depth. This is the short version.

### Personal accounts: Connected Apps

- Gemini can connect to Google apps and third-party services, and can act in them with your permission. [S61]
- You must be signed in, and Keep Activity must be on. With it off, Connected Apps don't work on gemini.google.com or iOS devices, and on Android only Phone, Messages, WhatsApp and Device assistance still work. [S61][S60]
- To connect, open gemini.google.com, select Customize in the sidebar, then Connectors at the top, then Add. In a chat, type @ to pick an app. [S61]
- Google's pages say Connected Apps. Some Google text also uses the word extension, such as "the Workspace extension". [S61][S66]

### Custom apps through MCP

- Personal accounts can add a custom app by entering an MCP server's address. [S62]
- You must be 18 or over and in the US, with Keep Activity on. For now, the feature is English-only and not available to work and school accounts. [S62]
- Google says it doesn't control, monitor or secure these servers. Once data reaches a custom app, that app's privacy practices apply. [S62]
- Gemini currently asks you to confirm every write action, but Google notes Gemini can make mistakes. [S62]
- Google warns custom apps may ask for more data than a task needs. Gemini may also share chat content and data from your other connected sources with them. [S62]
- This page gives a different menu path from the main Connected Apps page: Settings > Connected Apps > Custom apps. [S62][S61]

### Work and school accounts

- Work accounts need a qualifying Workspace edition, Keep Activity on (set by the administrator), and an administrator who has enabled connected apps. [S63]
- Type @ and choose the app. Google lists things Gemini can't do there, such as drafting or deleting Gmail messages. [S63]
- The Gemini app is a core service in most Workspace editions, including Business Starter, Business Standard and Business Plus. [S65]
- In those editions, content isn't human-reviewed or used for AI training outside your organisation's domain without permission. [S65][S66]
- Google's Workspace privacy hub says third-party apps used with Gemini come under different terms. [S66]

### Gemini Enterprise

- Gemini Enterprise is a separate Google Cloud product for company-wide search, an assistant and agents. It has prebuilt connectors for tools such as Confluence, Jira, SharePoint and ServiceNow. [S67]
- Its connectors either copy data into Gemini Enterprise's index or fetch it live, which Google calls federation. [S68]
- With federation, your query goes to the third-party system, may include parts of your conversation, and can be linked to you. After that, the third party's terms apply. [S68]
- Data stores can be placed in global, US or EU regions. [S68]

## MCP, in plain words

### What it is

- MCP is an open standard for connecting AI apps to outside systems. [S70]
- MCP's own website compares it to a USB-C port: one standard plug in place of a different cable for each device. [S70]
- Anthropic created it. [S24]
- The MCP site says the project is now established as "a Series of LF Projects, LLC". Seats in its technical governance belong to individuals, and no company has reserved seats. [S77]
- The current specification is the version dated 2026-07-28. [S72]
- Claude, ChatGPT, Visual Studio Code and Cursor are among the apps that support it. [S70]
- Microsoft's federated connectors and Copilot Studio use it, as do Gemini's custom apps. [S42][S45][S62]
- Zapier, Make and n8n each offer MCP connections. [S80][S88][S95]

### The pieces

- Host: the AI app you use, such as Claude Desktop. [S71]
- Client: the part inside the host that holds one connection to one server. [S71]
- Server: the program that offers the tools. [S71]
- A server can offer tools (actions the AI can take), resources (information it can read) and prompts (ready-made templates). [S72]

### Local and remote

- A local server runs on your computer and talks to the AI app directly. It usually serves one app. [S71]
- A remote server runs on the internet and usually serves many people. [S71]
- Remote servers can use bearer tokens, API keys or custom headers to check who's calling. MCP recommends OAuth for sign-in. [S71]
- A remote server needs no installing on each device, which suits AI apps used in a browser. [S74]
- MCP's security guide says apps should warn that a local server runs with the same privileges as the AI app itself. [S73]
- MCP's local-server guide notes that its example file server can do any file operation you can do yourself. [S75]

### Who makes servers

- Anyone can. The official MCP Registry lists publicly reachable servers, and checks that a publisher owns the GitHub account or web domain in the server's name. [S76]
- The registry is in preview and may have breaking changes or data resets. It leaves security scanning to package registries such as npm. [S76]
- The MCP project's own reference servers are teaching examples. The project says they aren't production-ready. [S78]
- Companies run their own servers too, such as Zapier's and Make's. [S80][S88]
- Anthropic's directory doesn't ask for proof of domain ownership. That requirement belongs to the open MCP Registry. [S33]

### What the specification says about safety

- Users must agree to, and understand, all data access and actions. [S72]
- AI apps must get explicit consent before running any tool. [S72]
- Tool descriptions should be treated as untrusted unless they come from a trusted server. [S72]
- MCP can't enforce these rules itself. Each app has to build them in. [S72]
- MCP's security guide warns that a malicious local server can run harmful commands or send data off your computer. It says one-click installs must show the exact command and ask for approval. [S73]
- The guide also warns against granting broad permissions up front, because a stolen token then reaches more. [S73]

## Automation tools as the glue

An automation service already holds sign-ins to many apps. Connect an AI to it once, and the AI can use those apps through it. [S80][S89] Our reading: this saves setting up each app separately, and it adds one more company that handles your data.

### Zapier

- Zapier MCP lets AI tools such as Claude, ChatGPT and Cursor take actions in apps connected to your Zapier account. [S79][S80]
- Zapier holds the app credentials, so the AI tool never handles a third-party key. [S81]
- Zapier says its connection works on every Claude plan, including Free. On Claude Team and Enterprise, an Owner has to enable Zapier first. [S84]
- Zapier's ChatGPT guide covers two routes: signing in to a Zapier app your workspace has already added, or creating your own plugin with Zapier's server address. [S83]
- It's included in every Zapier plan. Each successful tool call uses two tasks from your plan's allowance. [S79][S82]
- It's on by default for every account. Workspace administrators can restrict it, and app and action restrictions apply account-wide. [S82]
- Zapier stores customer data in AWS US-East-1 in the United States, unless otherwise agreed. [S82]
- Enterprise customers are opted out of AI model training by default. The page doesn't say what applies to other plans. [S82]
- Zapier Agents is Zapier's own product for AI agents that work across apps. [S86][S85]
- The old AI Actions addresses now redirect to Zapier MCP. That suggests AI Actions has been folded into Zapier MCP, but we found no page that says so. [S87]

### Make

- Make's MCP server lets an AI tool run your Make scenarios (automated workflows) and manage your Make account. [S88][S90]
- You connect with OAuth at mcp.make.com, and choose an organisation and permission scopes on the consent screen. [S89]
- The "Run your scenarios" scope gives access to every on-demand and active scenario in the organisation. [S89]
- Scenario run tools are on all plans. Management tools need a paid plan. [S88]
- MCP toolboxes are separate servers holding only the scenarios you pick, each marked Read only or Read & write. [S92][S91]
- Make AI Agent (New) has been in open beta since 2 February 2026. Its tools can include MCP server tools. [S90]
- Make suggests giving agents tasks you'd trust an intern with, and keeping them away from sensitive data and high-stakes decisions. [S90]
- Make's data zones are US1, US2, EU1 and EU2. Some features send requests to the US whatever zone you choose. [S93]

### n8n

- The AI Agent node connects a chat model to at least one tool, and the agent decides which tools to call. [S94]
- The MCP Client Tool node lets n8n agents use an outside MCP server. You choose which of its tools to expose. [S96]
- The MCP Server Trigger node turns n8n workflows into tools that other AI apps can call. Its authentication can be None, Bearer or Header. [S95]
- n8n can be self-hosted on your own infrastructure. [S97] Our reading: that lets an organisation choose where it runs. The pages we read don't mention Australian hosting.

### Power Automate

- Power Automate builds automated workflows between apps and services. [S59]
- It uses connectors that expose actions and triggers. Microsoft says all its connectors are agent-ready. [S54]
- Copilot in Power Automate lets you build a flow by describing it in plain language. [S52]
- Copilot in Power Automate is on by default in regions with GPUs, and Microsoft lists Australia as one. [S52]
- In Copilot Studio, agent flows are fixed, rule-based workflows that agents can call. They use Copilot Studio capacity. [S53]
- Microsoft's connector reference now has a section for MCP connectors. [S55]

## Your data when AI is connected

### The take-home training table, re-checked 15 October 2026

| Plan | What the take-home sheet relies on | Still holds? | What the vendor says now | Source |
|---|---|---|---|---|
| ChatGPT Free, Plus, Pro | May train on content. Opt out under Data controls. A thumbs rating overrides the opt-out. | Yes. Consider adding Go. | OpenAI may train on your content unless you turn off "Improve the model for everyone" (Settings > Data controls) or opt out in the Privacy Portal. Thumbs feedback can send the whole conversation for training even after opting out. The pricing page shows the same opt-out for Go. Page updated 12 Oct 2026 UTC (13 Oct in Perth). | [S9][S10][S7] |
| ChatGPT Business, Enterprise, Edu, API | Not trained on by default | Yes | Not used to improve models by default. For Business, Enterprise and Edu, thumbs feedback doesn't change that. The same applies to data from apps. | [S9][S20][S6] |
| Claude Free, Pro, Max | Trains only if Model Improvement is on | Yes, with a nuance | Chats are used if you allow it, if a chat is flagged for safety review, or if you opt in to a programme such as Trusted Tester. Raw connector content is excluded. Thumbs feedback keeps the whole conversation for up to 5 years and may be used for training. Page still dated 16 Mar 2026. | [S36] |
| Claude for Work, API | Not trained on by default, unless feedback is reported or you opt in | Yes | Unchanged. Page still dated 18 Aug 2026. Owners can switch off the feedback buttons. | [S37] |
| Gemini, personal | Keep Activity on: trains, with some human review. Off: kept 72 hours, no training unless feedback is sent | Yes | Unchanged. Page dated 13 Oct 2026. With Keep Activity off, most Connected Apps don't work. | [S60][S61] |
| Microsoft Copilot, work | No foundation-model training. Stored with your M365 data. Processing can leave your region. | Yes | Unchanged. Page updated 8 Oct 2026. Local processing in Australia is expected by the end of 2026. | [S47][S48] |
| Copilot, personal | Trains unless you opt out; kept 18 months. Where the control sits in the new app (18 Aug) is unconfirmed | **Changed** | For the updated Copilot app (from 18 Aug 2026), Microsoft says prompts, responses and file contents "aren't used to train foundation models". The new privacy controls page lists no training switch. The old FAQ, with opt-out training and 18-month storage, now says it applies only to the older app. We found no storage period for the new app. | [S50][S51][S49] |

The one-pager's line "kept or used to train, depending on tool and settings" still holds. [S9][S36][S60][S50]

### Rules for data fetched through a connection

| Vendor and plan | What the vendor says about data fetched through a connection | Source |
|---|---|---|
| ChatGPT Free, Go, Plus, Pro | May be used for training if "Improve the model for everyone" is on. | [S1] |
| ChatGPT with Google apps, any plan | OpenAI doesn't train its general models on data from connected Google apps. The exceptions are feedback, content you paste in, and content included in a reply. | [S11] |
| ChatGPT Business, Enterprise, Edu | Not used for training by default. | [S6][S20] |
| Claude, consumer plans | Raw connector content, including from local and remote MCP servers, is left out of training and feedback data unless it's copied into the chat. | [S36][S29] |
| Claude, work plans and API | Not used for training by default. Feedback data leaves out raw connector content. | [S37] |
| Gemini, personal | Gemini saves and uses Connected Apps information under its privacy notice, including to improve Gemini. Feedback can include connected-app content. We found no carve-out like OpenAI's or Anthropic's. | [S60] |
| Gemini, Workspace editions | Not human-reviewed or used for training outside your domain without permission. Third-party apps come under different terms. | [S65][S66] |
| Microsoft 365 Copilot, work | Prompts, responses and data accessed through Microsoft Graph aren't used to train foundation models. Agents have their own privacy statements. | [S47] |
| Zapier MCP, Enterprise | Opted out of AI model training by default. | [S82] |

### What the AI sends to the connected service

- ChatGPT: relevant conversation context, saved memories if Memory is on, your IP address and approximate location. [S1]
- Claude: Anthropic says a connected app can't see your other conversations. [S29]
- Gemini: chat content, device and preference details, location, and content from your Connected Apps. Third-party apps then use it under their own policies. [S60]
- Microsoft 365 Copilot agents: a query built from your prompt, your Copilot history and Microsoft 365 data you can access. [S47]
- Microsoft write actions: Copilot sends the connector what it needs to complete the action, and nothing is sent until you approve. [S42]
- Gemini Enterprise federation: your query, possibly including parts of your conversation, goes to each enabled third-party system and can be linked to you. [S68]

### Where your data sits, for Australian organisations

| Service | What the vendor documents | Source |
|---|---|---|
| ChatGPT Enterprise, Edu and API | Content can be stored at rest in Australia for eligible customers. In-region AI processing isn't offered for Australia. Data sent through apps and MCP may sit elsewhere. | [S17] |
| Claude apps | We found no Australian storage option. Connected services may operate outside the US. | [S23][S39] |
| Microsoft 365 Copilot | Queries may be processed in the US, the EU or elsewhere. Local processing in Australia is expected by the end of 2026. | [S47][S48] |
| Copilot in Power Automate | Australia is listed as a region with GPUs, where Copilot is on by default. Our reading: requests from Australian environments don't rely on cross-region data sharing. | [S52] |
| Gemini Enterprise | Data store regions are global, US or EU. | [S68] |
| Zapier MCP | Stored in AWS US-East-1 unless otherwise agreed. | [S82] |
| Make | Data zones are US1, US2, EU1 and EU2. | [S93] |
| n8n | Can be self-hosted on your own infrastructure. | [S97] |

## What to watch for, whichever AI you use

- **Work data in personal accounts.** OpenAI and Anthropic both offer Enterprise settings that stop work accounts being connected to personal AI accounts. [S6][S28] Anthropic's example: without the setting, someone could connect their work Gmail to a personal Claude account and move company information outside the organisation's controls. [S28]
- **Hidden instructions.** A web page, a file or a tool's reply can carry instructions meant for the AI. [S21][S24][S14] OpenAI's Lockdown Mode limits what can be sent out, but OpenAI says it doesn't stop injected text affecting answers. [S21]
- **Standing approvals.** Always allow and Allow all actions remove a check. OpenAI labels Allow all actions as elevated risk, and Anthropic says to use Always allow only for tools you trust unsupervised. [S4][S24]
- **Research modes.** Claude's Research can call connector tools without asking each time. [S24] ChatGPT's deep research and Microsoft's Researcher agent only read. [S13][S42]
- **Shared keys.** A connector set up with one API key gives everyone who uses it that key's access. Anthropic suggests a key limited to what members should reach. [S24]
- **Tools that change after approval.** MCP server developers can change their tools at any time. [S24][S32] ChatGPT keeps a frozen copy until an administrator reviews changes. [S5] Copilot Studio picks up server changes automatically. [S45] Microsoft puts changed write tools back to Needs approval. [S42]
- **Badges and labels.** OpenAI says its Verified badge doesn't replace your organisation's own privacy, security or vendor review. [S2] Anthropic says its Verified label isn't a security audit. [S32]
- **Disconnecting.** Disconnecting stops future access. It doesn't delete past chats, memories, or data the other service has already received. [S3][S60]
- **All-or-nothing consent screens.** Microsoft Entra's consent screen for ChatGPT's Microsoft apps has no per-permission boxes. [S6] Microsoft says not to grant organisation-wide consent unless you trust the app and its publisher. [S57]
- **Data leaving the region.** Residency promises cover the AI vendor's own storage. Connected services keep their own terms and locations. [S17][S23][S68]
- **Work that runs while you're away.** ChatGPT tasks can run when a connected app receives an event, and workspace agents can run on a schedule. Actions needing approval pause until someone reviews them. [S1][S16]
- **Costs.** App use counts toward ChatGPT plan limits. [S1] Each Zapier MCP tool call uses two tasks. [S82] Agent flows use Copilot Studio capacity. [S53]
- **Guides that go stale.** Menu names differ between a vendor's own pages, and third-party guides lag behind. [S31][S26][S61][S62][S5][S83]

## Announced changes

- Microsoft: write, update and delete actions through federated Copilot connectors "begin rolling out in early October 2026". [S42][S41]
- Microsoft: a Tools list for each connector in the admin center is marked "Coming soon". [S42]
- Microsoft: the Allowed agent types setting replaces a tenant-wide PowerShell switch for federated connectors. The old switch stops being honoured after a notice period. [S42]
- Microsoft: local processing of Microsoft 365 Copilot interactions in Australia is expected by the end of 2026. It was first promised for the end of 2025, and Microsoft revised the timeline on 3 April 2026. [S48]
- OpenAI: workspace agents start switched off for Enterprise workspaces at launch. [S16]
- OpenAI: developer mode carries a beta label on the pricing pages. [S7][S8]
- OpenAI: more data residency and inference residency regions are planned. [S17]
- Anthropic: Enterprise-managed auth supports Okta at launch, "with more identity providers coming soon". [S27]
- Anthropic: request header sign-in for custom connectors is in beta for a limited set of organisations. [S34]
- Anthropic: installing connectors on mobile is in beta. [S23]
- Google: for now, custom MCP apps in Gemini are English-only and unavailable to work and school accounts. They also require the user to be in the US. [S62]
- Google: Personal Intelligence, which connects Google apps for personalisation, is being released gradually and isn't offered in the EEA, Switzerland, the UK or Nigeria. [S64]
- MCP: the Registry is in preview, and breaking changes or data resets may happen before general availability. [S76]
- MCP: the 2026-07-28 version deprecates a feature called sampling. [S71]
- Zapier: building Next Gen Zaps from AI tools is in early access. Running them is free during early access, then priced in tasks. [S79]
- Make: Make AI Agent (New) is in open beta, and its features and pricing may change. [S90]
- n8n: the old version of the AI Agent node will be removed in n8n 3.0. [S94]

## What we couldn't establish

- Whether ChatGPT Plus can connect custom MCP servers. We re-read both pages on 15 October 2026. The pricing page still lists Developer mode (beta) for Plus and Pro, while the help page names only Pro (read and fetch) and Business, Enterprise and Edu (full). [S7][S5]
- Whether OpenAI-built apps can write. The custom MCP page says they're search-only, while other OpenAI pages describe write actions in apps such as Google Drive and Microsoft's apps. [S5][S6][S1]
- How the local MCP apps in ChatGPT desktop plugins fit with the custom MCP page, which answers "Not directly" when asked about local servers. [S2][S5]
- Whether Anthropic's Enterprise-managed auth is in beta or generally available. One Anthropic page says beta, and another says generally available. [S23][S27]
- Whether Microsoft's write actions through federated connectors are live in Australian tenants yet. [S42]
- Whether Copilot Chat users without the paid licence can use federated connectors. Microsoft says "where available". [S42]
- A formal Microsoft statement that Graph connectors became Copilot connectors. The pages we read use the new name without stating a rename. [S41][S43]
- A formal Google statement that Gemini extensions became Connected Apps. Current pages use the new name without stating a rename. [S61][S66]
- That Gemini Enterprise was formerly called Agentspace. Google's current overview doesn't mention an earlier name. [S67]
- The storage period for the updated personal Copilot app, and whether it has any training switch. [S50][S51]
- Whether Microsoft's wording for the new Copilot app ("foundation models") also covers other models. [S50]
- Any Australian storage or processing option for the Claude apps (web, desktop and mobile). [S23][S39]
- Whether Claude's memory saves information that came through connectors. The pages we read don't say.
- What Zapier does with non-Enterprise data for AI training. [S82]
- Connectors in Microsoft's personal Copilot app. We didn't research these.
- Prices in Australian dollars. OpenAI's Business page shows A$ headline prices next to fine print in another, unlabelled currency, and Claude's pricing page shows US dollars only. We've named plans instead. [S8][S35]
- Exact update dates for Google's Gemini help articles and Make's help centre, which show no date.
- Research note: the session's shared web-search allowance ran out partway through. Later checks were done by opening known official pages directly. Google's Workspace admin settings for third-party apps in Gemini weren't covered in depth.

## Sources

Many help centres show relative dates such as "4 days ago". Where a page carried an exact timestamp, it's given in brackets, in UTC. Perth is eight hours ahead of UTC. "Page metadata" means the date sits in the page's code, with no date shown to readers.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Connected apps in ChatGPT | OpenAI | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 4 days ago" (timestamp 11 Oct 2026, UTC) | 15 Oct 2026 |
| S2 | Plugins in ChatGPT | OpenAI | https://help.openai.com/en/articles/20001256-plugins-in-chatgpt | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S3 | Connecting and managing app accounts in ChatGPT | OpenAI | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S4 | Managing app permissions in ChatGPT | OpenAI | https://help.openai.com/en/articles/20001495-managing-app-permissions-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S5 | Connecting custom MCP servers in ChatGPT | OpenAI | https://help.openai.com/en/articles/12584461-connecting-custom-mcp-servers-in-chatgpt | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S6 | Admin controls, security, and compliance for plugins and apps | OpenAI | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S7 | Plans and Pricing (individual plans) | OpenAI | https://chatgpt.com/pricing/ | No date shown | 15 Oct 2026 |
| S8 | ChatGPT Business and Enterprise pricing | OpenAI | https://openai.com/business/pricing/ | No date shown | 15 Oct 2026 |
| S9 | How your data is used to improve model performance | OpenAI | https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance | "Updated: 3 days ago" (12 Oct 2026, UTC) | 15 Oct 2026 |
| S10 | Data controls in ChatGPT | OpenAI | https://help.openai.com/en/articles/7730893-data-controls-in-chatgpt | "Updated: 17 days ago" (28 Sep 2026, UTC) | 15 Oct 2026 |
| S11 | Google app data controls FAQ | OpenAI | https://help.openai.com/en/articles/10408842-google-app-data-controls-faq | "Updated: 20 days ago" (25 Sep 2026, UTC) | 15 Oct 2026 |
| S12 | Memory in ChatGPT | OpenAI | https://help.openai.com/en/articles/8590148 | "Updated: 26 days ago" (19 Sep 2026, UTC) | 15 Oct 2026 |
| S13 | Deep research in ChatGPT | OpenAI | https://help.openai.com/en/articles/10500283-deep-research | "Updated: 24 days ago" (21 Sep 2026, UTC) | 15 Oct 2026 |
| S14 | ChatGPT agent | OpenAI | https://help.openai.com/en/articles/11752874-chatgpt-agent | "Updated: last month" (15 Sep 2026, UTC) | 15 Oct 2026 |
| S15 | ChatGPT Work and Codex | OpenAI | https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex | "Updated: 5 days ago" (10 Oct 2026, UTC) | 15 Oct 2026 |
| S16 | ChatGPT Workspace Agents for Enterprise and Business | OpenAI | https://help.openai.com/en/articles/20001143 | "Updated: 2 days ago" (13 Oct 2026, UTC) | 15 Oct 2026 |
| S17 | Data residency and inference residency for ChatGPT | OpenAI | https://help.openai.com/en/articles/9903489 | "Updated: 12 days ago" (3 Oct 2026, UTC) | 15 Oct 2026 |
| S18 | Administrator-managed apps with sync in ChatGPT | OpenAI | https://help.openai.com/en/articles/10847137 | "Updated: 10 days ago" (5 Oct 2026, UTC) | 15 Oct 2026 |
| S19 | ChatGPT Supported Countries | OpenAI | https://help.openai.com/en/articles/7947663-chatgpt-supported-countries | "Updated: 2 months ago" (12 Aug 2026, UTC) | 15 Oct 2026 |
| S20 | Enterprise privacy at OpenAI | OpenAI | https://openai.com/enterprise-privacy/ | "Updated: January 8, 2026" | 15 Oct 2026 |
| S21 | Lockdown Mode | OpenAI | https://help.openai.com/en/articles/20001061 | "Updated: 21 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S22 | Elevated Risk labels | OpenAI | https://help.openai.com/en/articles/20001062 | "Updated: last month" (31 Aug 2026, UTC) | 15 Oct 2026 |
| S23 | Use connectors to extend Claude's capabilities | Anthropic | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated over 2 weeks ago" (1 Oct 2026) | 15 Oct 2026 |
| S24 | Get started with custom connectors using remote MCP | Anthropic | https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp | "Updated over 2 weeks ago" (1 Oct 2026) | 15 Oct 2026 |
| S25 | Getting Started with Local MCP Servers on Claude Desktop | Anthropic | https://support.claude.com/en/articles/10949351-getting-started-with-local-mcp-servers-on-claude-desktop | "Updated over 2 weeks ago" (25 Sep 2026) | 15 Oct 2026 |
| S26 | When to use desktop and web connectors | Anthropic | https://support.claude.com/en/articles/11725091-when-to-use-desktop-and-web-connectors | "Updated over 2 weeks ago" (25 Sep 2026) | 15 Oct 2026 |
| S27 | Authorize MCP connectors for your entire organization | Anthropic | https://support.claude.com/en/articles/15537633-authorize-mcp-connectors-for-your-entire-organization | August 24, 2026 | 15 Oct 2026 |
| S28 | Restrict verified-domain connectors to your Enterprise | Anthropic | https://support.claude.com/en/articles/15402193-restrict-verified-domain-connectors-to-your-enterprise | "Updated over 2 weeks ago" (25 Sep 2026) | 15 Oct 2026 |
| S29 | How Claude suggests connected apps | Anthropic | https://support.claude.com/en/articles/14730684-how-claude-suggests-connected-apps | April 23, 2026 | 15 Oct 2026 |
| S30 | Manage Claude's tool access | Anthropic | https://support.claude.com/en/articles/13730515-manage-claude-s-tool-access | March 16, 2026 | 15 Oct 2026 |
| S31 | Get started with connectors | Anthropic | https://claude.com/docs/connectors/getting-started | No date shown (page metadata 25 Sep 2026) | 15 Oct 2026 |
| S32 | Connector verification | Anthropic | https://claude.com/docs/connectors/verification | No date shown (page metadata 25 Sep 2026) | 15 Oct 2026 |
| S33 | Connectors directory | Anthropic | https://claude.com/docs/connectors/directory | No date shown (page metadata 25 Sep 2026) | 15 Oct 2026 |
| S34 | Add a connector that isn't in the directory | Anthropic | https://claude.com/docs/connectors/custom/add-unlisted | No date shown (page metadata 25 Sep 2026) | 15 Oct 2026 |
| S35 | Plans & pricing | Anthropic | https://claude.com/pricing | No date shown | 15 Oct 2026 |
| S36 | Is my data used for model training? (consumer products) | Anthropic | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | March 16, 2026 | 15 Oct 2026 |
| S37 | Is my data used for model training? (commercial products) | Anthropic | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | August 18, 2026 | 15 Oct 2026 |
| S38 | Supported Regions Policy | Anthropic | https://www.anthropic.com/legal/supported-regions | "Effective May 12, 2026" | 15 Oct 2026 |
| S39 | Regional compliance | Anthropic | https://claude.com/regional-compliance | No date shown | 15 Oct 2026 |
| S40 | Overview of Microsoft Copilot Chat | Microsoft | https://learn.microsoft.com/en-us/copilot/overview | "Last updated on 2026-09-10" | 15 Oct 2026 |
| S41 | Copilot connectors overview | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview | Updated 12 Oct 2026 (page metadata) | 15 Oct 2026 |
| S42 | Federated connectors overview | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Updated 14 Oct 2026 (page metadata) | 15 Oct 2026 |
| S43 | Microsoft 365 Copilot connectors overview (developer) | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-copilot-connector | Updated 30 Sep 2026 (page metadata) | 15 Oct 2026 |
| S44 | Compare declarative and custom engine agents | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agents-overview | Updated 30 Sep 2026 (page metadata) | 15 Oct 2026 |
| S45 | Extend your agent with Model Context Protocol (Copilot Studio) | Microsoft | https://learn.microsoft.com/en-us/microsoft-copilot-studio/agent-extend-action-mcp | Updated 26 Aug 2026 (page metadata) | 15 Oct 2026 |
| S46 | Governance and lifecycle actions for agents available in Microsoft 365 admin center | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/admin/manage/agent-actions | Updated 13 Oct 2026 (page metadata) | 15 Oct 2026 |
| S47 | Data, Privacy, and Security for Microsoft Copilot | Microsoft | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy | Updated 8 Oct 2026 (page metadata) | 15 Oct 2026 |
| S48 | Microsoft offers in-country data processing to 15 countries to strengthen sovereign controls for Microsoft 365 Copilot | Microsoft (Microsoft 365 Blog) | https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/ | Published 5 Nov 2025; editor's note dated 3 Apr 2026 | 15 Oct 2026 |
| S49 | Privacy FAQ for Microsoft Copilot (older app) | Microsoft | https://support.microsoft.com/en-au/microsoft-copilot/privacy-faq-for-microsoft-copilot | Updated 31 Aug 2026 (page metadata) | 15 Oct 2026 |
| S50 | Microsoft Copilot for individuals: your activity history | Microsoft | https://support.microsoft.com/en-us/privacy/microsoft-copilot/activity-history | Updated 18 Aug 2026 (page metadata) | 15 Oct 2026 |
| S51 | Microsoft Copilot for individuals: your privacy controls and choices | Microsoft | https://support.microsoft.com/en-us/privacy/microsoft-copilot/privacy-controls | Updated 17 Sep 2026 (page metadata) | 15 Oct 2026 |
| S52 | Copilot in Power Automate | Microsoft | https://learn.microsoft.com/en-us/power-automate/copilot-overview | Updated 18 Aug 2026 (page metadata) | 15 Oct 2026 |
| S53 | Agent flows overview (Copilot Studio) | Microsoft | https://learn.microsoft.com/en-us/microsoft-copilot-studio/flows-overview | Updated 3 Aug 2026 (page metadata) | 15 Oct 2026 |
| S54 | Connectors overview | Microsoft | https://learn.microsoft.com/en-us/connectors/overview | Updated 27 Aug 2026 (page metadata) | 15 Oct 2026 |
| S55 | Copilot Studio, Power Platform, and Azure Logic Apps connectors documentation | Microsoft | https://learn.microsoft.com/en-us/connectors/ | Updated 30 Sep 2026 (page metadata) | 15 Oct 2026 |
| S56 | Overview of permissions and consent in the Microsoft identity platform | Microsoft | https://learn.microsoft.com/en-us/entra/identity-platform/permissions-consent-overview | Updated 25 Jun 2026 (page metadata) | 15 Oct 2026 |
| S57 | Overview of user and admin consent | Microsoft | https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/user-admin-consent-overview | Updated 19 Feb 2026 (page metadata) | 15 Oct 2026 |
| S58 | OAuth 2.0 and OIDC authentication flow in the Microsoft identity platform | Microsoft | https://learn.microsoft.com/en-us/entra/identity-platform/v2-protocols | Updated 30 Jun 2026 (page metadata) | 15 Oct 2026 |
| S59 | Explore the Power Automate home page | Microsoft | https://learn.microsoft.com/en-us/power-automate/getting-started | Updated 25 Sep 2026 (page metadata) | 15 Oct 2026 |
| S60 | Gemini Apps Privacy Hub | Google | https://support.google.com/gemini/answer/13594961 | "Last updated: October 13, 2026" | 15 Oct 2026 |
| S61 | Use & manage Connected Apps in Gemini | Google | https://support.google.com/gemini/answer/13695044 | No date shown | 15 Oct 2026 |
| S62 | Connect & manage custom apps for Gemini Apps | Google | https://support.google.com/gemini/answer/17209137 | No date shown | 15 Oct 2026 |
| S63 | Use apps connected to Gemini with a work or school Google Account | Google | https://support.google.com/gemini/answer/14959807 | No date shown | 15 Oct 2026 |
| S64 | Connect your Google apps to personalize your Gemini experience | Google | https://support.google.com/gemini/answer/16598406 | No date shown | 15 Oct 2026 |
| S65 | Turn the Gemini App on or off | Google | https://knowledge.workspace.google.com/admin/generative-ai/gemini-app/turn-the-gemini-app-on-or-off | "Last updated 2026-10-13 UTC" | 15 Oct 2026 |
| S66 | Generative AI in Google Workspace Privacy Hub | Google | https://knowledge.workspace.google.com/admin/generative-ai/generative-ai-in-google-workspace-privacy-hub | "Last updated 2026-10-13 UTC" | 15 Oct 2026 |
| S67 | What is Gemini Enterprise? | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs | "Last updated 2026-10-14 UTC" | 15 Oct 2026 |
| S68 | Introduction to connectors and data stores (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/introduction-to-connectors-and-data-stores | "Last updated 2026-10-14 UTC" | 15 Oct 2026 |
| S69 | Manage API keys | Google Cloud | https://docs.cloud.google.com/docs/authentication/api-keys | "Last updated 2026-10-13 UTC" | 15 Oct 2026 |
| S70 | What is the Model Context Protocol (MCP)? | Model Context Protocol | https://modelcontextprotocol.io/docs/getting-started/intro | No date shown (page metadata 13 Oct 2026) | 15 Oct 2026 |
| S71 | Architecture overview | Model Context Protocol | https://modelcontextprotocol.io/docs/learn/architecture | No date shown (page metadata 13 Oct 2026) | 15 Oct 2026 |
| S72 | Specification (version 2026-07-28) | Model Context Protocol | https://modelcontextprotocol.io/specification/2026-07-28 | No date shown (page metadata 13 Oct 2026) | 15 Oct 2026 |
| S73 | Security Best Practices | Model Context Protocol | https://modelcontextprotocol.io/docs/2026-07-28/tutorials/security/security_best_practices | No date shown (page metadata 28 Jul 2026) | 15 Oct 2026 |
| S74 | Connect to remote MCP Servers | Model Context Protocol | https://modelcontextprotocol.io/docs/2026-07-28/develop/connect-remote-servers | No date shown (page metadata 28 Sep 2026) | 15 Oct 2026 |
| S75 | Connect to local MCP servers | Model Context Protocol | https://modelcontextprotocol.io/docs/2026-07-28/develop/connect-local-servers | No date shown (page metadata 11 Oct 2026) | 15 Oct 2026 |
| S76 | The MCP Registry | Model Context Protocol | https://modelcontextprotocol.io/registry/about | No date shown (page metadata 13 Oct 2026) | 15 Oct 2026 |
| S77 | Governance and Stewardship | Model Context Protocol | https://modelcontextprotocol.io/community/governance | No date shown (page metadata 5 Aug 2026) | 15 Oct 2026 |
| S78 | Model Context Protocol servers (README) | Model Context Protocol (official GitHub organisation) | https://github.com/modelcontextprotocol/servers | No date shown (README last changed 31 Aug 2026, per GitHub history) | 15 Oct 2026 |
| S79 | Zapier MCP | Zapier | https://zapier.com/mcp | No date shown | 15 Oct 2026 |
| S80 | Zapier MCP: Model Context Protocol for 9,000+ app integrations | Zapier | https://docs.zapier.com/mcp/home | No date shown (page metadata 9 Oct 2026) | 15 Oct 2026 |
| S81 | How Zapier MCP connections work | Zapier | https://docs.zapier.com/mcp/overview/how-connections-work | No date shown (page metadata 1 Oct 2026) | 15 Oct 2026 |
| S82 | Zapier MCP security | Zapier | https://docs.zapier.com/mcp/manage/security | No date shown (page metadata 1 Oct 2026) | 15 Oct 2026 |
| S83 | Zapier MCP for ChatGPT | Zapier | https://docs.zapier.com/mcp/get-started/connect/chatgpt | No date shown (page metadata 7 Oct 2026) | 15 Oct 2026 |
| S84 | Zapier MCP for Claude | Zapier | https://docs.zapier.com/mcp/get-started/connect/claude | No date shown (page metadata 1 Oct 2026) | 15 Oct 2026 |
| S85 | What is Zapier? | Zapier | https://help.zapier.com/hc/en-us/articles/37518970271245-What-is-Zapier | 8 Sep 2026 (page timestamp) | 15 Oct 2026 |
| S86 | Zapier Agents | Zapier | https://zapier.com/agents | No date shown | 15 Oct 2026 |
| S87 | AI Actions (former addresses) | Zapier | https://actions.zapier.com/ and https://docs.zapier.com/ai-actions/home | No date; both redirected to Zapier MCP when read | 15 Oct 2026 |
| S88 | Make MCP Server | Make | https://developers.make.com/mcp-server | "Last updated 2 hours ago" (15 Oct 2026) | 15 Oct 2026 |
| S89 | Connect using OAuth | Make | https://developers.make.com/mcp-server/connect-using-oauth | "Last updated 1 month ago" | 15 Oct 2026 |
| S90 | Introduction to Make AI Agent (New) | Make | https://help.make.com/introduction-to-make-ai-agent-new | No date shown | 15 Oct 2026 |
| S91 | Introduction to MCP | Make | https://help.make.com/introduction-to-mcp | No date shown | 15 Oct 2026 |
| S92 | MCP toolboxes | Make | https://help.make.com/mcp-toolboxes | No date shown | 15 Oct 2026 |
| S93 | AI providers and data zones in Make | Make | https://help.make.com/ai-providers-and-data-zones-in-make | No date shown | 15 Oct 2026 |
| S94 | AI Agent (node) | n8n | https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.agent/ | "Last updated 2 days ago" (13 Oct 2026) | 15 Oct 2026 |
| S95 | MCP Server Trigger (node) | n8n | https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-langchain.mcptrigger/ | "Last updated 2 days ago" (13 Oct 2026) | 15 Oct 2026 |
| S96 | MCP Client Tool (node) | n8n | https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.toolmcp/ | "Last updated 2 days ago" (13 Oct 2026) | 15 Oct 2026 |
| S97 | Host n8n | n8n | https://docs.n8n.io/deploy/host-n8n | "Last updated 2 days ago" (13 Oct 2026) | 15 Oct 2026 |
| S98 | ChatGPT release notes | OpenAI | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
