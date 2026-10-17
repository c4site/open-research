# Microsoft 365: the AI inside it, and the AI that connects to it

Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

A quick note on names before anything else. Microsoft now calls "Microsoft 365 Copilot" just "Microsoft Copilot", and "Microsoft 365 Copilot Chat" is now "Microsoft Copilot Chat" [S2][S3]. Microsoft says some screens and licences will keep the old names during the changeover [S3]. Its Australian price pages still use the old names, so you'll see both below [S12].

## The short version

Microsoft's main business plans include Microsoft Copilot Chat, a work-safe AI chat, at no extra cost [S2]. On its own it mostly answers from the web and from files you give it, though inside Outlook it can also read your inbox and calendar [S1][S3]. For Copilot to work across all your email, files, chats and meetings by itself, you need the paid add-on, which Microsoft's Australian page lists at AU$31.40 per user a month on a yearly plan, before GST [S12][S4]. Whichever version you use, Copilot only sees what the signed-in person can already open, so loose SharePoint sharing shows up in Copilot's answers [S6][S38]. Microsoft says your prompts and work data aren't used to train its foundation models [S6]. Copilot now runs some features on Anthropic's Claude models and on OpenAI-operated models, both switched on by default for most business customers, and an admin can turn either off [S7][S8]. ChatGPT and Claude both have official connections into SharePoint, OneDrive, Outlook and Teams [S59][S71]. Claude's needs a Microsoft admin's approval before anyone can connect, and ChatGPT's needs one for many of its actions [S71][S61][S62]. Google's everyday Gemini app has no Microsoft 365 connection on its list, while its business product, Gemini Enterprise, has one [S88][S82]. Staff who pay for a personal Microsoft 365 plan can use that Copilot on work documents unless an admin switches it off [S52].

## The tool, and the plans that matter

Microsoft 365 for business bundles Word, Excel, PowerPoint and Outlook with Teams, OneDrive, SharePoint and business email [S13]. The business plans top out at 300 users across the whole family of business plans, and Microsoft points bigger organisations to its enterprise plans [S13].

The AI comes in two layers. Copilot Chat is included with eligible work accounts at no extra cost [S2]. Work-grounded Copilot is a paid add-on, or comes built into the "with Copilot" bundles [S12].

### Business plans (Australian prices)

Per user per month, in Australian dollars, excluding GST, as shown on Microsoft's Australian pages on 15 October 2026 [S12][S13]. Microsoft says the GST-inclusive amount shows on the "Payment and Billing" page before you buy [S13].

| Plan | Paid yearly | Paid monthly | AI included | Source |
|---|---|---|---|---|
| Microsoft 365 Business Basic | AU$10.50 | AU$12.60 | Copilot Chat. Office apps on web and mobile only | [S16][S2] |
| Microsoft 365 Business Standard | AU$21.00 | AU$25.20 | Copilot Chat. Desktop apps included | [S14][S2] |
| Microsoft 365 Business Premium | AU$32.90 | AU$39.48 | Copilot Chat. Adds advanced security and device management | [S15][S2] |
| Microsoft 365 Apps for business | AU$15.80 | AU$18.96 | Desktop apps without Teams chat or calling. Not on Microsoft's Copilot Chat eligibility list | [S17][S13][S2] |
| Microsoft 365 Business Standard with Copilot | AU$35.20 | AU$42.24 | Copilot Business built in | [S12] |
| Microsoft 365 Business Premium with Copilot | AU$47.90 | AU$57.48 | Copilot Business built in | [S12] |
| Microsoft 365 Copilot Business (add-on) | AU$31.40, or AU$26.91 in the first year under a promotion | AU$37.68 | Add-on for an existing Business plan, up to 300 users | [S12] |

- Each plan has a cheaper "no Teams" version. Paid yearly: Basic AU$8.10, Standard AU$16.10, Premium AU$28.10, Standard with Copilot AU$30.40, Premium with Copilot AU$43.10 [S13][S14][S15][S16].
- The Copilot Business promotion runs from 1 July to 31 December 2026. It's only for existing customers on an eligible Business plan, needs an annual commitment, and the lower price applies to the first year only [S12].
- The Copilot plans have a one-month free trial. It needs a credit card and becomes a paid subscription unless you cancel during the trial [S12].
- Microsoft's documentation site now calls the add-on "Microsoft Copilot Business" [S5]. It can be added to Business Basic, Business Standard, Business Premium, Apps for Business and Teams Essentials [S5].

### Enterprise plans (bigger workplaces)

| Plan | Paid yearly, annual commitment, ex GST | AI | Source |
|---|---|---|---|
| Microsoft 365 E3 | AU$58.40 | Copilot Chat. Copilot add-on AU$44.90 per user a month, paid yearly | [S18] |
| Microsoft 365 E5 | AU$89.80 | Copilot Chat. Same Copilot add-on price | [S18] |
| Microsoft 365 E7 | AU$148.20 | Copilot included, plus Agent 365 | [S18][S39] |

E7 became generally available on 1 May 2026. Microsoft describes it as E5 with Copilot and Agent 365 added, along with the full Entra Suite [S39].

### Personal plans, and why they turn up at work

| Plan | Price shown | AI | Source |
|---|---|---|---|
| Microsoft 365 Personal | AU$16.00 a month or AU$159.00 a year | Copilot in the desktop apps, with usage limits | [S19] |
| Microsoft 365 Family | AU$18.00 a month or AU$179.00 a year | The same AI, for the subscription owner only | [S19] |
| Microsoft 365 Premium | AU$33.00 a month or AU$329.00 a year | Heavier AI use, plus "agentic" research and analytics | [S19] |

- On Family and Premium the AI belongs to the subscription owner and can't be shared with the others on the plan [S19].
- Copilot in Excel on these plans needs AutoSave on, so the file has to be saved to OneDrive [S19].
- AI use on personal plans runs on monthly "AI credits". Microsoft's help page doesn't give the amounts [S54].
- Researcher (covered below) comes with Microsoft 365 Premium and Pro, and isn't in Personal or Family [S27].
- Microsoft brought AI features into Personal and Family in Australia and changed their pricing in October 2024 [S20]. In November 2025 it apologised for not making clear that a cheaper "Classic" plan without Copilot was open to all subscribers [S20]. It quoted Classic at A$11 (Personal) and A$14 (Family) a month including tax, and said Classic "may not receive new feature updates" [S20].
- The part that matters at work: someone with a personal plan can use their personal Copilot on a work document in Word, Excel, PowerPoint, Outlook or OneNote, unless the organisation turns that off [S52][S53]. See "Personal Copilot on work files" below.

### What changed on 1 July 2026

- Microsoft raised list prices for most commercial suites from 1 July 2026. Its US-dollar table shows Business Basic going from US$6.00 to US$7.00, Business Standard from US$12.50 to US$14.00 and Apps for business from US$8.25 to US$10.00. Business Premium stayed at US$22.00 [S21].
- Existing customers keep their current price until renewal [S21].
- Standalone Copilot and Teams products weren't part of the change [S21].
- Alongside the increase, Microsoft said Business Basic, Standard and Premium would get Copilot Chat "enhancements", rolling out from June 2026. Those are inbox and calendar awareness plus Word, Excel and PowerPoint agents [S21][S22].
- The Australian prices in the tables above are what the pages showed on 15 October 2026 [S13][S14][S15][S16][S17]. We didn't find an Australian-dollar version of Microsoft's before-and-after table.

## AI built in

### Microsoft Copilot Chat

**What it does.** A chat assistant for work. It can research and summarise from the web, write and rewrite, analyse files you upload, make images and run agents [S1]. It answers mainly from the web [S1][S23]. It uses your organisation's content when you hand it over: by pasting it in, uploading a file with the **+** button, or typing **/** to pick a file you already have access to [S3]. It can also reach work content through Outlook (next section) and through agents your organisation pays for by usage [S3]. A model picker offers **Auto**, **Quick response** and **Think deeper** [S1].

**Where to find it.** At copilot.cloud.microsoft, in the Microsoft Copilot app on web, desktop and mobile, inside Outlook and Teams, in the Edge sidebar, and as Word, Excel and PowerPoint agents inside Chat [S2]. Signed in with a work account, you'll see a "Work" label under your profile and a green shield, which marks enterprise data protection [S2][S3]. A label such as **Copilot Chat (Basic)** tells you which version you have [S1][S2].

**Plans and cost.** No extra cost for work or school accounts on eligible plans. The list includes Business Basic, Business Standard, Business Premium, E3, E5, E7 and Teams Essentials [S2]. Without the paid licence you get "standard access", which Microsoft says "may be temporarily restricted" when demand is high [S24]. Agents built only from instructions and public websites are free [S31]. Agents that read shared company content, such as SharePoint, are billed by usage and start switched off. The billing runs through an Azure subscription [S31][S13].

**On by default, and who controls it.** It's pinned in the Microsoft 365 apps by default for most eligible users [S2]. An admin with the AI Administrator role can change that under **Copilot** > **Settings** > **Pin Microsoft Copilot Chat** [S56]. Since January 2026 the pin setting no longer controls the Copilot app itself [S56][S2]. Unpinning doesn't remove access either [S2]. Admins can block Copilot Chat for everyone or for chosen users and groups [S2]. They can also show blocked users a company policy page, set under **Copilot** > **Settings** > **View all** > **Custom link for blocked Microsoft Copilot app** [S2]. Web searching is controlled by the **Allow web search in Copilot** policy. With it off, Copilot answers from the language model alone [S2]. Copilot Pages and Notebooks are allowed by default, and admins control them through Cloud Policy [S57].

