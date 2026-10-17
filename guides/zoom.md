# Zoom: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Zoom has retired the name "AI Companion". Its built-in AI features now go by plain names, like meeting summary, and Zoom groups them as Zoom AI. [S4] [S7] [S17]
- Paid Zoom Workplace plans include the core AI at no extra cost, including meeting summaries, in-meeting questions and AI note-taking. The free Basic plan gets summaries for three meetings a month. [S4] [S1]
- ZoomMate is Zoom's paid AI agent. With the currency set to Australian dollars, Zoom lists it at A$30.40 a user a month, or A$25.33 a month billed annually, with 2,200 AI credits a month. [S2]
- Zoom says it doesn't use your meeting audio, video, chat, screen sharing or other "communications-like" content to train its own or third-party AI models. [S18]
- When meeting summary or meeting questions is on, everyone in the meeting sees a lit AI icon. Admins can add a custom message and require people to agree to recording and transcription. [S11] [S12]
- My Notes is the one to watch. In Microsoft Teams, Google Meet or in-person meetings it transcribes your device's audio, and Zoom gives the other people no notice. [S14]
- Accounts hosted in Australia run Zoom's AI on Zoom's own models and Zoom-managed copies of other models on Amazon Bedrock. Some features, including ZoomMate's agents and deep research, aren't offered that way. [S9] [S15]
- Claude and ChatGPT each have official Zoom connections. They read meeting summaries, transcripts and recordings, and create Zoom documents after you confirm. [S34] [S41]
- Microsoft Copilot connects two ways: Microsoft's own Zoom Meetings connector, and Zoom's "Zoom for Cowork" app. [S44] [S43]
- We found no official connection between Zoom and Google Gemini. [S47] [S49]

## The tool, and the plans that matter

Zoom Workplace puts Zoom's meetings together with team chat, phone, mail, calendar, whiteboards and documents. [S1]

These are the plans on Zoom's pricing pages with the currency set to Australian dollars, read from Perth on 17 October 2026. [S1] [S2] [S3]

| Plan | Price a month (AUD, as shown) | AI included | Worth knowing |
|---|---|---|---|
| Basic | Free | Meeting summaries for 3 hosted meetings a month, 3 AI note-taking uses and 20 AI queries | 40-minute meetings, 100 participants |
| Pro | A$25.99 per user paying monthly, or A$21.66 billed annually | Unlimited meeting summaries, in-meeting questions and AI note-taking. 8 custom summary templates a month. | 30-hour meetings, 10 GB of cloud recording per licence |
| Business | A$32.99 per user paying monthly, or A$27.83 billed annually | As Pro, plus AI in Whiteboard | 300 participants, single sign-on, multi-region storage |
| Enterprise | No price shown | As Business | Unlimited cloud recording |
| ZoomMate (add-on) | A$30.40 per user paying monthly, or A$25.33 billed annually | 2,200 AI credits a month, AI agents, deep research, third-party connectors and unlimited AI note-taking | Agent actions and third-party work use credits |
| My Notes (added to Basic) | A$15.20 per user paying monthly, or A$12.67 billed annually | Unlimited AI note-taking, and summaries for all hosted meetings | Summaries "can be sent to Slack automatically" |

Sources for the table: [S1] [S2] [S3] [S4]

- When we first loaded the pricing page it showed US dollars. Switching the currency selector to Australian dollars gave the prices above. [S1]
- Zoom's FAQ says any GST is added in the shopping cart before checkout, depending on tax law and your details. It doesn't say whether listed prices include GST. [S1]
- Zoom's support articles also name Pro Plus, Business Plus, Enterprise Plus and Enterprise Bundle plans. The pricing pages we read don't price them. [S19]
- The comparison table says AI features don't apply to users with Basic permissions on a paid account. [S1]
- Zoom says many AI features, including meeting summaries and note-taking, don't use AI credits. Credits pay for metered features, such as ZoomMate's agents and AI-made slides and spreadsheets. [S29]
- Monthly credits expire at each subscription anniversary and don't roll over. [S29]
- ZoomMate "builds on Custom AI Companion", the older paid add-on. Zoom says Custom AI Companion customers will still be supported. [S4]
- Zoom launched ZoomMate on 1 June 2026 for North American customers, "starting at $20 per user per month". It said EMEA and APAC were "expected to roll out later this year". [S5]
- Verified non-profits get 50% off Workplace Pro and Business. [S1]
- Zoom AI On-Prem, launched on 22 June 2026, runs captions and transcription inside an organisation's own infrastructure through the Zoom Node add-on. [S6]

## AI built in

### Meeting summary

**What it does**

- After a meeting, Zoom AI writes a summary of the key points, decisions and next steps. [S13] [S17]
- It works from the meeting's speech-to-text data. Depending on settings it can also use screen-shared content, read by OCR (which turns pictures of text into text), and the in-meeting chat. [S18]
- A summary can be turned into a Canvas document, and its next steps can become Zoom Tasks. [S13] [S17]

**Where to find it**

- In a meeting on desktop, hover over the **Zoom AI** icon at the top right, tick **Meeting summary**, optionally tick **Generate transcript**, then click **Start Zoom AI**. [S19]
- A participant can click **Ask host to start Zoom AI**. [S19]
- To stop, untick **Meeting summary** or click **Stop Zoom AI**. You can also tick **Delete meeting assets** to delete the transcript and summary made so far. [S19]
- Afterwards, find summaries in the web portal under **My account > Summaries**, in Zoom Hub, by email or in the meeting's group chat. [S19]
- Hosts can set summaries to start automatically. Zoom says generation then begins as soon as someone starts the meeting, even if the host isn't there. [S19]

**Which plans have it**