**Your data.** Prompts and responses are processed inside the Microsoft 365 service boundary under enterprise data protection, and aren't used to train the underlying foundation models [S3]. They're logged and stored in Exchange so admins can audit and search them [S3]. Files you upload are stored in your OneDrive [S3]. When Copilot searches the web, it sends Bing a short query of a few words with no user or tenant identifiers [S3]. Bing handles that query under the Microsoft Services Agreement, with Microsoft acting as an independent data controller [S3]. The exact search queries show in the answer's citations for 24 hours [S3].

**In Australia.** Sold here in Australian dollars [S12]. For tenants set up in Australia, Microsoft's Product Terms commit to storing Copilot Chat interaction content at rest in Australia. Copilot Chat joined that commitment on 1 September 2025 [S10]. Processing is a separate question. Microsoft says calls to the language model go to the nearest data centres but can move to other regions under heavy load [S3]. It also says customers outside the EU "may have their queries processed in the US, EU, or other regions" [S6].

### Copilot Chat in Outlook

**What it does.** Inside Outlook, Copilot Chat can answer questions about your emails, calendar, meetings and chats, plus a limited set of files [S3]. It can also act in Outlook: drafting an email, scheduling a meeting, flagging unread emails or setting up an automatic reply [S25]. The files it can reach are your OneDrive, files from SharePoint sites you visit often, files shared directly with you, and files you've viewed, edited or created [S3].

**Where to find it.** Sign in to Outlook with your work account and select the Copilot button near the top of the app [S25]. Microsoft's help page lists Outlook for Microsoft 365 on Windows and Mac, and the new Outlook for Windows [S25].

**Plans and cost.** No add-on needed for this limited version [S25][S1]. With the paid licence it reaches more of your organisation's data [S25].

**On by default, and who controls it.** It follows the Copilot Chat settings above [S2].

**Your data.** It finds your content with a simpler keyword index. The full semantic index and Work IQ are for licensed users only [S3]. It respects existing Microsoft 365 permissions [S1].

**In Australia.** Same storage and processing position as Copilot Chat [S10][S6].

### Copilot in Word, Excel, PowerPoint and OneNote

**What it does.** For users with in-app access but no add-on, Microsoft lists: drafting, rewriting and summarising in Word; analysing data and creating formulas and visuals in Excel; building and editing decks in PowerPoint; drafting plans and lists in OneNote; drafting and summarising email in Outlook; drafting questions in Forms [S4]. The Word, Excel and PowerPoint agents inside Copilot Chat can create new files. PowerPoint files are saved to your OneDrive, and Word and Excel files come back as downloads [S3]. In "Edit with Copilot", users can choose Claude where the admin allows Anthropic models [S7].

**Where to find it.** Inside each app. A label shows your version: **Microsoft 365 Copilot (Premium)** for the paid licence, **Microsoft 365 Copilot (Basic)** for standard access without it, and **Copilot Chat (Basic)** where in-app Copilot isn't available [S1][S4].

**Plans and cost.** Microsoft says the in-app experience "might vary" with your licensing and tenant setup [S1]. The paid licence gives priority access and grounds answers in your work data [S4]. Business Basic only has the web and mobile Office apps [S16].

**On by default, and who controls it.** If an admin turns off the privacy setting for connected experiences that analyse your content, Copilot stops working in Word, Excel, PowerPoint, Outlook and OneNote [S6].

**Your data.** The same commitments as Copilot generally. No foundation-model training, and only content the user can already access [S6][S1].

**In Australia.** Microsoft notes availability in its apps "may vary by market and customer licensing" [S12].

### Copilot in Teams meetings

**What it does.** Summarises the discussion, including who said what, and suggests action items. You can also ask it questions during or after the meeting [S26]. Microsoft's overview lists meeting summaries (up to 30 days) and transcription among the in-app features available without the add-on [S4].

**Where to find it.** In a meeting, select Copilot in the meeting controls [S26]. The organiser sets it in the meeting scheduler under **Online meeting options** > **Copilot and other AI**. There, **Allow Copilot and Facilitator** can be set to **During and after the meeting**, **Only during the meeting** or **Off** [S26]. Choosing **Off** also turns off recording and transcription for that meeting [S26].

**Plans and cost.** Intelligent recap comes with the Teams Premium add-on or a Microsoft Copilot licence [S26]. Microsoft's pricing page footnotes its Teams features with "Microsoft Teams license required" [S12].

**On by default, and who controls it.** The organiser controls Copilot for their own meetings, even without a licence [S26]. To ask Copilot about a meeting afterwards, live transcription has to be on during it [S26].

**Your data.** With **Only during the meeting**, untranscribed speech-to-text data and Copilot conversations are gone once the meeting ends [S26]. Teams chat messages are covered by Microsoft's Australian data-at-rest commitment [S10].

**In Australia.** No Australia-specific limits stated. Microsoft notes Copilot won't work in meetings hosted outside the participant's organisation [S26].

### Microsoft Copilot (the paid licence)

**What it does.** Answers across the emails, meetings, calendars, chats, documents, sites and files you have permission to open [S1]. It uses Microsoft Graph, Work IQ and a semantic index to find that material without you uploading it [S4]. Microsoft says Work IQ can be turned off, and answers then aren't enriched with your work context [S4]. It adds Copilot Search across Microsoft 365 and connected outside sources [S4]. Microsoft says Work IQ includes "Copilot Memory" to learn your style and preferences [S12].

**Where to find it.** copilot.cloud.microsoft, the Microsoft Copilot app, and the Office apps [S4].

**Plans and cost.** For Business plans it's Microsoft 365 Copilot Business: AU$31.40 per user a month paid yearly or AU$37.68 monthly, ex GST, for up to 300 users [S12]. Microsoft lists it with Copilot in the Office apps and Teams, the Researcher, Analyst and Facilitator agents, adoption analytics and "LLM model choice" [S12]. On enterprise plans the add-on is AU$44.90 a month paid yearly [S18]. The licence includes SharePoint Advanced Management, the oversharing toolkit covered under "What to watch for" [S36][S37].

**On by default, and who controls it.** An admin assigns licences in the Microsoft 365 admin center [S5]. Microsoft's Copilot controls cover pinning, image generation, agents, web search and removing access [S4]. Microsoft suggests the AI Administrator role so the job doesn't need a Global Administrator [S4].

**Your data.** Microsoft says prompts, responses and data reached through Microsoft Graph aren't used to train foundation models [S6]. Copilot only shows organisational data the user has at least view permission for [S6]. Microsoft says Copilot has opted out of the human-review abuse monitoring that Azure OpenAI offers [S6]. Interactions are stored as the user's Copilot activity history. Admins can search them and set retention in Microsoft Purview [S6]. Users can delete their own history from the My Account portal [S6][S55].

**In Australia.** Copilot has been part of Microsoft's Product Terms data-at-rest commitment since 1 March 2024, and Australia is one of the covered locations [S10]. In November 2025 Microsoft announced that Australian customers could have Copilot interactions processed in Australia by the end of 2025 [S9]. An editor's note dated 3 April 2026 moved that to the end of 2026 [S9].

### Researcher and Analyst

**What they do.** Researcher runs longer, multi-step research and returns a structured report with citations. It draws on the web and on the work files, emails, meetings and chats you can access [S27]. Analyst works on data you attach. It calculates statistics and picks out trends and outliers, with charts and tables where they help [S28].

**Where to find them.** In the Microsoft Copilot app, under **Agents**, select **Researcher** or **Analyst** [S27][S28]. In Analyst, select **+** then **Attach content** to add files [S28]. Microsoft also lists both under **Tools** in Copilot Chat [S32].

**Plans and cost.** Researcher needs the Copilot add-on for business users, or a Microsoft 365 Premium or Pro personal subscription [S27]. Analyst's help page doesn't name a licence, and Microsoft's pricing lists both agents with Copilot Business [S28][S12].

**On by default, and who controls it.** Microsoft treats both as part of core Copilot chat, so the agent settings don't apply to them [S32]. Analyst's help page says an admin may need to enable it [S28]. Claude in Researcher only appears once an admin allows Anthropic models [S27].

**Your data.** Microsoft says both run inside the Microsoft 365 commercial data-processing boundary [S32]. When someone picks Claude, Anthropic does the processing as a Microsoft subprocessor (see "Claude and OpenAI models running inside Copilot") [S7].

**In Australia.** We found no Australia-specific statement on either help page [S27][S28].

### Agents: Agent Builder, the Agent Store and Copilot Studio

**What they are.** Microsoft describes agents as custom versions of Copilot, set up with their own instructions and knowledge for a particular task [S32]. Copilot Chat users can build them in Agent Builder inside Copilot. Copilot Studio is the fuller tool for harder jobs [S31].

**Where to find them.** People find and add agents from the Agent Store in the Microsoft Copilot app [S32]. Admins see them on the **Agents** page and in the **Agent Registry** in the Microsoft 365 admin center [S32].

**Plans and cost.**
- Agents grounded only in instructions and public websites cost nothing extra in Copilot Chat [S31].
- Agents that read shared company content, such as SharePoint or connector data, are billed by usage and are off by default for Copilot Chat users [S31].
- Turning on that billing means an admin links an Azure subscription through a billing policy, with optional budgets and email alerts [S34].
- Licensed Copilot users don't need any of that [S31]. For them, Copilot Studio agents used in Copilot, Teams or SharePoint for answers and Graph grounding are "zero-rated" [S36].
- Otherwise Copilot Studio runs on Copilot Credits. Unused monthly capacity doesn't carry over, and going over can lead to "service denial" [S36].

**On by default, and who controls it.** Under **Agents** > **Settings** > **User access**, the default is **All users** [S33]. **Agent and plugin access** lets an admin block agents from outside publishers while still allowing Microsoft's and the organisation's own [S33]. **Sharing** decides who can share Agent Builder agents across the organisation [S33]. Agents published to the whole organisation need admin approval first [S32].

**Your data.** Microsoft warns that data processed by non-Microsoft agents and plugins "isn't subject to Microsoft agreements" [S33]. Admins can see each agent's permissions and terms under **Integrated apps** [S6].

**In Australia.** No Australia-specific limits stated on the agent pages we read [S31][S32][S33].

### Copilot Cowork

**What it does.** Carries out tasks for you across Microsoft 365. It can send emails, schedule meetings, create documents, post in Teams, manage files, and run tasks on a schedule or when something arrives [S29]. It asks before sensitive actions. The approve button carries the action's name, such as **Send** or **Post**, and a dropdown offers **Always allow** for the rest of that conversation [S30].

**Where to find it.** Open copilot.cloud.microsoft and select **Cowork** in the toggle next to Chat [S30]. It also works in Outlook and Teams [S30].

**Plans and cost.** It needs a Microsoft Copilot licence with usage-based billing switched on [S30]. It's billed in Copilot Credits as you use it [S35], and Microsoft's Australian pricing shows it as "Metered" [S12]. It's generally available for work accounts [S29].

**On by default, and who controls it.** Admins manage spending under **Copilot** > **Cost management** [S35]. Cowork can optionally use Anthropic models [S30].

**Your data.** For tenants whose default location is Australia, Microsoft commits to storing Cowork prompts and responses at rest in Australia [S11]. Working files and custom skills sit in OneDrive or SharePoint Embedded under those services' own commitments [S11].

**In Australia.** Available to Australian work tenants as far as the docs show [S11][S29]. Cowork for personal accounts is in preview in the US and Canada only [S54].

### Claude and OpenAI models running inside Copilot

**What it is.** Microsoft now runs some Copilot features on Anthropic's Claude models and on models operated by OpenAI, with both companies acting as Microsoft subprocessors [S7][S8]. Users can pick Claude in Researcher and in "Edit with Copilot" in the Office apps. Copilot Studio makers choose the model when they build an agent [S7]. Copilot shows an indicator when a Claude model is in use [S7].

**Where to find it.** Admins: Microsoft 365 admin center, **Copilot** > **Settings** > **View all** > **AI providers operating as Microsoft subprocessors** [S7][S8].

**Plans and cost.** Microsoft says Anthropic models are only in "applicable Microsoft 365 licensed experiences" [S4]. The pages we read mention no separate charge.

**On by default, and who controls it.** Anthropic models are on by default for most commercial customers, with the EU, EFTA and the UK as the exceptions [S7]. Australia isn't on that list of exceptions, so on our reading they're on for Australian business tenants unless an admin changes it [S7]. OpenAI-operated models have been on for all users of eligible commercial customers since 24 July 2026, unless an admin picks **No users** [S8]. An AI Administrator or Global Administrator can limit either provider to chosen users or groups, or turn it off [S7][S8]. Microsoft warns that some features stop working if you turn Anthropic off [S7]. A separate class called "Anthropic models with Data Retention" stays off until an admin opts in. Microsoft's examples are Claude Fable 5 and Claude Mythos 5 [S7].

**Your data.** For the standard Anthropic models, Microsoft's Product Terms and Data Protection Addendum apply, along with enterprise data protection [S7]. The Data Retention models work differently. Anthropic stores most inputs and outputs for up to 30 days, can keep flagged content for up to two years, and Anthropic's own commercial terms apply [S7]. For OpenAI-operated models, Microsoft says OpenAI offers zero data retention for the Responses API that Microsoft uses, subject to limitations [S8].

**In Australia.** Both providers are excluded from Microsoft's in-country processing commitments where those apply [S7][S8]. That matters once Microsoft's Australian in-country processing arrives, which it now expects by the end of 2026 [S9].

**Steps to switch Claude models on, or limit who gets them.** From Microsoft Learn, updated 18 September 2026 [S7]. You need the AI Administrator or Global Administrator role [S7].
1. In the Microsoft 365 admin center, select **Copilot** > **Settings** > **View all** [S7].
2. Select **AI providers operating as Microsoft subprocessors** [S7].
3. Under **Available subprocessors for your organization**, select **Anthropic**, then **Save** [S7].
4. Under **Choose who can access Anthropic models for Copilot and generative AI experiences**, pick the users or groups, then **Save** [S7].

To turn Claude off, the same page offers **Disable Anthropic as a Microsoft subprocessor** [S7]. For OpenAI-operated models, select **OpenAI** on that page, then under **Choose which users can access OpenAI operated models** pick **All users**, chosen users and groups, or **No users**, and **Save** [S8].

## Outside AI that connects

### ChatGPT and Microsoft 365 (the SharePoint, Outlook and Teams apps)

**Official?** Yes. OpenAI builds apps for ChatGPT called **SharePoint**, **Outlook Email**, **Outlook Calendar** and **Microsoft Teams** [S59][S62]. The SharePoint app also covers OneDrive for work or school. Personal OneDrive isn't supported [S61].

**What it can see and do.** It works as the connected person and only retrieves what their Microsoft account can already open [S61][S63].
- SharePoint: find files and pull summaries or comparisons from them. With actions an admin has enabled, it can create folders, upload or update files, manage sharing links and work with lists and pages [S61].
- Outlook Email: search and read messages, look up people and manage contacts [S62]. In shared or delegated mailboxes it can move messages and send plain-text email from the mailbox, where permissions and settings allow [S62]. OpenAI's release notes add that with Outlook connected, ChatGPT can draft an email in the chat and you choose whether to send it. That works on the web for Plus, Pro, Business and Enterprise [S91].
- Outlook Calendar: read events and availability. On supported shared calendars it can create, update, RSVP to, cancel or delete events [S62].
- Teams: search chats and channels, send or reply to messages, create chats or channels, manage Planner tasks and pull transcripts from eligible meetings [S63].
- ChatGPT may ask you to confirm before an action that changes content [S61][S63].

**What you need.**
- A ChatGPT plan that offers the app. OpenAI says availability depends on your plan, region, workspace and Microsoft settings, and these pages don't list the plans [S59][S61][S63].
- In ChatGPT Business, apps are on by default. In Enterprise and Edu workspaces, new apps generally start switched off until an admin turns them on [S64].
- A Microsoft work or school account [S61].
- A Microsoft Entra administrator to grant organisation-wide consent for the Microsoft Graph permissions some actions need [S62][S64]. Approving permissions doesn't switch actions on. A ChatGPT workspace admin does that separately [S62].
- Admin-managed "sync" for SharePoint or Teams (an index built ahead of time) is only for eligible Enterprise and Edu workspaces [S61][S63].

**Steps to connect.** From OpenAI's help pages, read 15 October 2026 [S60][S62].

Each person:
1. In ChatGPT, open **Settings** > **Plugins** and select the app. Older phone apps may still say **Apps** [S60][S59].
2. Select **Install plugin** if it's shown [S60].
3. Select **Connect** if prompted [S60].
4. Sign in with your Microsoft work or school account [S60][S61].
5. Review the requested permissions and finish the Microsoft authorisation [S60].

Admins, once per organisation:
1. A ChatGPT workspace owner or admin opens **Admin console**, picks the workspace and opens **Plugins** [S62].
2. Select **Configure Microsoft permissions**. Review each Microsoft Graph permission and the ChatGPT actions under it, and select only the ones your organisation will allow [S62].
3. Continue to Microsoft Entra (the older Apps page labels this **Review permissions in Microsoft Entra**) and sign in with an Entra admin account that can grant organisation-wide consent [S62][S61].
4. Check the organisation and the "ChatGPT / OpenAI, L.L.C." app are right, then select **Accept**. The Entra screen approves the whole request at once. There are no per-permission tick boxes [S62].
5. Back in ChatGPT, turn on the actions you want under **Actions** [S62].

**To disconnect.** Each person: **Settings** > **Plugins** > the app > the account's **⋯** menu > **Disconnect** [S60]. Disconnecting doesn't delete past conversations, saved files or memories [S60]. Admins can disable an app for the whole workspace from the Admin console's **Plugins** page [S59]. An Entra admin can also revoke the grant in Microsoft Entra. Actions that depend on it then fail until the approval is run again [S62].

**Limits.**
- Live SharePoint search doesn't support the narrower "Sites.Selected" permission. OpenAI offers its own site allowlist or deny list instead [S61].
- Admin-managed SharePoint sync asks for "Sites.FullControl.All", which OpenAI itself calls a broad permission for your Entra admin to review [S61].
- Files over 100 MB aren't supported, and files protected by encrypting sensitivity labels aren't indexed [S61].
- Broad email searches can come back incomplete, and attachments in shared mailboxes can't be fetched [S62].
- If your ChatGPT workspace keeps its data in Australia, you can't set up SharePoint or Teams sync. OpenAI lists only Europe, Japan and the US for those [S65]. That table doesn't apply to live connections [S65].
- On Free, Plus, Go and Pro, OpenAI may use information from apps for training if "Improve the model for everyone" is on. For Business, Enterprise and Edu it doesn't by default [S59].

### ChatGPT inside Excel, Word and PowerPoint (the "ChatGPT" add-in)

**Official?** Yes. OpenAI publishes a single add-in called "ChatGPT" on Microsoft Marketplace that works in Excel, Word and PowerPoint [S70].

**What it can see and do.** It sits in a sidebar beside the open file. It can create and edit content in that file and explain formulas [S70][S68][S69]. Microsoft's listing says it "can read and make changes to your document" and can send data over the internet [S70].

**What you need.** Any ChatGPT plan: Free, Go, Plus, Pro, Business, Enterprise, Edu or K-12, with usage limits [S70][S69]. For Business, Enterprise and Edu, use draws on the workspace's credits once flexible pricing applies [S69][S68].
OpenAI says the Excel and PowerPoint versions are available globally, with limited use on Free and Go [S68][S69].
For Word, workspace admins can switch it on or off in the ChatGPT admin console, and a Microsoft 365 admin must also allow the add-in. OpenAI set it to be on by default from 1 October 2026 [S90].