- Licensed users on Workplace Pro, Pro Plus, Business, Business Plus, Enterprise, Enterprise Plus or Enterprise Bundle. [S19]
- Basic gets summaries for three hosted meetings a month. [S1]

**What happens to your data**

- Only the host and co-hosts can start or stop the summary from the meeting controls. [S19]
- The summary goes to the host automatically. Participants get it by email or Zoom Chat if the host chose to share it. [S17] [S19]
- "Anyone who receives the meeting summary may save and share it with apps and others. The account owner can access the meeting summary." [S19]
- Participants see the AI icon change colour while AI features are on. [S19] [S11]
- Admins can keep summaries without keeping transcripts. If the meeting transcript setting is disabled and locked, or transcript retention is set to zero days, Zoom discards the speech-to-text data once the summary is made. [S9] [S12]
- Zoom emails summaries through Twilio SendGrid, which samples email content and keeps it for seven days for anti-fraud checks. Twilio processes data in the US. [S18]
- Admins can have some personal details redacted from summaries, or block patterns such as card numbers. Both need a Zoom support ticket to switch on. [S12]

**In Australia**

- For accounts hosted in Australia, Zoom offers meeting summary through its ZM+ and Zoom-hosted-only (ZMO) setups. [S9] [S15]
- Zoom says AI features "may not be available for select industry verticals and select regional customers". [S19]

### In-meeting questions

**What it does**

- Lets people ask Zoom AI about the meeting while it's running, such as "Catch me up" or "What are the action items?". [S20]
- Answers include timestamped citations from the conversation. [S13]

**Where to find it**

- The host clicks the **Zoom AI** icon, ticks **Meeting questions** and clicks **Start Zoom AI**. [S20]
- Hosts and participants can only ask questions in the desktop app. [S20]

**Which plans have it**

- Licensed users on Workplace Pro and above. Basic gets three hosted meetings a month. [S20] [S1]

**What happens to your data**

- Under **Who can ask questions about the meeting?**, the host chooses who can ask. The options run from all participants and invitees down to **Only meeting hosts**, and can stop people asking about what was said before they joined. [S20]
- It uses speech-to-text data and, depending on host settings, the meeting chat and screen-shared content. [S20]

**In Australia**

- Zoom lists it under both the ZM+ and ZMO setups. [S15]

### Smart recording

**What it does**

- Adds AI chapters, highlights, a summary and next steps to cloud recordings. [S21]
- It also gives hosts coaching figures such as talk speed and filler words. [S21]

**Where to find it**

- In the web portal, click **Profile**, then **Recordings and Transcripts**, open the **Cloud recordings** tab and click the meeting. [S21]

**Which plans have it**

- Workplace Pro and above, or Zoom Workplace for Education, with cloud recording, **Create audio transcript** and **Smart recording with AI** turned on. [S21]

**What happens to your data**

- Zoom says the chapters and highlights "can be shared and seen by others". [S17]
- The recording's owner, or someone allowed to manage recordings, can edit them. [S21]
- Admins choose where cloud recordings and their transcripts are stored, and Australia is one of the options. [S28]

**In Australia**

- Zoom lists smart recording under both the ZM+ and ZMO setups. [S15]

### Meeting transcripts (the record underneath)

**What it does**

- A transcript is the saved text record of what was said. Zoom AI can use it later for questions after the meeting and for Canvas documents. [S22]

**Where to find it**

- Admins go to **Admin Center > Settings > Meeting**, then under **In Meeting (Advanced)** use the **Meeting transcript** toggle. [S22]
- The sub-settings include **Custom disclaimer for transcripts**, **Delete transcripts after a specified number of days** (up to 9,999 days) and **Allow saving of transcripts to computer by**. [S22]

**Which plans have it**

- Pro, Business and Enterprise accounts. [S22]

**What happens to your data**

- Transcripts aren't on by default. A host or admin has to turn them on. [S22]
- Admins can make transcripts always on for the whole organisation. [S22]
- Live captions aren't kept after the session, though they show when a recording is played back. [S13]
- A cloud recording can create and keep its own transcript, whatever the meeting transcript setting says. [S9]
- Zoom notes that its settings don't stop participants or other parties making their own copies of a transcript. [S9] [S12]

**In Australia**

- Admins can store cloud recording transcripts in Australia. [S28]

### My Notes (AI note-taking, including in other meeting apps)

**What it does**

- A personal note-taker for Zoom meetings, other platforms' meetings such as Microsoft Teams and Google Meet, and in-person conversations. [S14]
- It combines your own notes with a transcript to produce detailed notes after the meeting. [S14]
- In other apps and in person, it uses your computer's microphone and system audio, once you've turned it on. [S14]

**Where to find it**

- Admins go to **Admin Center > Settings > Notes** and use **Enable My Notes** and its sub-settings, such as **Allow participants to transcribe meetings with My Notes**. [S25]
- Saved notes are in Zoom Hub under My Notes, on the meeting card and in Canvas. [S14]
- The desktop app can show a **Take notes** prompt when it detects your microphone in use. [S26]

**Which plans have it**

- Pro, Business, Enterprise, or a My Notes standalone account. Basic gets three uses a month. [S26] [S1]

**What happens to your data**

- Notes belong to the person who made them and aren't shared automatically. Authorised account admins can view them in the admin portal. [S14]
- Zoom deletes the audio once transcription is complete. The notes and transcript stay in your account under your retention settings. [S14]
- On mobile, the recording of a non-Zoom meeting is deleted by default. An admin setting can save it to cloud recording storage instead. [S26] [S25]
- In a Zoom meeting, others see a banner, a transcription icon and a pencil icon next to anyone using My Notes, and the host can stop it. [S11] [S14]
- In other platforms' meetings, Zoom gives the other people no notice and their host can't stop it. Zoom reminds the user to follow the law, "which may include providing notice". [S14] [S26]
- Muting yourself in Teams or a browser doesn't stop My Notes hearing your microphone. You have to pause it in My Notes. [S14]
- Zoom's zero data retention option for summaries doesn't cover My Notes, which has its own retention settings. [S14] [S27]
- Admins can auto-delete notes after a set time. Deleted notes sit in the trash for 30 days, but My Notes transcripts are deleted permanently with no trash. [S27]

**In Australia**

- Zoom lists My Notes under its ZM+ setup but not under Zoom-hosted models only (ZMO). [S15]
- For in-person and third-party meetings it transcribes 12 languages, including English. [S14]

### Zoom AI in Microsoft Teams and Google Meet meetings

**What it does**

- An admin can let users invite Zoom AI into Microsoft Teams and Google Meet meetings as a participant, to make transcripts and summaries. [S24]

**Where to find it**

- Admins go to **Admin Center > Settings > Zoom AI**, then under **Meetings** use the **Allow Zoom AI to join third-party meetings** toggle. [S24]
- **Automatically join meetings on user's calendar** can send it to every meeting with a video link, or only to meetings you host or attend. [S24]

**Which plans have it**

- Workplace Pro, Pro Plus, Business, Business Plus, Enterprise or Workplace for Education. The user's calendar must be synced. [S24]

**What happens to your data**

- An optional **Pre-meeting email notification** can tell all invitees, or only the host, 10 minutes before the meeting starts. [S24]
- The article doesn't describe any notice inside the other platform's meeting. [S24]

**In Australia**

- The article doesn't mention regions. [S24]

### AI in chat, mail, phone, documents and whiteboards

**What it does**

- An AI chat panel sits beside Mail, Team Chat and other Zoom products, and starts from whatever you're looking at. [S13]
- Chat compose drafts messages, and chat summaries catch you up on long threads. [S17]
- Email compose drafts replies, and email summary condenses long emails. [S13]
- Zoom Phone can summarise calls, list tasks from voicemails and answer questions during a call. [S13]
- Whiteboard and Canvas can generate content, and AI also works in Zoom Slides, Sheets and Paper. [S17]

**Where to find it**

- Admins turn features on or off under **Admin Center > Settings**, then the **Zoom AI** tab. Users can change unlocked settings under their own **Settings**. [S17]

**Which plans have it**

- Zoom says eligible paid plans include core AI features at no extra cost, and many aren't metered. [S4] [S29]
- Slides, Sheets and Paper generation are metered. They need an AI Productivity Suite or ZoomMate licence, plus credits. [S17]

**What happens to your data**

- Chat compose sends the chat thread, participant names and your draft to the AI model. [S18]
- Zoom says its AI "may provide incorrect, inaccurate, misleading, or offensive responses" and asks you to check the output. [S18]

**In Australia**

- Under ZM+, email compose and email summary are available, but voicemail prioritisation and whiteboard image generation aren't. [S15]

### ZoomMate (Zoom's paid AI agent)

**What it does**

- Zoom calls ZoomMate "an agentic AI work surface". It searches Zoom, the web and connected business systems, then helps finish the work. [S5]
- It can draft documents, slides and spreadsheets from meetings, schedule events and update records in other systems. [S5]
- AI agents can sit in Zoom Chat channels. When they're in a channel, a notice says "AI agents present". [S6] [S11]
- Its connectors reach Salesforce, Jira, Slack, Google Calendar, Confluence, Workday, Outlook, OneDrive and ServiceNow. [S30]
- It can browse the web and act on web pages through a Chrome extension or a cloud browser. [S30] [S18]

**Where to find it**

- In the desktop app, click the **ZoomMate** tab (or **More**, then **ZoomMate**). On the web portal, click the **Zoom Products** icon, then **ZoomMate**. [S30]

**Which plans have it**

- Some features work with Workplace Pro and above. Advanced and metered features need a ZoomMate licence and AI credits. [S30]
- The pricing page lists 2,200 credits per user a month. When credits run out, metered features are limited. [S2] [S29]

**What happens to your data**

- "You are responsible for your use of ZoomMate and the actions it takes on your behalf." [S30]
- Zoom says ZoomMate may ask for confirmation before sensitive actions, and urges caution before choosing "always approve". [S30]
- Data from ZoomMate's browser sessions, including screenshots, is saved to your conversation history. [S18]
- For sources an admin connects, such as Google Drive or Salesforce, Zoom stores the approved content in a customer-specific index along with the original permissions. [S16]
- Feedback can include your prompt, the response and screenshots if you choose. Admins can switch that extra context off. [S10]

**In Australia**

- Zoom's launch named North America, with APAC expected later in 2026. Its Australian-dollar pricing page now lists ZoomMate. [S5] [S2]
- Under ZM+, ZoomMate's AI agents, deep research, web search and live voice translation aren't available. [S15]
- Zoom says ZoomMate "may not be available for select verticals and select regional customers". [S30]

### Consent notices, admin switches and where AI data goes

**What it does**

- The recording consent disclaimer asks people to agree when a recording starts, or leave. The host can report who agreed. [S23]
- A separate **Custom Message** appears when meeting summary or meeting questions is turned on. Admins can require people to agree to recording and transcription before going on. [S12]
- **Custom disclaimer for transcripts** shows a notice when transcripts are turned on. [S22]
- Zoom's whitepaper says access to AI features depends on plan, licence, admin settings, region, credits and usage limits. [S8]

**Where to find it**

- Recording disclaimer: **Account Management > Account Settings**, then the **Recording & Transcript** tab. Under **Recording notifications - Zoom clients**, click **Customize Disclaimer**. [S23]
- AI features: **Admin Center > Settings**, then the **Zoom AI** tab. Click the lock icon to stop users changing a setting. [S17]

**Which plans have it**