**Steps to connect.** From OpenAI's help pages, read 15 October 2026 [S68][S69].
1. Open Excel or PowerPoint, on desktop or web [S68][S69].
2. Go to **Home** > **Add-ins** [S68].
3. Search for **ChatGPT** and add it [S68].
4. Open ChatGPT from the ribbon and sign in with the ChatGPT account that has your plan [S68].

For Word, OpenAI's page has you open the add-in's Microsoft Marketplace listing and select **Get it now**, then open ChatGPT from Word's ribbon and sign in. If you use your organisation's ChatGPT workspace, select it [S90].

If your organisation blocks the store, a Microsoft 365 admin can deploy it from a manifest file: **Integrated apps** > **Deploy Add-in** > **Upload custom apps**, upload the file, then assign users or groups [S68][S69]. Where a ChatGPT workspace uses role-based access, an admin may need to enable it under **Workspace settings** > **Permissions & roles** [S68].

**To disconnect.** OpenAI says you can delete or download in-app data from the add-in's **Settings** [S70][S68]. Removing the add-in itself uses Microsoft's normal add-in controls, which these pages don't spell out.

**Limits.** Chats in the add-in don't sync with your ChatGPT history, and Memory isn't available [S70]. OpenAI warns it can make unintended edits, "including editing or deleting content" [S70]. Macros and VBA may not be fully supported [S68]. OpenAI notes that under Microsoft's marketplace terms, Microsoft "may have the ability to read" workbook content and prompts [S68]. OpenAI may keep some data logs for 30 days for safety and integrity [S68].

### @ChatGPT inside Microsoft Teams

**Official?** Yes, from OpenAI [S66].

**What it can see and do.** People mention @ChatGPT in a Teams conversation to ask for help, such as a draft project update based on the thread [S66]. It runs on its own service account, using company connections an admin sets up, and doesn't inherit each person's access to files or apps [S67]. Replies in shared conversations are visible to everyone in them [S66].

**What you need.** ChatGPT Business, Enterprise or Edu, set up by an admin [S66][S67]. OpenAI says @ChatGPT is available globally on those plans [S66]. The workspace needs credits [S67]. The person connecting the Teams tenant must be a ChatGPT workspace owner or admin, signing in with a Microsoft account that holds Global Administrator or Privileged Role Administrator [S67].

**Steps to connect.** From OpenAI's help page, read 15 October 2026 [S67].
1. In the OpenAI admin console, pick the workspace [S67].
2. Open **Agents**, select **@ChatGPT agents**, select **Add**, choose **Microsoft Teams** and follow the prompts [S67].
3. Sign in with the authorised Microsoft account, review the permissions and complete organisational consent [S67].
4. Select **Open Teams admin center**, open **Users and groups**, select **Install app** and pick the users or groups [S67].
5. Back in the admin console, wait for **Ready**, then select **Done** [S67].
6. In **New agent**, check the tenant matches, give it a name and select **Create agent** [S67].
7. Mention @ChatGPT in an approved Teams channel to test it [S67].

**To disconnect.** Turn @ChatGPT off in the agent's **Overview**, which keeps the setup. Or delete the agent, which removes its settings and service account but leaves the Teams app installed [S67].

**Limits.** Each company tool it uses has to be connected with an approved account, and that account's permissions decide what @ChatGPT can reach [S67]. A spending cap can be set per agent [S67].

### Claude and Microsoft 365 (the Microsoft 365 connector)

**Official?** Yes. Anthropic hosts a "Microsoft 365" connector and has completed Microsoft's publisher verification [S73]. It shows up in your Entra tenant as two apps, "M365 MCP Client for Claude" and "M365 MCP Server for Claude" [S71].

**What it can see and do.** It acts as each person, using delegated permissions, and only reaches what that person can already see [S71].
- Reads: SharePoint and OneDrive files (Word, Excel, PowerPoint, PDF and plain text, but not OneNote), Outlook email including shared mailboxes you have delegate access to, calendars, the Teams chats and channels you're in, and meeting transcripts [S71][S72].
- Write tools, off until enabled: send and forward email, manage drafts and inbox rules, create and update calendar events, create, update or delete OneDrive and SharePoint files (deleted items go to the recycle bin), and send Teams messages [S71][S72].
- Sending a Teams chat message or posting in a channel always asks the person to confirm [S72].

**What you need.** The connector is on all Claude plans: Free, Pro, Max, Team and Enterprise [S71]. You need a Microsoft Entra tenant "tied to a Microsoft Business plan". Personal Microsoft accounts like @outlook.com can't connect [S71]. A Microsoft Entra Global Administrator has to grant one-time consent for the tenant [S71]. On Team and Enterprise, a Claude organisation owner also has to add the connector first [S71].

**Steps to connect.** From Claude Help Center articles updated 14 October 2026 and 8 September 2026 [S71][S72].

Claude organisation owner (Team and Enterprise only):
1. Sign in to Claude [S71].
2. Go to **Organization settings** > **Connectors** [S71].
3. Click **+ Add**, then **All available** [S71].
4. Find **Microsoft 365** and click **Add to your team** [S71].

Microsoft Entra Global Administrator, once per tenant:
1. In Claude, go to **Customize** > **Connectors** [S71].
2. Find **Microsoft 365** and click **Connect** [S71].
3. Sign in with Microsoft 365 credentials [S71].
4. Accept the permissions, ticking the box to grant access on behalf of the whole organisation [S71].

An admin without a Claude account can do the same in Microsoft Entra instead, by adding the two service principals in Graph Explorer and opening an admin-consent link for each [S71].

Each person:
1. Go to **Customize** > **Connectors** [S72].
2. Find **Microsoft 365** and click **Connect** [S72].
3. Sign in with your Microsoft 365 work account [S72].

**To disconnect.** Each person: **Customize** > **Connectors** > **Disconnect** [S72]. Team and Enterprise owners can remove it for everyone in **Organization settings** > **Connectors** [S71]. An Entra admin can revoke single permissions on the "M365 MCP Server for Claude" enterprise app. Anthropic's table maps them, for example revoking Mail.Read blocks Outlook and revoking Sites.Read.All blocks SharePoint [S73]. People can also switch individual tools off under **Tool permissions** [S72].

**Limits.**
- SharePoint search covers the whole tenant within the person's permissions. You can't limit it to chosen sites, because "Sites.Selected" isn't supported [S71][S72].
- Email search skips the separate Online Archive mailbox [S71].
- Write tools can't handle attachments and have per-user limits [S71].
- Emails Claude sends carry a header marking them as agent-initiated. File, calendar and Teams writes aren't marked [S71].
- Calendar changes make Microsoft 365 send invitations or updates to attendees automatically [S71].
- Conditional Access policies based on location or sign-in frequency can block it, because the connector's server-side requests come from Anthropic's IP range, 160.79.104.0/21 [S71][S73]. Anthropic suggests excluding that range from those policies, and never from device compliance policies [S71].
- A connection lapses after 90 days without use, by default [S73].

**Data.** Anthropic describes the connector as a proxy. Your documents stay in your tenant and are fetched only when a question needs them. File content isn't cached [S73]. Tool results that become part of a saved chat are kept with the chat [S73]. On commercial plans, Anthropic doesn't train on your inputs or outputs by default [S79]. On Free, Pro and Max, chats are used for training if you allow it. Raw content from connectors is left out unless you paste it into the chat [S80]. Anthropic says its commercial customer data is stored in the US, and traffic may be routed to the US, Europe, Asia and Australia [S81].

### Claude inside Excel, Word, PowerPoint and Outlook (Claude for Microsoft 365)

**Official?** Yes. Anthropic publishes "Claude for Microsoft 365" (Excel, PowerPoint and Word in one listing) and a separate "Claude for Outlook" listing on Microsoft's marketplace [S77][S78].

**What it can see and do.**
- Excel: answer questions with cell-level citations, change assumptions while keeping formulas intact, track down errors and build models [S74].
- Word: edit selected text, make edits as tracked changes, work through comment threads and summarise another party's redlines [S75].
- Outlook (beta): sort the inbox, draft replies into Outlook's compose pane unsent, summarise threads and find meeting times [S76]. It never sends mail or invites by itself and doesn't ask for the Mail.Send permission [S76].
- One conversation can carry across all four apps [S77].

**What you need.** A paid Claude plan: Pro, Max, Team or Enterprise [S74][S75][S76]. Outlook needs Exchange Online and a one-time Microsoft Graph consent from a Global Administrator [S76]. Excel needs Excel on the web or a recent Microsoft 365 build on Windows or Mac. Excel 2016 and 2019, iPad and Android aren't supported [S74].

**Steps to connect.** From Anthropic's Claude docs (no date shown), read 15 October 2026 [S74][S76].

For yourself:
1. Open the "Claude for Microsoft 365" listing on Microsoft AppSource [S74].
2. Select **Get it now** [S74].
3. Open Excel, activate the add-in and sign in with your Claude account [S74].

For the whole organisation:
1. In the Microsoft 365 admin center, go to **Settings** > **Org Settings** > **User owned apps and services** and turn on **Let users access the Office Store** [S74].
2. Go to **Settings** > **Integrated apps** > **Add-ins** [S74].
3. Search AppSource for "Claude for Microsoft 365" [S74].
4. Assign it to the organisation or to chosen users or groups [S74].

For Outlook, add one more step. A Global Administrator opens Anthropic's admin-consent link, checks the Mail.ReadWrite, Calendars.Read, User.Read and offline_access permissions, and selects **Accept** [S76].

**To disconnect.** Chat history is stored in your browser and can be cleared from the add-in's **Settings** [S74][S76]. Removing a deployed add-in uses Microsoft's Integrated apps controls. Anthropic's pages don't list those steps.

**Limits and data.**
- Inputs and outputs are deleted from Anthropic's systems within 30 days, with exceptions set out in Anthropic's privacy centre [S74][S76].
- For Outlook, the Microsoft Graph access token stays in your browser and isn't sent to Anthropic, but mailbox content Claude reads becomes part of the prompt sent to Anthropic [S76].
- Add-in activity isn't in Enterprise audit logs and doesn't follow custom retention settings. Enterprise organisations using Anthropic's Compliance API get it there, in public beta [S74][S76].
- Anthropic warns that hidden instructions in outside files or emails can manipulate the add-ins, so use them with trusted content [S74][S75][S76].
- Excel macros and VBA aren't supported [S74].
- If your admins use Microsoft Entra Privileged Identity Management, Anthropic notes a known Microsoft issue that makes deployment from Integrated apps fail [S74].

### Gemini and Microsoft 365

**Official?** For the everyday Gemini app: no. Google's table of Connected Apps for the Gemini app runs to dozens of apps, including Dropbox and Zoho Mail, and none of them is a Microsoft app [S88]. You connect and disconnect the listed apps under **Customize** > **Connectors** on gemini.google.com [S87]. The Gemini app can also link a "custom app" through its MCP server, but only for people aged 18 or over in the US, signed in with a personal Google account [S89]. For Gemini Enterprise, Google's business AI product on Google Cloud: yes. Google documents generally available connectors for Microsoft Entra ID, SharePoint Online, OneDrive, Outlook and Teams [S82].

**What it can see and do (Gemini Enterprise).** It searches Microsoft 365 content and can take actions. SharePoint actions include uploading and sharing documents and creating list items and pages [S83]. Outlook actions include sending mail and creating or updating events, with replying and forwarding added in September 2026 [S82]. Teams actions include sending channel and chat messages [S82].

**What you need.** Gemini Enterprise on a Google Cloud project. Google's connector pages cover the Standard, Plus, Pay-as-you-go and Frontline editions and send Business edition customers to a separate help centre [S82]. On the Microsoft side you need an Entra app registration with a client secret and admin-approved API permissions [S84][S85]. For copying SharePoint data into Google's index, Google asks for either "Sites.FullControl.All" or the narrower "Sites.Selected" [S83].

**Steps to connect (SharePoint, admin only).** From Google Cloud docs updated 14 October 2026 [S84][S85].
1. In the Microsoft Entra admin center, go to **Entra ID** > **App registrations** > **New registration**. Name it and choose **Accounts in this organizational directory only** [S84].
2. Add the web redirect addresses Google lists, then create a client secret under **Certificates & secrets** [S84].
3. Under **API permissions**, add the Microsoft Graph and SharePoint permissions for the mode you want, with a SharePoint admin's consent [S84][S85].
4. In the Google Cloud console, open the Gemini Enterprise page, select **Data stores** > **Create data store**, search for **Microsoft SharePoint** and click **Select** [S85].
5. Choose **Federated search** or **Data ingestion**, then enter the client ID, client secret, tenant ID and SharePoint address, and finish the sign-in [S85].
6. If you like, include or exclude particular sites and folders [S85].

**To disconnect.** The Google pages we read don't give removal steps [S83][S84][S85].

**Limits.** Google warns that with federated search your query, which can contain parts of your conversation, goes to the outside system and falls under that system's terms [S83]. Uploads and downloads are capped at 50 MB [S83].

**Documented alternative for everyday Gemini users.** Google doesn't list a Microsoft 365 connection for the consumer Gemini app [S88]. Its custom-app route isn't open to Australians yet, and Google says it "does not control, monitor, or secure" third-party MCP servers [S89]. Google's documented route to Microsoft 365 is Gemini Enterprise [S82].

### Microsoft Copilot and your other tools (Copilot connectors)

**Official?** Yes, Microsoft's own. Its privacy page still calls them Microsoft Graph connectors [S6][S40].

**What they do.** Bring outside data into Copilot and Microsoft Search. "Synced" connectors copy content into Microsoft 365's index, and "federated" connectors fetch it live through MCP without copying [S40]. Microsoft lists over 100 ready-made connectors, including Box, Dropbox, Google Drive, Confluence, Salesforce, ServiceNow, Jira and Zendesk [S40]. They respect the source system's permissions [S40]. Copilot Chat can't write back to outside systems by default. Microsoft says write actions for federated connectors start "early October 2026" [S40].

**What you need.** An AI administrator in the Microsoft 365 admin center, plus credentials for the outside system [S41]. Copilot-licensed users get connector content in Copilot [S39]. Copilot Chat users reach it through usage-billed agents [S3][S31].

**Steps to connect.** From Microsoft Learn, updated 7 April 2026 [S41].
1. Sign in to the Microsoft 365 admin center [S41].
2. Choose **Copilot** > **Connectors** [S41].
3. On the **Connectors** tab, choose **Gallery** and select the source, such as ServiceNow Knowledge or Salesforce [S41].
4. Enter a name and the source's address, then choose how to sign in to it [S41].
5. Roll it out to a small group of users first [S41].
6. Choose **Create** [S41].

**To disconnect.** Not covered on the page we read. For self-serve connectors, Microsoft says the indexed content is removed when the user disconnects or the admin turns the connector off [S40].

**Limits.** Under **Custom setup** > **Users**, one option makes indexed data visible to **Everyone in the organization** [S41]. Quicker "incremental" crawls don't pick up permission changes, so Microsoft says to run full crawls regularly [S41].

### The MCP and API route (Work IQ)

**Official?** Yes. Microsoft offers the Work IQ API, which includes a remote MCP server, an agent-to-agent (A2A) endpoint and a REST API [S47]. MCP, the Model Context Protocol, is a standard way for an AI tool to use another system's functions.

**What it can do.** The Work IQ MCP server gives AI agents tools to read, create, update and delete Microsoft 365 items such as mail, calendar events, files, chats and sites, and to ask Copilot itself [S48][S47]. In Copilot Studio it's read-only until an admin turns on write operations [S49].

**What you need.** Usage-based billing. Work IQ API use is separate from Copilot licences [S47]. A Global Administrator does a one-time setup [S50]. Microsoft's quick-starts cover GitHub Copilot CLI, Microsoft Foundry and Copilot Studio [S49].

**Steps to connect (Copilot Studio, preview).** From Microsoft Learn, updated 16 June and 28 September 2026 [S50][S49].
1. A Global Administrator opens Graph Explorer, sets the method to **POST** and the address to the servicePrincipals endpoint, consents to Application.ReadWrite.All under **Modify permissions**, posts the Work IQ app ID and selects **Run query** [S50].
2. In Copilot Studio, open the agent's **Tools** tab and select **Add Tool** [S49].
3. Select **MCP**, then **Work IQ (Preview)**, then **Create new connection** and **Create** [S49].
4. Sign in, then select **Add and Configure** [S49].

**Limits.** It's a route for developers and admins, and the cost moves with usage [S47]. The Copilot Studio version is a preview [S49]. Microsoft's pages don't document connecting ChatGPT or Claude straight to it.

### Power Automate (the documented automation route)

**Official?** Yes, Microsoft's own [S42].

**What it does.** Cloud flows link Microsoft 365 and outside services so routine steps run by themselves [S46]. Copilot in Power Automate drafts a flow from a plain description [S46]. You can then ask it to change the flow or explain it [S46].

**What you need.** Microsoft 365 licences include Power Automate with standard connectors and up to 6,000 actions per user a day. Premium connectors and AI Builder credits aren't included [S45]. Power Automate Premium adds premium connectors and 5,000 AI Builder credits a month [S44].

**On by default.** Copilot in Power Automate is on by default in Australia, which Microsoft lists as a region with Copilot GPUs [S43]. Microsoft's pages disagree on switching it off. One says an admin can turn it off [S43]. The other says the admin has to contact support for a PowerShell script that works only at tenant level [S42].

**Steps to connect.** From Microsoft Learn, updated 18 September 2026 [S46].
1. Sign in to Power Automate at make.powerautomate.com [S46].
2. On **Home**, select **Create with Copilot** and describe the flow in **What will your flow do?** [S46].
3. Select the send arrow [S46].
4. Check the suggested trigger and actions, then select **Keep it and continue** [S46].
5. Fix any connection marked with a red exclamation mark [S46].
6. Select **Create flow**, finish off in the Copilot pane and select **Save** [S46].

**Limits.** Copilot here is tuned for English [S46]. Microsoft recommends testing a flow after saving it [S46].

### Personal Copilot on work files (multiple account access)

**Official?** Yes, a Microsoft feature [S52].

**What it can do.** Someone with Microsoft 365 Personal, Family or Premium can use their personal Copilot on a work document open in Word, Excel, PowerPoint, Outlook or OneNote [S52][S53]. It can answer questions about the open document, edit it, search the web if that's allowed, and draft from documents the person can access [S52]. It can't reach the organisation's Microsoft Graph or ask about other documents [S52].

**What you need.** A personal subscription and a work account signed in to the same app. Microsoft's page says to select your account profile in the app header, then **Add an account** [S53].

**Who controls it.** It's on unless an admin disables the Cloud Policy setting **Multiple account access to Copilot for work documents** [S52]. Microsoft says enterprise data protection still applies, because protection follows the account that opened the file [S52].

**In Australia.** Always off in Microsoft's government clouds. Nothing Australia-specific stated [S52].

## Jobs it's good for