- Customising the recording disclaimer needs a Business, Education, API or Enterprise account with 100 or more licences. [S23]
- Those accounts can also turn the recording disclaimer off for internal users. [S23]

**What happens to your data**

- "Zoom does not use any customer audio, video, chat, screen sharing, attachments, or other communications-like customer content (such as poll results, whiteboard, and reactions) to train Zoom's or its third-party artificial intelligence models." [S9]
- Zoom's standard approach mixes its own models with models from Anthropic, OpenAI and Google, picking one per task. Zoom says the models can change at any time. [S9]
- Zoom says outside model providers keep no customer content, apart from limited trust and safety cases such as detecting child sexual abuse material. [S9] [S18]
- Zoom staff can't access meeting content or AI output unless the account owner or an admin allows it, or for legal, safety, security or support reasons. [S9]
- Zoom's sub-processor list names Anthropic and Perplexity in the US, and OpenAI in the US and EU, as AI service providers. [S31]
- Zoom's privacy statement says personal data "may be transferred to or stored in the United States". [S32]

**In Australia**

- "For customers hosted in the EU or AU, Zoom uses ZM+ (or customers can choose ZMO) to support account data residency preferences for available features." [S9]
- ZM+ runs third-party models as Zoom-managed copies on Amazon Bedrock, so data isn't sent to the model makers. ZMO uses only Zoom's own models. [S9]
- Zoom's getting-started article also says "Data may be processed within U.S.-based data centers." [S17]
- Paid accounts can store recordings, recording transcripts and some other data in Australia. Account and operational data stays in the US. [S28]

## Outside AI that connects

A quick translation of the jargon. **MCP** (Model Context Protocol) is a standard way for an AI assistant to use another app's tools. Zoom runs MCP servers, and the Zoom for Claude connector reaches Zoom through one. [S37] [S33]

Most of these connections read what Zoom's own AI has already made, so they need meeting summary or smart recording switched on. [S34] [S41] [S43]

### Claude and Zoom

**Official?**

- Yes. "Zoom for Claude" is made by Zoom, marked "Anthropic verified", and was added to Claude's directory in April 2026. [S33]
- Zoom announced it on 9 April 2026, together with a Zoom plugin for Claude Code. [S35]
- A second connector, "Zoom Canvas", lets Claude create and manage Zoom Canvas documents. [S36]

**What it can see and do**

- Search Zoom Meetings, Zoom Chat and Zoom Canvas in plain language. [S34]
- Retrieve AI summaries, transcripts, recordings, documents, whiteboards and next steps. [S34]
- Create a Zoom Doc or follow-up Canvas from meeting content. Zoom's example says "Claude will confirm that you want to create a new Zoom Doc". [S34]
- The Zoom Canvas connector can edit, rename, share and delete Canvas files, change link access and transfer ownership, all at your request. [S36]
- You only see assets for meetings you hosted, or ones the host gave you access to. [S34]
- Claude can ask before using a tool. You can set each tool to **Always allow**, **Needs approval** or **Blocked**. [S51]

**What you need**

- A licensed user on Workplace Pro or above, and a Zoom account owner or admin with privileges. [S34]
- Meeting summary and smart recording switched on, because the connector depends on them. Video features need cloud recordings. [S34]
- For Zoom Canvas, non-admins can add it only if it's pre-approved in the Zoom Marketplace. [S36]
- A Claude account. Zoom's page doesn't name a Claude plan. On Claude Team and Enterprise, an Owner adds the connector first. [S34] [S50]

**Steps to connect** (Anthropic and Zoom docs, not dated)

1. In Claude, go to **Customize > Connectors** and select **Discover**. [S51]
2. Search for Zoom for Claude, open it and select **Connect to Claude**. [S51] [S34]
3. Sign in to Zoom and approve the access it asks for. [S34]
4. In a chat, select **+**, then **Connectors**, and switch Zoom on. [S51]
5. Ask for something from a recorded meeting, such as its action items. [S34]

Zoom Canvas (Zoom's support article, last modified 11 September 2026):

1. In Claude, click **Customize** in the left navigation, then **Connectors**. [S36]
2. Click the add icon, then **Browse connectors**. Search for **Zoom Canvas** and click **Connect**. [S36]
3. On the Zoom Marketplace page, click **Add**, confirm the permissions and click **Allow**. [S36]
4. Back in Claude, complete the authorisation. Zoom says the sign-in has to start from Claude. [S36]

**To disconnect**

- In Claude, open **Customize > Connectors**, select the connector, then **Disconnect**, or use the three-dot menu to **Remove** it. [S51]
- Zoom's Canvas article describes **Settings > Connectors**, then selecting Zoom Canvas and clicking **Remove**. [S36]
- In Zoom, remove the app from the Zoom Marketplace under **My Library**. [S55]

**Limits**

- Anthropic's listing warns: "Only use connectors from developers you trust." [S33]
- Claude can't give itself access to a Canvas file that you don't have. [S36]
- Zoom says the connector gives access "without moving or duplicating customer information". [S35]
- Zoom stores the Claude tokens and your Zoom sign-in credentials in an encrypted database. [S36]

### ChatGPT and Zoom

**Official?**

- Yes. The "Zoom" plugin in ChatGPT is built by Zoom Communications, Inc. [S40]
- Zoom also offers a "Zoom Whiteboard" connector for ChatGPT. [S42]

**What it can see and do**

- Read meeting details, past meetings, summaries, transcripts, recordings and files. It can find the moment a topic came up and play it in an embedded player. [S41] [S39]
- Create agendas and other files attached to meetings, and Zoom Canvas docs. ChatGPT confirms first, and the doc is only made after you click **Create**. [S41]
- The Whiteboard connector can create, update and delete whiteboards and change who has access. [S42]
- Your ChatGPT permission setting decides when it asks first. OpenAI lists creating, editing or deleting a file as actions that may need extra review. [S52]

**What you need**

- A licensed user on Workplace Pro or above, a Zoom account owner or admin with privileges, and a ChatGPT account. [S41]
- Meeting summary or smart recording switched on. The Ask tool needs a ZoomMate or Custom AI Companion licence. [S41]
- OpenAI says availability depends on the plugin, your plan and workspace settings, and some connections need admin approval. [S39]

**Steps to connect** (Zoom's support article, last modified 17 September 2026)

1. Sign in to ChatGPT, click your name, then **Settings**. [S41]
2. Click **Apps & Connectors**, then **Zoom**, then **Connect**. [S41]
3. On the Zoom Marketplace page, click **Add** at the top right. [S41]
4. Confirm the permissions and click **Allow**, then finish the authorisation back in ChatGPT. [S41]
5. In a chat, click the add icon, then **More**, then **Zoom**. Or type @Zoom or /Zoom. [S41]

**To disconnect**

- In ChatGPT, open **Settings > Plugins**, select Zoom, then **Disconnect**. [S53]
- Zoom's article says to remove it in the Zoom App Marketplace: click **Manage**, then **Added Apps**, then **Remove** next to Zoom for ChatGPT. [S41]
- For the Whiteboard connector, Zoom says to open **Apps & Connectors**, select Zoom Whiteboard and click **Remove**. [S42]

**Limits**

- When connected, ChatGPT may share relevant chats and memories with Zoom, under Zoom's terms and privacy policy. [S40]
- Zoom says data shared with ChatGPT is processed by OpenAI under OpenAI's terms, and that admins can restrict third-party app permissions in the Zoom Marketplace. [S42]
- Disconnecting doesn't delete past chats or memories in ChatGPT. [S53]
- The ChatGPT listing says "Use of apps may come with elevated risk." [S40]

### Microsoft Copilot and Zoom

**Official?**

- Yes, two ways. Microsoft builds a "Zoom Meetings" connector for Microsoft 365 Copilot. [S44] [S46]
- Zoom builds "Zoom for Cowork", an app for Microsoft 365 Copilot's Cowork. [S43]

**What it can see and do**

- The Zoom Meetings connector copies meeting transcripts, key points, summaries and details into Microsoft 365, so Copilot can answer questions about them. [S44] [S45]
- Only the meeting's owner can see its content in Copilot. Other participants can't, even if they attended. [S44]
- Zoom for Cowork lets Copilot users search their Zoom meetings and retrieve summaries, recordings, transcripts and whiteboards. [S43]
- It can create a Zoom Canvas document of action items. Copilot confirms first, and the doc is created after you click **Create**. [S43]

**What you need**

- For Microsoft's connector: an AI administrator in your Microsoft 365 tenant, a paid Zoom Business or Enterprise plan with cloud recording on, and a Zoom admin to sign in and consent. [S44]
- For Zoom for Cowork: a Zoom owner or admin, a Microsoft 365 Copilot account with admin rights to deploy it, and meeting summary or smart recording switched on. [S43]
- Zoom for Cowork's agentic search needs a ZoomMate licence. [S43]

**Steps to connect** (Microsoft Learn, updated 6 October 2026)

1. In the Microsoft 365 admin center, set up the Zoom Meetings connector and give it a display name. [S44]
2. Under authentication, select **OAuth 2.0**, then **Authorize**, and sign in with a Zoom administrator account. [S44]
3. Optionally switch on **Rollout to limited audience** and choose users and groups. [S44]
4. Tick the box next to the Notice section, then choose **Create**. Indexing starts straight away. [S44]
5. Check the connection shows **Ready** under **Copilot > Connectors > Your connections**, then ask Copilot about a recent recorded meeting. [S44]

Zoom for Cowork (Zoom's support article, last modified 11 September 2026):

1. In the Microsoft 365 admin center, click **Show all**, then **Settings**, then **Integrated apps**. [S43]
2. Select **Get Apps**, search for **Zoom for Cowork**, review its permissions and terms, choose who gets it and click **Deploy**. [S43]
3. In Microsoft 365 Copilot, click **Cowork** at the top left, then the plugin icon, and check Zoom is switched on. [S43]
4. Sign in to Zoom when asked and click **Allow**. [S43]

**To disconnect**

- Zoom for Cowork: in the Microsoft 365 admin center, open **Settings > Integrated apps**, select the Zoom app and click **Remove**, then **Remove** again to confirm. [S43]
- The Microsoft connector page we read doesn't give removal steps. [S44]

**Limits**

- Microsoft says the Copilot connector app in the Zoom Marketplace "isn't currently available in the European Union". It doesn't mention Australia. [S44]
- Zoom's API rate limits can slow a full refresh. By default Microsoft checks for changes every 15 minutes and runs a full crawl daily. [S44]
- Microsoft says Copilot Chat can't write back to other systems through indexing connectors by default. [S45]

### Google Gemini and Zoom

**Official?**

- No official connection found. [S47] [S48] [S49]

**What it can see and do**

- Google's lists of apps that connect to the Gemini app, for personal and for work or school accounts, don't include Zoom. [S47] [S48]
- Gemini Enterprise's list of third-party data sources has no Zoom connector. Its "LegalZoom" and "ZoomInfo" connectors are other companies' products. [S49]
- Zoom's whitepaper says Google Gemini models are among those Zoom AI uses inside its own features. That happens within Zoom and isn't a connection you set up. [S9]

**What you need**

- Not applicable. [S49]

**Steps to connect**

- None documented. Zoom's MCP guide only documents Claude and ChatGPT. [S37]

**To disconnect**

- Not applicable. [S47]

**Limits**

- Zoom's sub-processor list names Google Cloud Platform as a cloud and AI provider for Zoom's own features. [S31]

### Zoom's MCP servers (the developer route)

**Official?**

- Yes. Zoom runs MCP servers for product areas such as Meetings, Chat and Whiteboard. [S37]
- On 18 May 2026 Zoom expanded them, adding a plugin for OpenAI's Codex and access from Claude. [S38]

**What it can see and do**

- Zoom says outside AI tools can access "Zoom meeting summaries, transcripts, recordings, notes, action items, and collaboration history". [S38]
- Its agentic search covers Zoom Meetings, Chat, Phone and Canvas, plus ten connected platforms at launch, such as Salesforce and ServiceNow. [S38]

**What you need**

- A Zoom account with admin or developer rights, a Zoom app created in the Zoom App Marketplace, and licences for the Zoom products you use. [S37]
- Access to Claude's custom connectors, or to ChatGPT's Developer mode. [S37]

**Steps to connect** (Zoom developer docs, not dated)

1. In the Zoom App Marketplace, select **Develop**, then **Build app**, choose **General app** and click **Create**. [S37]
2. Click **Scopes**, then **Add scopes**, choose what the app may do and click **Done**. [S37]
3. For Claude, go to **Customize > Connectors**, click **+**, then **Add custom connector**. Enter the server URL and the app's client ID and secret, then click **Add**. [S37]
4. For ChatGPT, go to **Settings > Apps > Advanced settings**, turn on **Developer mode** and click **Confirm**. Then click **Create app** and enter the server URL and OAuth details. [S37]
5. Copy the callback address from Claude or ChatGPT into the OAuth redirect URL of your Zoom app. [S37]

**To disconnect**

- Zoom's MCP guide doesn't describe it. In Claude, a connector can be removed from **Customize > Connectors**. [S37] [S51]

**Limits**

- Zoom's remote MCP servers don't support automatic client registration, so each app has to be registered by hand. [S37]
- This route involves OAuth codes and tokens, so it suits someone with developer skills. That's our reading of Zoom's steps. [S37]

### Zapier and other Zoom Marketplace apps

**Official?**

- Yes. Zoom documents a Zapier integration that triggers actions in other apps when something happens in Zoom, or the other way round. [S54]

**What it can see and do**

- Zoom says it can link Zoom with services that have no direct integration. [S54]

**What you need**

- Admins can require approval before users add Marketplace apps. If you see **Request** instead of **Add**, an owner or admin has to approve the app. [S55]

**Steps to connect**

- Add the app from the Zoom Marketplace. [S55]

**To disconnect**

- In the Zoom Marketplace, click **My Library**, then the **More** icon next to the app, then **Remove**, and confirm. [S55]

**Limits**

- Zapier is a separate company with its own terms. We didn't read Zapier's own pages for this guide. [S54]

## Jobs it's good for

- **Minutes without a minute-taker.** Turn on meeting summary, check it, then share it with the people who were there. [S19]
- **Catching up when you join late.** Ask "Catch me up" in meeting questions. [S20]
- **Finding the moment in a recording.** Use smart recording's chapters and highlights, or ask Claude or ChatGPT to find where a topic came up. [S21] [S41]
- **Turning a meeting into a to-do list.** Ask Claude, ChatGPT or Copilot for the action items and let it create a Zoom document once you confirm. [S34] [S41] [S43]
- **Asking Copilot about past meetings.** Microsoft's Zoom Meetings connector lets hosts ask Copilot about their own recorded meetings. [S44]
- **A first draft of a reply.** Chat compose and email compose draft messages from the thread. [S17] [S13]
- **Your own notes in someone else's meeting.** My Notes works in Teams or Google Meet, once you've told the other people. [S14]

## What to watch for

**Tell people before AI listens**

- Zoom shows a lit AI icon for summaries and questions, and a banner, transcription icon and pencil icon for My Notes in Zoom meetings. [S11]
- People can choose not to see the My Notes banner again, so they may not see it in later meetings. [S11]
- Outside Zoom meetings, My Notes gives the other people no notice. Zoom reminds users to follow the law, which may include giving notice. [S14] [S26]
- Our note: whether you need people's consent depends on where you and they are. This isn't legal advice.

**Summaries travel**

- Anyone who gets a summary can save it and share it with apps and other people. [S19]
- If summaries start automatically, they begin when anyone starts the meeting, even without the host. [S19]
- The Zoom mobile app prompts people to switch on summaries, and tapping **Enable** turns on auto-start for all their meetings. [S19]

**Transcripts and recordings are the raw material**

- The Claude, ChatGPT and Copilot connections read the summaries, transcripts and recordings Zoom keeps. Keeping fewer transcripts leaves less for them to find. That's our inference. [S34] [S41] [S43]
- Set a retention period with **Delete transcripts after a specified number of days**. [S22]
- Microsoft's connector copies transcripts into your Microsoft 365 tenant. [S44] [S45]

**Who switches things on**

- Admins set AI features for the account or for groups, and can lock them. Users can change unlocked ones themselves. [S12] [S17]
- Hosts can turn off summaries and questions someone else started, and delete what was made so far. [S12]
- In Zoom meetings, hosts on desktop 6.7.5 or later can stop a participant's My Notes transcription. [S14]

**Where it's processed**

- Australian-hosted accounts use ZM+, yet Zoom's getting-started article says AI data may be processed in US data centres. [S9] [S17]
- Summary emails go through Twilio SendGrid in the US. [S18]
- AI-generated virtual backgrounds are checked by Amazon Rekognition in US data centres. [S18]

**Costs**

- ZoomMate's agents and third-party work use AI credits, and unused monthly credits expire. [S29]
- Accounts can allow overage, so set per-user credit limits. [S29]

**Check the output**

- Zoom says its AI may give "incorrect, inaccurate, misleading, or offensive responses". [S18]
- If you haven't set your pronouns, the AI picks them in summaries. [S19]

**Agents act for you**

- Zoom says ZoomMate "may take unintended actions", and that you're responsible for what it does. [S30]
- Zoom bans using ZoomMate for decisions with legal or similarly significant effects, such as employment or lending, with little or no human input. [S30]

## Announced changes

- **8 September 2025:** Zoom added an archive API for AI Companion conversations. [S7]
- **9 April 2026:** Zoom launched its Claude connector and a Zoom plugin for Claude Code. [S35]
- **18 May 2026:** Zoom expanded its MCP server and added a plugin for OpenAI's Codex. [S38]
- **1 June 2026:** ZoomMate launched in North America. EMEA and APAC were "expected to roll out later this year". [S5]
- **1 June 2026:** Zoom said ZoomMate's availability "may vary by customer type, region, and industry vertical at launch". [S56]
- **22 June 2026:** AI agents arrived in ZoomMate. Zoom AI On-Prem launched, with meeting summaries, Q&A and agentic search promised "later this year". [S6]
- **24 June 2026:** AI Companion's features were folded into Zoom Workplace under their functional names. [S4]
- **2 July 2026:** Zoom's developer changelog recorded that the AI Companion brand was retired. Planned search and ask APIs weren't released, and Zoom points to its MCP server instead. [S7]
- **Promotion:** Zoom Workflow Automation offers unlimited runs "for a limited time", and pricing may change afterwards. [S1]
- **Microsoft:** write actions through Copilot connectors start "early October 2026". [S45]

## What we couldn't establish

- **Whether ZoomMate is fully launched in Australia.** The June launch named North America only, but Zoom's Australian-dollar pricing page lists it. [S5] [S2]
- **GST.** Zoom's pages don't say whether the listed prices include GST. [S1]
- **Prices for Pro Plus, Business Plus and Enterprise Plus.** These plans appear in support articles but not on the pricing pages we read. [S19] [S1]
- **Which setup your account uses.** Zoom says AU-hosted accounts use ZM+, and that customers should ask Zoom support which deployment they have. An Australian business could be on Zoom's US-based cluster instead. [S9] [S15]
- **Where Zoom AI runs for Australian accounts.** The whitepaper describes ZM+ for AU-hosted accounts, while the support article says data may be processed in US-based data centres. [S9] [S17]
- **How long meeting summaries are kept.** Transcripts have a retention setting, but the pages we read give no retention period for summaries. The privacy statement says data is kept "as long as required". [S22] [S32]
- **Whether AI features are on by default** for a new paid account. The pages we read don't say. [S17] [S12]
- **Who sees the Custom Message.** Zoom's whitepaper doesn't make clear whether it's shown to everyone in the meeting or only to the person turning the feature on. [S12]
- **Notice in Teams and Google Meet.** Zoom's article on Zoom AI joining third-party meetings doesn't describe any notice inside those meetings. [S24]
- **Microsoft's connector in Australia.** Microsoft only says the Zoom Marketplace app isn't available in the EU. [S44]
- **ChatGPT menu names.** Zoom's article says **Apps & Connectors**, while OpenAI's current help pages say **Plugins**. [S41] [S53]
- **Removing Zoom for ChatGPT.** Zoom's ChatGPT article says **Manage > Added Apps**, while its general Marketplace article says **My Library**. [S41] [S55]
- **Which Claude plans work with Zoom for Claude.** Neither Anthropic's listing nor Zoom's page says. [S33] [S34]
- **Zoom's MCP server addresses.** Zoom's per-product MCP pages wouldn't load for us. [S37]
- **Dates on Zoom's support articles.** We took their last-modified dates from each page's metadata. [S17]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Zoom Workplace Pricing | Zoom | https://zoom.us/pricing | No date shown (©2026). Read from Perth in a browser with the currency set to Australian dollars | 17 Oct 2026 |
| S2 | ZoomMate Pricing | Zoom | https://zoom.us/pricing/aic | No date shown. Read with the currency set to Australian dollars | 17 Oct 2026 |
| S3 | My Notes Pricing | Zoom | https://zoom.us/pricing/my-notes | No date shown. Read with the currency set to Australian dollars | 17 Oct 2026 |
| S4 | Meet ZoomMate: Zoom's next chapter in AI | Zoom blog | https://www.zoom.com/en/blog/zoom-ai-companion-zoommate/ | 24 Jun 2026 | 17 Oct 2026 |
| S5 | Zoom launches ZoomMate: the first AI teammate built to turn conversations into completed work | Zoom (press release) | https://news.zoom.com/zoom-launches-zoommate/ | 1 Jun 2026 | 17 Oct 2026 |
| S6 | Zoom introduces AI agents as part of ZoomMate and Zoom AI On-Prem for regulated enterprises | Zoom (press release) | https://news.zoom.com/zoom-introduces-ai-agents-as-part-of-zoommate-and-zoom-ai-on-prem-for-regulated-enterprises/ | 22 Jun 2026 | 17 Oct 2026 |
| S7 | AI Companion Changelog | Zoom Developer | https://developers.zoom.us/changelog/ai-companion/ | Dated entries, latest 2 Jul 2026 | 17 Oct 2026 |
| S8 | Zoom AI Whitepaper | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper | "Last updated: September 25, 2026" | 17 Oct 2026 |
| S9 | Models, Processing, Storage, and Usage (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/models-processing-storage-and-usage | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S10 | Data Governance and Privacy (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/data-governance-and-privacy | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S11 | User Transparency and Notice (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/user-transparency-and-notice | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S12 | Administrative Controls (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/administrative-controls | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S13 | Zoom AI Features (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/zoom-ai-features | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S14 | My Notes (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/my-notes | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S15 | Feature Availability Table (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/feature-availability | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S16 | ZoomMate (Zoom AI Whitepaper) | Zoom (Zoom Library) | https://library.zoom.com/ai/ai-whitepaper/zoommate | No date on the page (whitepaper last updated 25 Sep 2026) | 17 Oct 2026 |
| S17 | Getting started with Zoom AI features | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0057623 | Last modified 15 Oct 2026 (page metadata) | 17 Oct 2026 |
| S18 | How Zoom AI features handle your data | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0057861 | Last modified 30 Sep 2026 (page metadata) | 17 Oct 2026 |
| S19 | Using Meeting Summary with AI | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0058013 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S20 | Asking in-meeting questions with AI | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0057748 | Last modified 24 Sep 2026 (page metadata) | 17 Oct 2026 |
| S21 | Using smart recording with AI | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0061101 | Last modified 5 Oct 2026 (page metadata) | 17 Oct 2026 |
| S22 | Enabling or disabling meeting transcripts | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0085675 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S23 | Customizing the recording consent disclaimer | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0068402 | Last modified 24 Sep 2026 (page metadata) | 17 Oct 2026 |
| S24 | Enabling or disabling Zoom AI to join third-party meetings for meeting summaries | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0080357 | Last modified 14 Oct 2026 (page metadata) | 17 Oct 2026 |
| S25 | Enabling or disabling the My Notes feature | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0083850 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S26 | Using My Notes | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0083849 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S27 | Managing retention policies for My Notes | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0073651 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S28 | Managing Data & Storage location | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0066473 | Last modified 15 Oct 2026 (page metadata) | 17 Oct 2026 |
| S29 | Understanding and managing Zoom AI Credits | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0085614 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S30 | Using ZoomMate | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0083738 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S31 | Sub-processors | Zoom | https://www.zoom.com/en/trust/subprocessors/ | Effective 2 Oct 2026 | 17 Oct 2026 |
| S32 | Zoom Privacy Statement | Zoom | https://www.zoom.com/en/trust/privacy/privacy-statement/ | "Last updated: September 17, 2026" | 17 Oct 2026 |
| S33 | Zoom for Claude (connector listing) | Anthropic | https://claude.com/connectors/zoom-for-claude | "Added April 2026" | 17 Oct 2026 |
| S34 | Zoom for Claude Connector | Zoom Developer Docs | https://developers.zoom.us/docs/mcp/plug-ins-and-connectors/claude-connector/ | No date shown | 17 Oct 2026 |
| S35 | Zoom unlocks meeting intelligence for AI workflows with Claude | Zoom (press release) | https://news.zoom.com/zoom-meeting-intelligence-in-claude/ | 9 Apr 2026 | 17 Oct 2026 |
| S36 | Using the Zoom Canvas for Claude connector | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0088594 | Last modified 11 Sep 2026 (page metadata) | 17 Oct 2026 |
| S37 | Connect to Zoom MCP Servers | Zoom Developer Docs | https://developers.zoom.us/docs/mcp/servers/connect-to-zoom-mcp-servers/ | No date shown | 17 Oct 2026 |
| S38 | Zoom connects conversations and organizational context across AI tools through expanded MCP capabilities | Zoom (press release) | https://news.zoom.com/zoom-mcp-expanded-capabilities/ | 18 May 2026 | 17 Oct 2026 |
| S39 | Zoom plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/zoom/ | No date shown | 17 Oct 2026 |
| S40 | ChatGPT plugin listing: Zoom | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69373a13116c819189d046aea1278836 | No date shown (version 2.0.0) | 17 Oct 2026 |
| S41 | Using the Zoom for ChatGPT app | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0083574 | Last modified 17 Sep 2026 (page metadata) | 17 Oct 2026 |
| S42 | Using the Zoom Whiteboard for ChatGPT connector | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0087802 | Last modified 22 Sep 2026 (page metadata) | 17 Oct 2026 |
| S43 | Using the Zoom for Cowork app | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0088547 | Last modified 11 Sep 2026 (page metadata) | 17 Oct 2026 |
| S44 | Zoom Meetings connector | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/zoom-connector | Updated 6 Oct 2026 (page metadata) | 17 Oct 2026 |
| S45 | Microsoft 365 Copilot connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview | Updated 12 Oct 2026 (page metadata) | 17 Oct 2026 |
| S46 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 30 Sep 2026 (page metadata) | 17 Oct 2026 |
| S47 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S48 | Use apps connected to Gemini with a work or school Google Account | Google Gemini Apps Help | https://support.google.com/gemini/answer/14959807?hl=en | No date shown | 17 Oct 2026 |
| S49 | Connect a third-party data source (Gemini Enterprise) | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/connect-third-party-data-source | "Last updated 2026-10-15 UTC" | 17 Oct 2026 |
| S50 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (17 Oct 2026) | 17 Oct 2026 |
| S51 | Get started with connectors | Anthropic (Claude docs) | https://claude.com/docs/connectors/getting-started | No date shown | 17 Oct 2026 |
| S52 | Managing app permissions in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001495-managing-app-permissions-in-chatgpt | "Updated: 15 days ago" (timestamp 2 Oct 2026, UTC) | 17 Oct 2026 |
| S53 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 8 hours ago" (timestamp 17 Oct 2026, UTC) | 17 Oct 2026 |
| S54 | Getting started with integrations | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0066581 | Last modified 16 Oct 2026 (page metadata) | 17 Oct 2026 |
| S55 | Adding and removing Marketplace Apps for personal use | Zoom Support | https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0062865 | Last modified 14 Oct 2026 (page metadata) | 17 Oct 2026 |
| S56 | Getting Started with ZoomMate | Zoom blog | https://www.zoom.com/en/blog/zoommate-getting-started/ | 1 Jun 2026 | 17 Oct 2026 |