- **Catching up after leave.** Copilot Chat in Outlook can answer questions about your inbox, calendar and meetings, and draft replies, without the paid add-on [S25][S3].
- **Meeting notes and actions.** Copilot in Teams summarises who said what and suggests action items. Turn transcription on if you want to ask about it later [S26].
- **First drafts and rewrites.** Ask Copilot in Word for a first draft or a tighter rewrite, then check it yourself [S4].
- **A quick look at a spreadsheet.** Ask Excel's Copilot for formulas or insights, or give Analyst a file and ask for trends and outliers. Microsoft lists Analyst among the agents that come with the paid licence [S4][S28][S12].
- **A deck from a document.** PowerPoint's Copilot can build a presentation from a prompt or existing content [S4].
- **A researched briefing with sources.** Researcher writes a cited report from the web and your work files. It needs the paid licence [S27].
- **A simple question-answering agent.** An agent built only from instructions and public web pages costs nothing extra in Copilot Chat. One that reads your SharePoint is billed by usage [S31].
- **Taking the busywork out of a hand-off.** Describe a flow in Power Automate, for example posting a Teams message when an email arrives, and Copilot drafts it [S46].
- **Finding a file when you don't know where it lives.** Claude's connector and ChatGPT's SharePoint app both search the SharePoint content the person can already open [S72][S61].
- **Reviewing a contract's changes.** Claude for Word can summarise another party's tracked changes and make its own edits as tracked changes for you to accept [S75].
- **Clearing an inbox with drafts you approve.** Claude for Outlook sorts unread mail and leaves drafts unsent for you to check [S76].
- **Bringing another system into Copilot.** A Copilot connector can make Salesforce, Jira or a Google Drive searchable from Copilot, within each person's permissions [S40][S41].
- **Checking for oversharing before you switch Copilot on.** SharePoint's data access governance reports show sites shared with the whole organisation or with lots of "Anyone" links. They're part of SharePoint Advanced Management, which comes with the Copilot licence [S38][S37].

## What to watch for

### Permissions decide what any AI can see

- Copilot shows anything the signed-in person has at least view permission for [S6]. Microsoft notes SharePoint's sharing settings start at the most permissive option [S38].
- Microsoft's oversharing toolkit, SharePoint Advanced Management, comes with the Copilot licence [S37][S39]. It includes a **Content Management Assessment** (SharePoint admin center > **Advanced Management** > **Start assessment**), data access governance reports, Restricted Access Control and Restricted Content Discovery, which hides chosen sites from Copilot without changing who can open them [S38].
- The outside connectors work the same way. Claude's connector searches every SharePoint site the person can open and can't be limited to chosen sites [S71]. ChatGPT's live SharePoint app can't use "Sites.Selected" either, though OpenAI offers its own site allowlist [S61].
- Some setups ask for very broad Microsoft permissions. ChatGPT's admin-managed SharePoint sync asks for "Sites.FullControl.All", and so can Gemini Enterprise's SharePoint ingestion [S61][S83].
- Copilot connectors have an option to show indexed data to everyone in the organisation [S41].

### Personal and work accounts get mixed up

- The Copilot app takes either a work or a personal account. Microsoft marks the work side with a "Work" label and the green shield, and gives each kind of account its own background colour [S2]. Admins can control personal sign-ins with Tenant Restrictions v2 [S2].
- Personal Microsoft 365 subscribers can use their own Copilot on work documents unless you disable **Multiple account access to Copilot for work documents** [S52].
- Claude's connector refuses personal Microsoft accounts [S71]. Anthropic's setting **Restrict verified-domain connectors to your enterprise** stops staff connecting a work Microsoft 365 account to a Claude account outside the organisation [S73].
- OpenAI notes that connecting a personal account doesn't give access to work-only files [S60]. A ChatGPT Enterprise organisation can ask OpenAI Support to stop work accounts being connected from workspaces outside the organisation [S59].

### Data and training

- Microsoft: your prompts and the work data Copilot reads through Graph aren't used to train foundation models [S6]. Web searches go to Bing under different terms, with Microsoft as an independent controller [S3].
- OpenAI: on Free, Plus, Go and Pro, information from apps can be used for training if "Improve the model for everyone" is on. Business, Enterprise and Edu aren't used by default [S59].
- Anthropic: commercial plans aren't used for training by default. Free, Pro and Max chats are if the person allows it, though raw connector content is excluded unless pasted in [S79][S80].
- Thumbs-up and thumbs-down buttons are worth knowing about. When someone rates a chat, Anthropic keeps the whole conversation for up to five years and may use it for training, even on commercial plans [S79]. Team and Enterprise owners can switch rating off with the **Rate chats** setting under **Organization settings** > **Data and Privacy** [S79]. Microsoft says it uses optional feedback to improve Copilot without using it to train the foundation models, and admins can manage feedback [S6].

### Where data is processed

- Copilot data at rest stays in Australia for Australian tenants under Microsoft's Product Terms [S10]. The language model calls can be processed elsewhere [S6].
- Claude and OpenAI-operated models inside Copilot are excluded from in-country processing commitments, and both are on by default for most business tenants [S7][S8].
- Anthropic stores its commercial customer data in the US [S81].
- A side note for schools: Microsoft's terms let it store Office 365 Education data in the EU or North America unless the school buys the Advanced Data Residency for Education add-on [S10].

### Accuracy and checking

- Microsoft says AI responses "aren't guaranteed to be 100% factual" and asks users to review before sending [S6].
- OpenAI says its add-in can edit or delete content you didn't mean it to, and to check formulas, numbers, citations and claims against primary sources [S70].
- Anthropic says Claude for Excel isn't recommended for final client deliverables without human review [S74].
- Researcher shows its sources so you can check them [S27].

### Hidden instructions in files and emails

- Anthropic warns that outside files and emails can carry hidden instructions that steer its add-ins into leaking data or making changes [S74][S75][S76].
- Microsoft says Copilot uses classifiers to block these "cross-prompt injection" attacks, but they "may not be available in all" Copilot scenarios [S6].
- OpenAI says its safeguards reduce prompt-injection risk without removing it [S64].

### Cost surprises

- The Copilot Business promotion only covers the first year [S12].
- Monthly billing costs more than yearly: AU$37.68 against AU$31.40 for Copilot Business [S12].
- Copilot plan trials need a credit card and roll into paid subscriptions [S12].
- Agents that read company data in Copilot Chat are billed through Azure by usage [S31][S13].
- Cowork and some other Copilot services are billed in Copilot Credits by usage, even for licensed users [S35].
- Spending policies for those services have **Auto-apply new services** on by default, so new metered services can fall under an existing budget automatically [S35].
- Copilot Studio credits don't roll over, and going over capacity can stop the service [S36].
- @ChatGPT in Teams needs workspace credits [S67].
- The ChatGPT and Claude add-ins draw on your ChatGPT or Claude plan limits [S68][S74].

### Admin settings worth looking at early

- **Copilot** > **Settings** in the Microsoft 365 admin center, including **Pin Microsoft Copilot Chat** and **AI providers operating as Microsoft subprocessors** [S56][S7].
- **Allow web search in Copilot** [S2].
- **Agents** > **Settings** > **User access**, which defaults to **All users** [S33].
- **Multiple account access to Copilot for work documents**, in Cloud Policy [S52].
- The Teams meeting option **Allow Copilot and Facilitator** [S26].
- Entra admin consent grants for ChatGPT, Claude or Gemini, which you can review or revoke later [S62][S71][S84].

### Microsoft's own pages don't always agree

- Microsoft's Australian business-plan FAQ says Copilot Chat "doesn't integrate with" files, emails or chats [S13]. Its documentation says Copilot Chat in Outlook can use your inbox, calendar, meetings and chats [S1][S3]. The documentation is more specific and carries 2026 dates; the FAQ shows no date [S1][S3][S13].
- The pinning page gives both 20 and 28 January 2026 as the date the pin setting stopped applying to the Copilot app [S56].
- The two Power Automate pages describe different ways to turn Copilot off [S42][S43].

## Announced changes

- **15 January 2025:** the Microsoft 365 (Office) app was renamed and moved to m365.cloud.microsoft. It's now the Microsoft Copilot app, and web addresses are consolidating at copilot.cloud.microsoft [S58][S2].
- **1 September 2025:** Copilot Chat interaction content joined Microsoft's data-at-rest commitment [S10]. Copilot Studio switched its billing unit from messages to Copilot Credits the same day [S36].
- **January 2026:** the **Pin Microsoft Copilot Chat** setting stopped controlling the Copilot app worldwide [S56][S2].
- **2026, undated on the pages we read:** "Microsoft 365 Copilot" became "Microsoft Copilot", and "Microsoft 365 Copilot Chat" became "Microsoft Copilot Chat", with a transition period [S2][S3].
- **1 May 2026:** Microsoft 365 E7 and Microsoft Agent 365 became generally available [S39][S51].
- **7 May 2026:** Claude for Excel, PowerPoint and Word reached general availability, and Claude for Outlook entered public beta [S77].
- **2 June 2026:** the free preview of ChatGPT for Excel ended for Business, Enterprise, Edu and K-12. Use then followed each plan's credits [S68].
- **8 June 2026:** ChatGPT could draft and send email through a connected Outlook or Gmail account, on the web for Plus, Pro, Business and Enterprise [S91].
- **17 September 2026:** ChatGPT for Word launched on all ChatGPT plans, using the same add-in as Excel and PowerPoint [S91][S90].
- **1 October 2026:** OpenAI's date for ChatGPT for Word to be on by default. Workspace admins can still switch it off [S90].
- **June 2026 onwards:** Copilot Chat enhancements for Business plans, rolling out over the northern summer [S21].
- **1 July 2026:** Microsoft 365 commercial list prices rose. Existing customers move at renewal [S21].
- **1 July to 31 December 2026:** Copilot Business first-year promotion in Australia [S12].
- **9 and 24 July 2026:** OpenAI-operated models became available in Copilot, then switched on by default [S8].
- **September 2026:** Gemini Enterprise added Outlook, OneDrive and Teams actions [S82].
- **Early October 2026:** write actions for federated Copilot connectors [S40].
- **By the end of 2026:** Microsoft expects local processing of Copilot interactions in Australia [S9].
- **31 December 2026:** Copilot Business promotion ends [S12].
- **No date given:** OpenAI says individually authorised app sync is no longer available, leaving admin-managed sync only [S65].
- **No date given:** Microsoft retired Deep Research for personal subscribers. Researcher replaces it for Premium and Pro, and Personal and Family subscribers keep old reports in their chat history [S27].

## What we couldn't establish

- **Which ChatGPT plans include the live SharePoint, Outlook and Teams apps.** OpenAI's pages say it depends on plan, region and workspace without naming the plans [S59][S61][S63]. Its release notes name Plus, Pro, Business and Enterprise only for sending email through Outlook [S91].
- **Which Business plans get in-app Copilot without the add-on.** Microsoft says the "Basic" in-app experience depends on licensing and tenant configuration, and doesn't map it to Business Basic, Standard or Premium [S1][S4].
- **Whether Apps for business users get Copilot Chat.** It qualifies for the Copilot add-on but isn't on Microsoft's Copilot Chat eligibility list [S5][S2].
- **What unlicensed users get in Teams meetings.** Microsoft's overview lists meeting summaries without the add-on, but the Teams help page doesn't say [S4][S26].
- **The dated announcement of the Copilot rename.** The notes on Microsoft's pages carry no date [S2][S3].
- **Whether in-country processing is live in Australia yet.** Microsoft's latest statement, from April 2026, says "expected" by the end of 2026 [S9].
- **Where Anthropic processes Copilot prompts.** Microsoft's page doesn't say. Anthropic's own commercial page describes its own products and doesn't mention the Microsoft arrangement [S7][S81].
- **Whether the Personal and Family Classic plans are still offered in Australia.** Microsoft's November 2025 notice doesn't say [S20].
- **The ACCC's court action.** The ACCC has a media release titled "Microsoft in court for allegedly misleading millions of Australians over Microsoft 365 subscriptions" (accc.gov.au). The ACCC's site blocked our request, so we couldn't read it or check the case's status.
- **Monthly AI credit amounts for personal plans.** Microsoft's page doesn't give figures [S54].
- **Gemini Enterprise Business edition.** Google covers it in a separate help centre we didn't reach, so we can't say whether its plan includes the Microsoft connectors [S82][S86].
- **Prices for Claude, Gemini Enterprise, Teams Premium, Copilot Studio and Agent 365 in Australian dollars.** Not checked against their official pricing pages.
- **ChatGPT prices in Australian dollars.** OpenAI's Business pricing page shows A$ headline prices next to fine print in another, unlabelled currency, so we haven't quoted them [S92].
- **Exact click paths** for blocking Copilot Chat and for removing a deployed add-in. The pages we read describe the result without the steps [S2].
- **Copilot Chat in Outlook on the web and on phones.** Microsoft's help page lists only Outlook for Microsoft 365 on Windows and Mac and the new Outlook for Windows [S25].
- **Whether ChatGPT or Claude can connect straight to Microsoft's Work IQ MCP server.** Microsoft documents GitHub Copilot CLI, Microsoft Foundry and Copilot Studio only [S49].
- **Other AI add-ins in Microsoft's marketplace.** We only checked OpenAI's and Anthropic's official listings [S70][S78].
- Our web-search allowance ran out near the end of this research. Pages we reached by direct address are cited. Anything we couldn't reach is listed above.

## Sources

All read on 15 October 2026. "Updated" is the date the page shows; for OpenAI's help centre that's a relative time ("4 days ago"), with our calculated date beside it.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Overview of Microsoft Copilot Chat | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/overview | 9 Sep 2026 | 15 Oct 2026 |
| S2 | Manage Microsoft Copilot Chat | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/manage | 12 Oct 2026 | 15 Oct 2026 |
| S3 | Microsoft Copilot Chat Privacy and Protections | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/privacy-and-protections | 18 Aug 2026 | 15 Oct 2026 |
| S4 | What is Microsoft Copilot? | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-overview | 14 Oct 2026 | 15 Oct 2026 |
| S5 | License Options for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-licensing | 25 Sep 2026 | 15 Oct 2026 |
| S6 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy | 9 Jul 2026 | 15 Oct 2026 |
| S7 | Anthropic models in Microsoft Online Services | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connect-to-ai-subprocessor | 18 Sep 2026 | 15 Oct 2026 |
| S8 | OpenAI as a subprocessor in Microsoft Online Services | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/openai-subprocessor | 9 Oct 2026 | 15 Oct 2026 |
| S9 | Microsoft offers in-country data processing to 15 countries to strengthen sovereign controls for Microsoft 365 Copilot | Microsoft AI at Work Blog | https://www.microsoft.com/en-us/copilot/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/ | Published 4 Nov 2025; editor's note 3 Apr 2026 | 15 Oct 2026 |
| S10 | Product Terms Data Residency | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/enterprise/m365-dr-product-terms | 8 Oct 2026 | 15 Oct 2026 |
| S11 | Data Residency for Microsoft 365 Copilot and Copilot Chat | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/enterprise/m365-dr-service-copilot | 8 Oct 2026 | 15 Oct 2026 |
| S12 | Microsoft 365 Copilot Plans and Pricing (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365-copilot/pricing | No date shown | 15 Oct 2026 |
| S13 | Microsoft 365 Pricing for Business: Plans & Features (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/business/compare-all-microsoft-365-business-products | No date shown | 15 Oct 2026 |
| S14 | Microsoft 365 Business Standard (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/business/microsoft-365-business-standard | No date shown | 15 Oct 2026 |
| S15 | Microsoft 365 Business Premium (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/business/microsoft-365-business-premium | No date shown | 15 Oct 2026 |
| S16 | Microsoft 365 Business Basic (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/business/microsoft-365-business-basic | No date shown | 15 Oct 2026 |
| S17 | Microsoft 365 Apps for business (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/business/microsoft-365-apps-for-business | No date shown | 15 Oct 2026 |
| S18 | Microsoft 365 Enterprise: Compare Plans and Pricing (Australia) | Microsoft | https://www.microsoft.com/en-au/microsoft-365/enterprise/microsoft-365-plans-and-pricing | No date shown | 15 Oct 2026 |
| S19 | Compare Microsoft 365 Plans & Pricing (Australia, home) | Microsoft Store | https://www.microsoft.com/en-au/microsoft-365/buy/compare-all-microsoft-365-products | No date shown | 15 Oct 2026 |
| S20 | An apology to our Microsoft 365 subscribers in Australia | Microsoft Source Asia | https://news.microsoft.com/source/asia/2025/11/06/an-apology-to-our-microsoft-365-subscribers-in-australia/ | 6 Nov 2025 | 15 Oct 2026 |
| S21 | Microsoft 365 Pricing and Packaging Updates | Microsoft Licensing | https://www.microsoft.com/en-us/licensing/news/2026-m365-packaging-pricing-updates | 16 Feb 2026 | 15 Oct 2026 |
| S22 | Advancing Microsoft 365: New capabilities and pricing update | Microsoft Copilot Blog | https://www.microsoft.com/en-us/copilot/blog/2025/12/04/advancing-microsoft-365-new-capabilities-and-pricing-update/ | Published 4 Dec 2025; updated 18 Mar 2026 | 15 Oct 2026 |
| S23 | How grounding works with a work or school account | Microsoft Support | https://support.microsoft.com/en-us/Microsoft-365-Copilot/how-grounding-works-with-a-work-or-school-account | No date shown | 15 Oct 2026 |
| S24 | Standard versus priority access to features in Microsoft Copilot Chat | Microsoft Support | https://support.microsoft.com/topic/standard-versus-priority-access-in-microsoft-365-copilot-chat-12c8d9f8-db32-4f99-8ebe-d8d85879137f | No date shown | 15 Oct 2026 |
| S25 | Chat with Copilot in Outlook | Microsoft Support (Australia) | https://support.microsoft.com/en-au/outlook/copilot-outlook/chat-with-copilot-in-outlook | No date shown | 15 Oct 2026 |
| S26 | Catch up on meetings with Microsoft Copilot in Teams | Microsoft Support (Australia) | https://support.microsoft.com/en-au/teams/copilot/catch-up-on-meetings-with-microsoft-365-copilot-in-teams | No date shown | 15 Oct 2026 |
| S27 | Get started with Researcher in Microsoft Copilot | Microsoft Support (Australia) | https://support.microsoft.com/en-au/microsoft-365-copilot/get-started-with-researcher-in-microsoft-365-copilot | No date shown | 15 Oct 2026 |
| S28 | Get started with Analyst in Microsoft Copilot | Microsoft Support (Australia) | https://support.microsoft.com/en-au/microsoft-365-copilot/get-started-with-analyst-in-microsoft-365-copilot | No date shown | 15 Oct 2026 |
| S29 | Copilot Cowork overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/ | 29 Sep 2026 | 15 Oct 2026 |
| S30 | Get started with Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/get-started | 14 Sep 2026 | 15 Oct 2026 |
| S31 | Agents for Microsoft Copilot Chat | Microsoft Learn | https://learn.microsoft.com/en-us/copilot/agents | 4 Feb 2026 | 15 Oct 2026 |
| S32 | Manage agents in the Microsoft 365 admin center | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/admin/manage/manage-copilot-agents-integrated-apps | 9 Jul 2026 | 15 Oct 2026 |
| S33 | Agent settings in Microsoft 365 admin center | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/admin/manage/agent-settings | 3 Sep 2026 | 15 Oct 2026 |
| S34 | Microsoft Copilot Pay-as-You-Go Service Overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/pay-as-you-go/overview | 17 Jul 2026 | 15 Oct 2026 |
| S35 | Usage-Based Billing and Cost Management for Copilot Credits | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/usage-based-billing-overview-copilot-credits | 30 Sep 2026 | 15 Oct 2026 |
| S36 | Standard harness licensing (Microsoft Copilot Studio) | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-copilot-studio/billing-licensing | 3 Aug 2026 | 15 Oct 2026 |
| S37 | Secure & Governed Data Foundation for Microsoft Copilot: Foundational Deployment Guidance | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/secure-govern-copilot-foundational-deployment-guidance | 6 May 2026 | 15 Oct 2026 |
| S38 | Get ready for Microsoft Copilot with SharePoint Advanced Management | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/get-ready-copilot-sharepoint-advanced-management | 16 Jul 2026 | 15 Oct 2026 |
| S39 | Prepare for Microsoft Copilot by comparing E3, E5, and E7 license features | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-license-feature-overview | 22 Jun 2026 | 15 Oct 2026 |
| S40 | Copilot connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview | 6 Oct 2026 | 15 Oct 2026 |
| S41 | Deploy connectors in the Microsoft 365 admin center | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/deployment-overview | 7 Apr 2026 | 15 Oct 2026 |
| S42 | Copilot in Power Automate | Microsoft Learn | https://learn.microsoft.com/en-us/power-automate/copilot-overview | 17 Aug 2026 | 15 Oct 2026 |
| S43 | Regions overview for Power Automate | Microsoft Learn | https://learn.microsoft.com/en-us/power-automate/regions-overview | 19 Aug 2026 | 15 Oct 2026 |
| S44 | Types of Power Automate licenses | Microsoft Learn | https://learn.microsoft.com/en-us/power-platform/admin/power-automate-licensing/types | 22 Sep 2026 | 15 Oct 2026 |
| S45 | Deep dive on specific licenses (Power Automate) | Microsoft Learn | https://learn.microsoft.com/en-us/power-platform/admin/power-automate-licensing/deep-dive-on-specific-license | 22 Sep 2026 | 15 Oct 2026 |
| S46 | Create your first cloud flow using Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/power-automate/create-cloud-flow-using-copilot | 18 Sep 2026 | 15 Oct 2026 |
| S47 | Work IQ overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/ | 25 Sep 2026 | 15 Oct 2026 |
| S48 | Work IQ MCP overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/mcp/overview | 5 Oct 2026 | 15 Oct 2026 |
| S49 | Work IQ in Microsoft Copilot Studio (GitHub Copilot) (preview) | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/add-work-iq | 28 Sep 2026 | 15 Oct 2026 |
| S50 | Enable your tenant for Work IQ | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/enable-work-iq | 16 Jun 2026 | 15 Oct 2026 |
| S51 | Microsoft Agent 365 overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-agent-365/overview | 19 Aug 2026 | 15 Oct 2026 |
| S52 | Multiple account access to Microsoft Copilot for work and school documents | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/multiple-account-access | 13 Apr 2026 | 15 Oct 2026 |
| S53 | Use Microsoft 365 Personal, Family, or Premium at work | Microsoft Support (Australia) | https://support.microsoft.com/en-au/microsoft-365-copilot/use-microsoft-365-personal-family-or-premium-at-work | No date shown | 15 Oct 2026 |
| S54 | How AI usage works across Microsoft 365 subscriptions for individuals | Microsoft Support | https://support.microsoft.com/topic/68530f1a-4459-4d02-9818-8233c1f673b8 | "Last updated October 2026" | 15 Oct 2026 |
| S55 | Delete your Microsoft Copilot activity history | Microsoft Support | https://support.microsoft.com/office/76de8afa-5eaf-43b0-bda8-0076d6e0390f | No date shown | 15 Oct 2026 |
| S56 | Pin Microsoft Copilot Chat in the Microsoft 365 apps | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/pin-copilot-chat-navbar | 26 Sep 2025 (page metadata shows a revision on 18 Sep 2026) | 15 Oct 2026 |
| S57 | Microsoft Copilot app settings for IT admins | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-app-admin-settings | 16 Sep 2025 (page metadata shows a revision on 11 Sep 2026) | 15 Oct 2026 |
| S58 | The Microsoft 365 app transition to the Microsoft Copilot app | Microsoft Support | https://support.microsoft.com/microsoft-365-copilot/the-microsoft-365-app-transition-to-the-microsoft-365-copilot-app | No date shown | 15 Oct 2026 |
| S59 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S60 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S61 | SharePoint app and setup in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12143177-sharepoint-app-and-setup-in-chatgpt | "10 days ago" (6 Oct 2026, UTC) | 15 Oct 2026 |
| S62 | Outlook Email and Calendar apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12512241-outlook-email-and-calendar-apps-in-chatgpt | "4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S63 | Microsoft Teams app and setup in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/12552368-microsoft-teams-app-and-setup-in-chatgpt | "23 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S64 | Admin controls, security, and compliance for plugins and apps | OpenAI Help Center | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S65 | Administrator-managed apps with sync in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/10847137-administrator-managed-apps-with-sync-in-chatgpt | "10 days ago" (5 Oct 2026, UTC) | 15 Oct 2026 |
| S66 | ChatGPT with Slack and Microsoft Teams | OpenAI Help Center | https://help.openai.com/en/articles/20001536-chatgpt-with-slack-and-microsoft-teams | "23 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S67 | Setting up and managing @ChatGPT in Slack and Microsoft Teams | OpenAI Help Center | https://help.openai.com/en/articles/20001538-setting-up-and-managing-chatgpt-in-slack-and-microsoft-teams | "23 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S68 | ChatGPT for Excel and Google Sheets | OpenAI Help Center | https://help.openai.com/en/articles/20001063-chatgpt-for-excel-and-google-sheets | "2 months ago" (16 Aug 2026, UTC) | 15 Oct 2026 |
| S69 | ChatGPT for PowerPoint | OpenAI Help Center | https://help.openai.com/en/articles/20001242-chatgpt-for-powerpoint | "17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S70 | ChatGPT (add-in for Excel, Word and PowerPoint, by OpenAI, LLC) | Microsoft Marketplace | https://marketplace.microsoft.com/en-us/product/WA200010215 | Version 2.0.0.1, updated 15 Sep 2026 | 15 Oct 2026 |
| S71 | Set up the Microsoft 365 connector | Claude Help Center (Anthropic) | https://support.claude.com/en/articles/12542951-set-up-the-microsoft-365-connector | 14 Oct 2026 ("Updated today") | 15 Oct 2026 |
| S72 | Connect to Microsoft 365 | Claude Help Center (Anthropic) | https://support.claude.com/en/articles/15183774-connect-to-microsoft-365 | 8 Sep 2026 | 15 Oct 2026 |
| S73 | Microsoft 365 connector security guide | Claude Help Center (Anthropic) | https://support.claude.com/en/articles/12684923-microsoft-365-connector-security-guide | 14 Oct 2026 ("Updated today") | 15 Oct 2026 |
| S74 | Use Claude for Excel | Claude Docs (Anthropic) | https://claude.com/docs/office-agents/excel | No date shown | 15 Oct 2026 |
| S75 | Use Claude for Word | Claude Docs (Anthropic) | https://claude.com/docs/office-agents/word | No date shown | 15 Oct 2026 |
| S76 | Use Claude for Outlook | Claude Docs (Anthropic) | https://claude.com/docs/office-agents/outlook | No date shown | 15 Oct 2026 |
| S77 | Collaborate with Claude across Excel, PowerPoint, Word and Outlook | Anthropic (claude.com) | https://claude.com/resources/articles/collaborate-with-claude-across-excel-powerpoint-word-and-outlook | 7 May 2026 | 15 Oct 2026 |
| S78 | Claude for Microsoft 365 (marketplace listing) | Microsoft Marketplace | https://marketplace.microsoft.com/en-us/product/WA200010725 | No date shown in the text we captured | 15 Oct 2026 |
| S79 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | 18 Aug 2026 | 15 Oct 2026 |
| S80 | Is my data used for model training? (consumer products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | 16 Mar 2026 | 15 Oct 2026 |
| S81 | Where are your servers located? Do you host your models on EU servers? | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996890-where-are-your-servers-located-do-you-host-your-models-on-eu-servers | 15 Jun 2026 | 15 Oct 2026 |
| S82 | Connect a third-party data source (Gemini Enterprise) | Google Cloud Documentation | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/connect-third-party-data-source | 15 Oct 2026 | 15 Oct 2026 |
| S83 | Microsoft SharePoint data store overview (Gemini Enterprise) | Google Cloud Documentation | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/ms-sharepoint | 14 Oct 2026 | 15 Oct 2026 |
| S84 | Microsoft SharePoint configuration (Gemini Enterprise) | Google Cloud Documentation | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/ms-sharepoint/third-party-config | 14 Oct 2026 | 15 Oct 2026 |
| S85 | Set up a Microsoft SharePoint data store (Gemini Enterprise) | Google Cloud Documentation | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/ms-sharepoint/set-up-data-store | 14 Oct 2026 | 15 Oct 2026 |
| S86 | Compare editions of Gemini Enterprise | Google Cloud Documentation | https://docs.cloud.google.com/gemini/enterprise/docs/editions | 14 Oct 2026 | 15 Oct 2026 |
| S87 | Use & manage Connected Apps in Gemini | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/13695044 | No date shown | 15 Oct 2026 |
| S88 | Check the availability & requirements of Connected Apps in Gemini Apps | Gemini Apps Help (Google) | https://support.google.com/gemini/table/17434654 | No date shown | 15 Oct 2026 |
| S89 | Connect & manage custom apps for Gemini Apps | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/17209137 | No date shown | 15 Oct 2026 |
| S90 | ChatGPT for Word | OpenAI Help Center | https://help.openai.com/en/articles/20001526-chatgpt-for-word | "27 days ago" (18 Sep 2026, UTC) | 15 Oct 2026 |
| S91 | ChatGPT release notes | OpenAI Help Center | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
| S92 | ChatGPT Business and Enterprise pricing | OpenAI | https://openai.com/business/pricing/ | No date shown | 15 Oct 2026 |
