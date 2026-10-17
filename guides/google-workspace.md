# Google Workspace: the AI inside it, and the AI that connects to it

Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

Every Google Workspace business plan now has Google's Gemini AI built in, and it's included in the plan price [S11][S1]. How much you get depends on the plan: Business Starter mostly gets Gemini in Gmail, while Business Standard and above add it to Docs, Sheets, Slides, Drive, Meet and Chat [S1]. Google says your Workspace content isn't read by human reviewers or used to train its AI models outside your organisation without your permission [S9]. Gemini only pulls from files and emails the signed-in person can already open, so loose sharing settings will show up in its answers (our inference from [S9]). There's no Australian data region: Google's data-regions setting offers the United States or Europe, and only on some plans [S10]. ChatGPT, Claude and Microsoft Copilot each have an official way to connect to Gmail and Google Drive, and some of these connections can now make changes as well as read [S75][S80][S84][S87]. Out of the box, a Workspace admin's settings let staff connect any third-party app to their work account, so it's worth setting rules early [S55]. Two defaults changed recently: Meet now takes AI notes automatically on Business Standard and Plus (from 29 September 2026), and Gemini's links to apps like HubSpot and Salesforce are switched on for people who have Gemini [S28][S50]. Google is replacing Gems with "skills", and on business plans Gems stop working no sooner than 1 March 2027 [S49]. Google's own help pages warn that Gemini can get things wrong, so check summaries and drafts before you rely on them [S17][S35].

## The tool, and the plans that matter

Google Workspace is Google's paid set of work apps, sold per user per month [S1]. This guide covers Gmail, Docs, Sheets, Slides, Drive, Meet, Calendar, Chat and Forms, plus the AI products Google sells alongside them [S1][S6].

**Business plans in Australia** (A$ per user per month, excluding tax, read 15 October 2026)

| Plan | Month to month | With a one-year commitment | Users |
|---|---|---|---|
| Business Starter | A$11.80 | A$9.90 | Up to 300 |
| Business Standard | A$23.60 | A$19.80 | Up to 300 |
| Business Plus | A$37 | A$30.90 | Up to 300 |
| Enterprise | Contact Google sales | Contact Google sales | No limit |

- The prices come from Google's Australian business and pricing pages [S2][S1].
- Google labels A$19.80 as the Business Standard price with a one-year commitment ("save 16%"); we've matched the Starter and Plus pairs the same way, which is our inference [S13][S2].
- The pricing page also showed introductory discounts for new customers when we read it, and its footnotes about how long they last didn't agree with each other, so check the price at sign-up [S1].

**What AI each plan gets** (Google's Australian pricing table) [S1]

| | Business Starter | Business Standard | Business Plus | Enterprise |
|---|---|---|---|---|
| Gemini in Gmail | Yes | Yes | Yes | Yes |
| Gemini in Docs, Sheets, Slides, Drive, Meet and Chat | No | Yes | Yes | Yes |
| Gemini in Vids | Yes | Yes | Yes | Yes |
| Gemini app | Basic access | Expanded access, incl. Google's most capable models | Expanded | Expanded |
| Gemini Notebook (formerly NotebookLM) | Basic, up to 3 Audio Overviews a day | Expanded, up to 20 a day | Expanded | Expanded |
| Workspace Studio (AI automations) | Yes | Yes | Yes | Yes |

- Enterprise also lists "AI classification for Google Drive" [S1].
- Google's feature table also lists a few Chat summary features ("AI Overviews") for all Business plans, so Starter may see some Gemini in Chat [S6].

**How Gemini came into the plans**
- In January 2025 Google folded its AI into Business and Enterprise plans so customers didn't need a separate Gemini add-on [S11].
- Existing customers' prices changed from 17 March 2025 for monthly plans, or at renewal for annual plans [S11].

**Add-ons and separate products**
- **AI Expanded Access**: a paid add-on that raises limits on advanced AI features, for Business Standard and Plus and Enterprise Standard and Plus [S12].
- It's sold in every country where Workspace is sold; Google's page shows no price, and online purchases are billed on the Flexible Plan [S12].
- Since 1 March 2026 it has been needed for higher use of advanced image generation and of video and avatar generation in Vids [S14].
- **AI Ultra Access** (formerly Google AI Ultra for Business) is the highest access tier [S14].
- **Gemini Enterprise** is a separate Google product and isn't included in a Workspace subscription [S63].

**Usage limits**
- AI limits apply to each person and aren't pooled across the organisation [S15].
- Daily limits reset at midnight US Pacific time, and monthly limits reset on the 1st [S15].
- Google's limits table shows "No access" for Business Starter on several Docs, Sheets, Slides and Drive AI features, such as the Sheets AI function and Drive audio overviews for PDFs [S15].

**Google Workspace for Education** (where it differs)
- The Gemini app and Gemini Notebook are core services in Education Fundamentals, Standard and Plus [S59].
- Google describes Gemini for Education as included free in all Workspace for Education editions [S58].
- Students under 18 get a separate experience with extra guardrails [S58].
- In primary and secondary schools, anyone not marked as 18 or older is treated as under 18 [S61].
- **Google AI Pro for Education** is a paid add-on that brings fuller Gemini into Workspace apps and higher limits [S58][S60].
- That add-on is only available to users aged 18 and over [S60].
- The Australian Gemini for Education page lists it at A$33.60 per user per month billed monthly, with lower one-year prices shown (A$28.00, and an asterisked A$21.00 that appears to be a discount) [S58].
- Without the add-on, Education Plus (and the Teaching and Learning add-on) gets smaller limits on some AI features, and Fundamentals and Standard get none for most of them [S60].

**Personal Google accounts**
- Staff who use Gemini with a personal Google account are covered by Google's consumer terms, and their chats may be reviewed by human reviewers [S8][S37].
- Google tells admins to warn people in that situation not to enter confidential information [S8].

## AI built in

### Gemini in Gmail

**What it does**
- Summarises long threads into bullet points and explains emails in simpler terms [S16].
- Drafts new emails, or rewrites your draft for tone and clarity ("Help me write") [S16][S17].
- Searches your inbox for details such as a booking time or a tracking number [S16].
- Archives, deletes, labels or stars emails for you, after showing a confirmation [S16].
- Uses Drive files you add with "Add sources" [S16].
- Creates, moves or deletes events on your primary calendar [S16].
- Google's feature table also lists AI Overviews for threads and for Gmail search, "Suggested replies" and "Proofread" [S6].

**Where to find it**
- Side panel: open Gmail on a computer, click "Ask Gemini" at the top right, type in the prompt box at the bottom, then click "Submit" [S16].
- Drafting: click "Compose" (or reply), type in the prompt bar at the bottom of the message, then click "Create"; if the bar isn't there, click the "Help me write" icon [S17].
- To adjust a draft, use "Formalize", "Friendly" or "Shorten", or type a new instruction [S17].
- The "Sources" icon shows which emails and Drive files Gemini used [S17].

**Plans and cost**
- Included in every Business and Enterprise plan, Business Starter included [S6][S1].
- No separate charge [S1].

**On by default, and who controls it**
- Gemini features in Workspace apps are on by default [S7].
- Admins can turn Gemini off app by app under Menu > Generative AI > Gemini for Workspace > "Feature access", but Google lists that panel for Enterprise Standard and Plus and some Education editions only [S7].
- Google's page doesn't say how Business Starter, Standard or Plus admins switch Gemini off in a single app [S7].
- Each person needs Workspace smart features turned on for Gemini to work in Workspace apps [S7][S54].

**Your data**
- Gemini only retrieves Workspace content the user already has access to [S9].
- Content isn't reviewed by humans or used to train generative AI models outside your domain without permission [S9].
- On supported editions, your existing data loss prevention (DLP) rules apply when Gemini's text goes into an email [S9].
- Gemini chat history in Workspace apps is kept separately for each app; admins can set automatic deletion or keep it [S9].

**Limits**
- It can't create new labels or handle requests that match more than 10,000 threads [S16].
- An action can only be undone within 60 seconds, or until you send another prompt [S16].
- It can't work with calendars other than your primary one [S16].

**In Australia**
- Google says work accounts can use "Help me write" globally in supported languages; the personal-account version is US-only [S17].
- "AI Inbox", a Beta feature, is limited to Enterprise Plus users in the United States [S53].

### Gemini in Google Docs

**What it does**
- Summarises your document, selected text, Drive files and Gmail emails [S18].
- Rewrites sections, changes tone, and adds facts from Drive, Gmail or the web [S18].
- Drafts new documents, and can create images, spreadsheets and presentations [S18].
- One-click changes on selected text: "Rephrase", "Shorten", and under "More", "Elaborate", "More formal" or "More casual"; also "Bulletize" and "Summarize" [S19].

**Where to find it**
- Click the "Ask Gemini" icon at the top right to open the side panel, then click "Insert" to keep an answer [S18].
- Or click the Gemini icon and type in the bar at the bottom; review changes with "Accept suggestion", "Accept all" or "Reject all" [S19].
- To edit selected text, click "Refine" on the floating bar [S19].
- To point Gemini at a file, click "Sources" or type "@" and pick the file [S19].
- To build a reusable instruction, click Tools > "Skill builder" [S18].

**Plans and cost**
- Business Standard, Business Plus, Enterprise Standard and Enterprise Plus; not Business Starter [S6][S1].
- No separate charge; matching writing style has a monthly cap [S15].

**On by default, and who controls it**
- On by default; same admin controls as Gmail [S7].

**Your data**
- Same Workspace commitments as Gmail [S9].
- When a file is shared outside your organisation, the side panel warns that prompts and AI content may be visible to outsiders, and Gemini stops drawing on your wider Drive and Gmail by default [S9].
- Feedback you send with the thumbs buttons may be read by people, so Google says to leave out personal or confidential details [S18].

**Limits**
- Side-panel history disappears if you refresh, close the file or go offline [S18].
- For web answers you need to ask, for example with "Use Google Search" [S18].

**In Australia**
- No Australia-specific limits in the pages we read; some languages aren't supported in the side panel [S18].

### Gemini in Google Sheets (including the AI function)

**What it does**
- Builds tables and formulas, fixes formula errors, and makes charts [S20].
- Analyses data and carries out sheet actions such as pivot tables, filters and conditional formatting [S20].
- Can bring in data through third-party connectors your admin has enabled [S20].
- The AI function, written as =AI("instruction", range), fills cells with generated text, summaries, categories or sentiment, and can use Google Search [S21].

**Where to find it**
- Click the "Ask Gemini" icon at the top right [S20].
- For the AI function: type it in a cell, or go to Insert > Function > AI; select the cells, then click "Generate and Insert" [S21].
- Use "Refresh and Insert" to run it again [S21].

**Plans and cost**
- Business Standard and Plus, Enterprise Standard and Plus [S6].
- Business Starter has "No access" to the AI function [S15].

**On by default, and who controls it**
- On by default; same admin controls as Gmail [S7].

**Your data**
- Same Workspace commitments [S9].
- The side panel warns that content added by Gemini may be visible outside your domain on shared files [S20].

**Limits**
- Works best on native Google Sheets; Excel files need converting first [S20].
- Charts Gemini makes don't update when the data changes [S20].
- The AI function returns text only and can't see the rest of the spreadsheet or other Drive files [S21].
- Only the first 350 selected AI cells run at once, and there's no undo [S21].
- Results don't refresh by themselves; you choose when to refresh [S21].

**In Australia**
- No Australia-specific limits in the pages we read [S20][S21].

### Gemini in Google Slides

**What it does**
- Generates images and new slides, summarises a deck, and rewrites text [S22].
- Uses Drive files you reference while writing [S22].

**Where to find it**
- Click "Ask Gemini" at the top right [S22].
- For images: Tools > "Create images", enter a prompt, click "Submit", then "Insert" [S22].
- For a slide: "Help me create a slide" from the toolbar, the Insert menu or the Slide menu [S22].
- In an empty text box: "Write a title" or "Help me write" [S22].

**Plans and cost**
- Business Standard and Plus, Enterprise Standard and Plus [S6].
- Generating whole presentations has a monthly cap; Business Starter has no access [S15].

**On by default, and who controls it**
- On by default; same admin controls as Gmail [S7].

**Your data**
- Same Workspace commitments [S9].

**Limits**
- Generated images are for use within Slides [S22].
- History is lost if you refresh, close the deck or go offline [S22].

**In Australia**
- No Australia-specific limits in the pages we read [S22].

### Gemini in Google Drive

**What it does**
- Summarises files and folders and researches a topic across several files [S23].
- Finds files using AI Overviews in search [S23].
- Suggests where to move loose files ("Suggest file moves"); it won't move anything without your permission [S24].
- Saves a set of source files as a "project" you can reuse in Docs, Sheets, Slides, Gmail, Chat and Meet [S25].
- Google's feature table also lists "Catch me up" and audio overviews for PDFs [S6].

**Where to find it**
- Click "Ask Gemini" at the top right [S23].
- In My Drive or a folder, click "Suggest file moves", review, then click "Move files" and "Create and move"; "Undo" reverses it [S24].
- For a project: click "New" > "New Project", or "Save as a project" from the full-screen Ask Gemini view [S25].

**Plans and cost**
- Business Standard and Plus, Enterprise Standard and Plus [S6].
- Audio overviews for PDFs and file organising have caps, and Business Starter has no access [S15].

**On by default, and who controls it**
- On by default; same admin controls as Gmail [S7].

**Your data**
- Same Workspace commitments [S9].
- Creating a project doesn't move files or change who can see them [S25].

**Limits**
- "Suggest file moves" works on the web only, in English only, and needs Editor access [S24].
- Since 20 April 2026 you can no longer ask the side panel to move files or create folders [S26].

**In Australia**
- File organising is English-only; no other Australia-specific limits in the pages we read [S24].

### Gemini in Google Meet ("Take notes for me" and more)

**What it does**
- "Take notes for me" writes meeting notes into a Google Doc with a short summary, decisions and action items [S27].
- People who join late can catch up with "Summary so far" [S27].
- Google's feature table also lists translated captions, speech translation, "Ask Gemini in Meet" and generated backgrounds [S6].

**Where to find it**
- In a meeting, click "Take notes for me" at the top right, then "Start taking notes" [S27].
- Before a meeting, in the Calendar event: "Video call options" > "Meeting records" > tick "Take notes with Gemini" [S27].

**Plans and cost**
- Business Standard and Plus, Enterprise Standard and Plus [S6].
- The meeting organiser's edition has to include it [S27].

**On by default, and who controls it**
- From 29 September 2026, automatic note-taking is on by default for Business Standard and Plus, and off by default for Enterprise [S28].
- Admins can choose all meetings, or only meetings with three or more people; staff can change their own default afterwards [S28].
- Admin settings live at Menu > Apps > Google Workspace > Google Meet > "Gemini settings" [S29].
- The default sharing setting sends notes to "Invited guests in your organization" [S29].
- Admins can require every participant to consent [S27].
- Everyone in the meeting is told notes are being taken, and a pencil icon appears [S27].

**Your data**
- Notes are saved in the organiser's Drive, in a "Google Meet" folder [S27].
- The Doc is emailed to the organiser and to whoever started the notes, and attached to the Calendar event [S29].
- Notes follow your organisation's Meet retention policy [S27].

**Limits**
- Supported languages are English, French, German, Italian, Japanese, Korean, Portuguese and Spanish, one per meeting [S27].
- Notes can be incomplete or missing for meetings under about 15 minutes or with connection problems [S27].

**In Australia**
- English is supported; no other Australia-specific limits in the pages we read [S27].

### Gemini for scheduling (Gmail and Calendar)

**What it does**
- "Help me schedule" suggests meeting times from your calendar inside an email; the recipient picks one and a Calendar invite goes to everyone [S30].
- It suggests four times by default and handles up to 20 guests [S30].
- Gemini in Gmail can also create, move or delete events on your primary calendar [S16].

**Where to find it**
- In a new email or reply, click "Help me schedule" at the bottom (or "More options" > "Help me schedule"), check the times, then click "Send" [S30].

**Plans and cost**
- Business Standard and Plus, and Enterprise plans [S6].

**On by default, and who controls it**
- On by default; same admin controls as Gmail [S7].

**Your data**
- Same Workspace commitments [S9].

**Limits**
- If you change the recipients after inserting the times, you need to insert them again [S30].

**In Australia**
- No Australia-specific limits in the pages we read [S30].

### Gemini in Google Chat

**What it does**
- Summarises conversations, including unread messages, in direct messages, spaces and threads [S31].
- Google's feature table also lists "Ask Gemini in Chat", answering questions and automatic translation for Business Standard and Plus [S6].

**Where to find it**
- Hover over a conversation in Home and click "Summarize", or open a conversation with unread messages and click "Summarize unread" [S31].

**Plans and cost**
- "AI Overviews" in Chat are listed for all Business plans; the other Chat features for Standard and Plus [S6].
- "Ask Gemini in Chat" is still a Beta feature [S53].

**On by default, and who controls it**
- Summaries are on by default in busy spaces for eligible users [S31].

**Your data**
- Same Workspace commitments [S9].

**Limits**
- No summaries for messages with apps or conversations with history turned off [S31].

**In Australia**
- Available in select languages only; no Australia-specific limits in the pages we read [S31].

### Gemini in Google Forms

**What it does**
- Builds a draft form from a description, or from a Doc, Sheet, Slides file or PDF you point it at [S32].
- Google's feature table also lists generating questions and summarising responses [S6].

**Where to find it**
- In a form, describe what you want and Gemini drafts it; you can retry or edit the prompt [S32].

**Plans and cost**
- Business Standard and Plus, Enterprise Standard and Plus [S32][S6].

**On by default, and who controls it**
- Needs smart features turned on [S32].

**Your data**
- Same Workspace commitments [S9].

**Limits**
- English only; no multi-section forms; inserting a draft replaces what's already in the form (you're warned first) [S32].

**In Australia**
- English-only; no other Australia-specific limits in the pages we read [S32].

### Google Vids

**What it does**
- Google's video maker; its AI options include AI avatars, AI voiceover, AI video clips, music and "Slides to Vids" [S6].
- The start menu offers "Create AI videos", "Edit videos" and "AI avatar" [S33].

**Where to find it**
- Open Vids from your Workspace apps; AI options appear in the start menu if your account has AI access [S33].

**Plans and cost**
- Vids AI features are listed for all Business plans, Business Starter included [S6][S1].
- Avatars, generated video seconds and music have monthly caps that rise with the plan [S15].

**On by default, and who controls it**
- Admins have a separate "Google Vids access" control [S7].

**Your data**
- Same Workspace commitments [S9].

**Limits**
- New Vids features roll out gradually [S33].

**In Australia**
- No Australia-specific limits in the pages we read [S33].

### The Gemini app with a work account

**What it does**
- A chat assistant at gemini.google.com and in the mobile app [S8].
- Features include Deep Research, Audio Overviews, image and video generation, Canvas, Gems and scheduled actions [S37].
- It can connect to your Workspace apps: find and summarise in Gmail, Drive and Chat; create and edit Calendar events; add tasks; and create Keep notes [S35][S34].
- Third-party apps available to work accounts include GitHub (web, 18+), Monday.com (18+, English) and WhatsApp (Android) [S38].
- Gemini in Chrome is covered by the same admin setting [S8].

**Where to find it**
- Go to gemini.google.com and sign in with your work account; type "@" in the box and pick an app such as Gmail or Drive, then ask [S35].
- A "Pro", "Expanded" or "Ultra" badge at the top shows your access level; no badge means standard access [S37].

**Plans and cost**
- A core service in Business Starter, Standard and Plus, and in Enterprise editions [S8].
- Business Starter gets basic access; Standard and above get expanded access and Google's most capable models [S1].
- Usage caps apply, for example on Deep Research reports and image generation [S8].

**On by default, and who controls it**
- Available by default to licensed users over 18 [S8].
- Admin switch: Menu > Generative AI > Gemini app > "Service status" [S8].
- Connections to Workspace apps are controlled under the same page's "Apps" section, and "Workspace apps" is on by default [S36].
- Google Chat as a source is off by default for users and admins [S34].
- Third-party apps such as Gemini for GitHub are managed through the Marketplace app allowlist [S36].

**Your data**
- On core-service editions, chats and uploads aren't reviewed by humans or used to improve AI models without permission [S8][S37].
- Chat history is kept for 18 months by default; admins can choose 3 or 36 months, or turn history off [S8].
- With history off, new chats are still kept for up to 72 hours [S9].
- Gemini in Chrome reads the address and content of tabs you choose to share [S9].
- Google's "Personal Intelligence" feature isn't available to Workspace accounts [S9].

**Limits**
- Work-account users must be 18 or over, except in Education editions [S37][S8].
- On the mobile app, Workspace users can't use Gems or Canvas [S8].
- For Business editions, the mobile app needs a business email address or a verified domain [S8].
- Through the Gemini app, Gmail can't create drafts or delete emails, and Drive can't move files [S35].
- If a prompt needs an app that's switched off, none of its actions run [S35][S36].

**In Australia**
- Australia is on Google's list of countries for the Gemini web app; the mobile app list may differ [S39].

### Skills (replacing Gems)

**What it does**
- Skills are reusable custom instructions you call in a chat by typing "/" and the skill's name [S49].
- They use an open Markdown format (SKILL.md), so instructions can move between tools [S49].
- Skills are replacing Gems, Gemini's earlier custom assistants [S49].

**Where to find it**
- In the Gemini app; in Docs, through Tools > "Skill builder" [S18][S49].

**Plans and cost**
- Gemini app skills: all Workspace editions and all ages [S48].
- Skills inside Workspace apps: Business Starter, Standard and Plus; Enterprise Standard and Plus; Google AI Pro for Education; AI Expanded Access; 18+ only [S48][S49].

**On by default, and who controls it**
- Admin setting for Workspace: "Allow people to use skills in Studio and Gemini in Workspace" [S48].
- There are no admin controls for skills in the Gemini app [S48].

**Your data**
- The skills pages we read don't add data terms beyond Google's general Workspace AI commitments [S9].

**Limits**
- Skills and Gems don't sync between the Gemini app and Workspace apps [S49].
- Gemini app skills began rolling out on 13 October 2026; skills inside Workspace apps are delayed "until further notice" [S48].

**In Australia**
- No Australia-specific limits in the pages we read [S48].

### Gemini Notebook (formerly NotebookLM)

**What it does**
- A research assistant that answers only from the sources you add, with citations [S3][S41].
- Turns sources into Audio Overviews, study guides, briefings and mind maps [S41].
- Takes PDFs, websites, YouTube videos, audio files, Google Docs and Google Slides [S41].
- Google renamed NotebookLM to Gemini Notebook on 16 July 2026; old links redirect [S4].

**Where to find it**
- notebook.google.com [S40].

**Plans and cost**
- A core service in Business Starter, Standard and Plus, Enterprise editions and Education editions [S40].
- Business Starter gets basic access (up to 3 Audio Overviews a day); Standard and above get up to 20 a day and five times more notebooks [S1].

**On by default, and who controls it**
- Admin switch: Menu > Generative AI > Gemini Notebook > "Service status" [S40].
- Google's page doesn't state the default [S40].

**Your data**
- Uploads, questions and answers aren't reviewed by humans or used to train AI models [S41][S40].
- When you add a Drive file, Gemini Notebook stores its own copy [S9].
- Your data-region settings don't apply to Gemini Notebook, and it isn't connected to Workspace DLP [S9][S10].
- Chat questions and answers aren't kept after the session; pin an answer as a note to keep it [S9][S3].

**Limits**
- People under 18 face stricter content rules, and some features are 18+ only [S41].

**In Australia**
- No Australia-specific limits in the pages we read; data regions don't cover it in any country [S10].

### Google Workspace Studio (AI automations)

**What it does**
- A no-code tool for building automations ("flows"): a starter (an event, a schedule or a button) followed by steps [S42].
- Steps can use Gemini, for example to recap unread emails and post the summary in Chat [S42].
- Flows can take actions in other services, such as Asana, Mailchimp, Salesforce, HubSpot and monday, through Beta integration steps [S43].
- Webhooks and custom steps written in Apps Script are also supported [S5].
- Workspace Studio grew out of the earlier "Workspace Flows" alpha [S5].

**Where to find it**
- Go to studio.workspace.google.com and browse templates on "Discover", or choose "Choose a Starter" to build your own [S42].
- Click "Test run", then "Start", then "Turn on" [S42].

**Plans and cost**
- Business Starter, Standard and Plus; Enterprise Standard and Plus; Education Fundamentals, Standard and Plus [S42][S45].
- Usage is on promotional access now; limits start being enforced on 1 November 2026 [S15].
- You can have up to 25 flows, with up to 20 steps each, and there's a daily cap on runs [S44].

**On by default, and who controls it**
- By default everyone in the organisation can create and use flows [S45].
- Admin switch: Menu > Apps > Google Workspace > Workspace Studio > "Flows" > "Create and use flows" [S45].
- Admins can require staff to approve steps that share data outside the organisation, under "Approvals" [S46].
- Google recommends using the Marketplace allowlist to control which integrations people can use [S47].

**Your data**
- Integration steps can pass Gmail, Chat or Calendar content to the outside service; Google advises only using services you trust [S43].
- A test run takes real actions [S42].

**Limits**
- Users marked as under 18 can't use AI steps [S45].
- Paid outside services need your own subscription [S43].

**In Australia**
- No Australia-specific limits in the pages we read [S42].

### Gemini integrations with other business apps

**What it does**
- From the Gemini side panel in Gmail, Docs, Sheets, Slides, Drive or Chat, you can look things up in Asana, Atlassian Rovo (Jira and Confluence), HubSpot, Mailchimp, Monday.com, QuickBooks or Salesforce [S52].
- These integrations only read for now; they can't change anything in the other app [S52].

**Where to find it**
- Open the Workspace Marketplace integrations page, pick the integration, click "Connect" and grant access [S52].
- Then click "Ask Gemini", type "@", choose the integration and ask your question [S52].

**Plans and cost**
- Google's admin page lists Business Standard and Plus and Enterprise Standard and Plus [S51].
- Some integrations need a paid subscription to the other app [S52].

**On by default, and who controls it**
- On by default for people with Gemini, according to Google's launch post [S50].
- Integrations are managed as Marketplace apps; Google says API controls can't restrict them [S51].
- If you later set one to "Blocked", people already using it can keep going [S51].

**Your data**
- Data flows to the other company while connected; deleting the connection stops it [S52].
- The pages we read don't say which company's terms cover that data [S51][S52].

**Limits**
- Some integrations need a helper app installed from the other service [S51].

**In Australia**
- No Australia-specific limits in the pages we read [S52].

### Gemini in Google Classroom (schools)

**What it does**
- For teachers: drafts lesson plans, quizzes and feedback, re-levels texts, and more [S62].
- For students: a "Gemini" tab with study help, plus Gemini Notebook tools such as flashcards and audio overviews [S62].

**Where to find it**
- Inside Classroom; students use the "Gemini" tab on the web and in the app [S62].

**Plans and cost**
- All Workspace for Education editions; some features, such as AI feedback on written work, need Education Plus or the Teaching and Learning add-on [S62].

**On by default, and who controls it**
- Admins must enable it and can limit who has it; students also need the Gemini app or Gemini Notebook turned on [S62].
- Age labels are set at Account settings > "Age-based access settings" [S61].

**Your data**
- Google says student data in Gemini for Education and Gemini Notebook isn't reviewed by humans or used to train AI models [S62][S58].

**Limits**
- Some teacher features are English-only [S62].

**In Australia**
- No Australia-specific limits in the pages we read [S59][S62].

## Outside AI that connects

### ChatGPT (Gmail and Google Drive apps) and Google Workspace

**Official?**
- Yes, built by OpenAI. OpenAI's docs describe a Gmail plugin and a Google Drive plugin that works across Drive, Docs, Sheets and Slides [S75].
- OpenAI's training site calls these connections "apps" and uses Google Drive as an example [S74].
- OpenAI's help centre also covers Google Calendar and Google Contacts apps, and its plugin directory lists Google Calendar [S93][S100].

**What it can see and do**
- OpenAI's examples include summarising today's unread Gmail threads and pulling notes from Google Drive [S75].
- OpenAI describes plugins as able to take actions in outside systems as well as read them [S75].
- Gmail: OpenAI's listing calls it "Read and manage Gmail", including drafting replies [S99]. With Gmail connected, ChatGPT can draft an email and you choose whether to send it. OpenAI's release notes say that works on the web for Plus, Pro, Business and Enterprise [S98].
- Google Drive: it searches and reads files the connected account can open, including Docs, Sheets and Slides. Where your workspace allows it, it can also create and update files, and share or delete them. ChatGPT may ask you to confirm first [S94].
- Google Calendar: OpenAI's listing says it can check availability and create, update or delete events [S100].
- Google Contacts: OpenAI's FAQ lists only read-only Google permissions for it [S93].
- In Business and Enterprise workspaces, admins can limit connections that support "Action control" to read-only actions or an approved set [S76].
- ChatGPT reaches only what the Google account you connect can open [S93]. A company-managed connection uses its own account's permissions, which can go beyond yours [S77].

**What you need**
- A ChatGPT plan that offers the apps. OpenAI's help pages say it depends on your plan, location, workspace and Google's settings, without listing plans [S94]. Its release notes name Plus, Pro, Business and Enterprise for recent Gmail features, such as sending email and connecting a second Google account. We couldn't confirm Free, Go or Edu [S98].
- In ChatGPT Business or Enterprise, the ChatGPT admin decides which apps are available [S74][S76].
- Business workspaces start with apps switched on, including Drive's Docs, Sheets and Slides actions. In Enterprise and Edu those Drive actions stay off until an admin turns them on [S97].
- On Google's side, the Workspace admin's API controls decide whether outside apps can reach Gmail and Drive [S55].
- A Google Workspace admin may need to approve the Google permissions behind each action ChatGPT has switched on. If one is blocked, people may see an error when they connect or use that action [S93].

**Steps to connect** (OpenAI help centre, read 15 October 2026)
1. In ChatGPT, go to "Settings", then "Plugins", and select Gmail, Google Drive or Google Calendar [S96].
2. Select "Install plugin" if you see it. This may start the sign-in [S96].
3. Select "Connect" if asked, and sign in to the Google account that holds the email or files you want [S96].
4. On Google's screen, approve the permissions. If ChatGPT says it needs them all, select "Try again" and choose "Select all" on Google's screen. To connect fewer Google apps, use "Select fewer apps" in ChatGPT [S96].
5. In a chat, type "@" and pick the app, or select "+" and choose it [S95][S75].

OpenAI Academy's page, last updated 4 September 2026, still shows an older route through "Settings" > "Apps" [S74]. OpenAI says very old versions of the phone apps may still show "Apps" [S95].

**To disconnect**
- To disconnect your Google account in ChatGPT: "Settings" > "Plugins" > the app > the account's "•••" menu (or "Connection") > "Disconnect" [S96].
- Open the plugin and choose "Uninstall plugin" where it's offered; workspace-installed plugins are managed by admins [S75].
- OpenAI's help centre warns that uninstalling a plugin can disconnect all the accounts connected through it. Its Learn docs add that a separately connected integration stays connected [S96][S75].
- Disconnecting doesn't delete past chats or saved memories, and it leaves any admin-managed Drive index in place [S93].
- On Google's side, go to myaccount.google.com/linkedapps > "Access to your Google Account" > the app > "See details" > "Remove access" > "Confirm" [S57].

**Limits**
- OpenAI says information accessed through these connections isn't used to train models for Business, Enterprise and Edu customers [S76][S74].
- On every plan, OpenAI says it doesn't train its general models on data from connected Google apps. The exceptions are feedback you send and anything that ends up in the chat itself, such as pasted content or ChatGPT's reply [S93].
- With "Improve the model for everyone" turned off, OpenAI says app data isn't used to improve its models, even when it appears in your chats [S93].
- The connected service's own retention and data-residency rules also apply [S76].

### ChatGPT for Google Sheets and Google Workspace

**Official?**
- Yes. The "ChatGPT" add-on in the Google Workspace Marketplace is published by OpenAI; the listing was updated on 1 June 2026 and shows more than 3 million installs [S79].

**What it can see and do**
- Works in Google Sheets only, in a sidebar, to build, edit and analyse spreadsheets from plain-language requests [S79].
- Can pull in context from your ChatGPT apps, such as Gmail [S79].
- You can upload "Skills" for jobs you repeat [S79].

**What you need**
- ChatGPT Free, Go, Plus or Pro; OpenAI also lists Business, Enterprise, Edu and K-12 users [S79]. OpenAI says it's available globally, with limited use on Free and Go [S101].
- Your Workspace admin has to allow Marketplace installs, or allowlist this add-on [S56].
- If your ChatGPT workspace uses role-based access, an admin may need to switch it on under "Workspace settings" > "Permissions & roles" [S101].

**Steps to connect**
1. Install the add-on from its Marketplace listing [S79].
2. Open a spreadsheet, then open ChatGPT from the "Extensions" menu. It appears in a sidebar [S101][S79].
3. Sign in with your OpenAI account [S79].

**To disconnect**
- Delete or download your data from the add-on's Settings [S79].
- Remove its access on your Google Account's linked apps page [S57].
- Admins can block it with the Marketplace allowlist or API controls [S56][S55].

**Limits**
- Memory isn't available, and sheet chats don't sync with your ChatGPT history [S79].
- It follows each person's ChatGPT training setting, and chats, attachments and workbook content may be shared with Google and OpenAI [S79].

### Claude (Gmail, Google Calendar, Google Drive, Docs, Sheets and Slides connectors) and Google Workspace

**Official?**
- Yes, built by Anthropic ("Google Workspace connectors") [S80].

**What it can see and do**
- Gmail: search and read emails, draft, send, reply and forward, and manage labels [S80].
- Google Calendar: view calendars, create, update and delete events, and find a time that suits everyone [S80].
- Google Drive: search and read Docs, Sheets, Slides, PDFs and Office files, upload files, create folders, and share, move or trash files [S80].
- Separate Docs, Sheets and Slides connectors can create new Google files and edit them live (beta) [S80].
- By default Claude asks for your approval before sending email or sharing, moving or trashing files [S80].
- Claude only sees data for the Google account you connect and can't reach anything that account can't open [S80].

**What you need**
- Anthropic says the connectors are available to all Claude users [S80].
- On Team and Enterprise plans, an Owner or Primary Owner must turn them on for the organisation first [S80].
- If your Workspace blocks unknown apps, a Google admin has to mark Claude as trusted [S80].

**Steps to connect** (Claude Help Center, "updated over 2 weeks ago" as of 15 October 2026)
1. In Claude, go to Customize > "Connectors" and click "+" next to Connectors [S81].
2. Choose Gmail, Google Calendar or Google Drive, read the description and click "Connect" [S81][S80].
3. Sign in to Google and approve access; Google's screen mentions permission to send email [S80].
4. In a chat, click "+", hover over "Connectors" and switch on the ones you want, including Docs, Sheets and Slides [S80][S81].

For Team and Enterprise owners, before step 1: Organization settings > "Connectors" > "Browse connectors" > "Add to your team" [S81].

For the Google admin, if access is blocked: admin.google.com > Security > Access and data control > API controls > Manage third-party app access, add the Claude app, set it to "Trusted", then wait about 15 minutes [S80].

**To disconnect**
- In Claude: Customize > "Connectors", select the Google connector, click "Disconnect" and confirm [S80].
- In Google: myaccount.google.com/connections, find Claude, and choose "Delete all connections" [S80].

**Limits**
- Claude can see attachment details from Gmail but can't read what's inside the attachments [S80].
- Claude reads text from Drive files but not the images inside them [S80].
- Files have to fit within the conversation's size limit [S80].
- The Drive connector can't add files to shared projects [S80].
- Anthropic says it doesn't train its models on Gmail, Drive or Calendar connector data; on consumer plans, content you paste from them may be used if you've opted in to training [S80].
- Team and Enterprise owners can set each tool to "Always allow", "Needs approval" or "Blocked" [S81].

### Claude for Google Docs, Sheets and Slides and Google Workspace

**Official?**
- Yes. The "Claude" add-on in the Workspace Marketplace is published by Anthropic; the listing was updated on 14 October 2026 [S82].
- Anthropic calls it beta [S83].

**What it can see and do**
- Adds a Claude sidebar that reads the open file and edits it in place; edits show in version history under your name [S83].
- In Docs it proposes changes as cards you accept or reject; in Sheets it builds models and fixes formulas; in Slides it creates and restyles slides [S83].
- It can use connectors your organisation has set up in Claude [S83].

**What you need**
- A Claude Pro, Max, Team or Enterprise plan [S83].
- A Google account that's allowed to install Marketplace apps [S83].

**Steps to connect** (Claude Help Center, "updated yesterday" as of 15 October 2026)
1. Open the Claude listing in the Workspace Marketplace and click "Install"; one install covers all three apps [S83].
2. Open a Doc, Sheet or Slides file and go to Extensions > Claude > "Open Claude" [S83].
3. Allow the two permissions Google asks for [S83].
4. Sign in to your Claude account in the sidebar [S83].

Admin install for the whole organisation: open the listing as a super admin, click "Admin install", then "Continue", choose everyone or specific groups, tick the agreement and click "Finish" [S83].

**To disconnect**
- Admins: Google Admin console > Apps > Google Workspace Marketplace apps > Apps list > "Claude" > "Uninstall app" [S83].
- Anthropic's page doesn't describe how an individual removes it [S83].

**Limits**
- Native Google files only; Office files need converting [S83].
- It only works in the file it's opened in and can't share files [S83].
- In Docs it can't read or resolve comments or accept suggestions [S83].
- Each task stops after six minutes; Firefox isn't supported [S83].
- Anthropic says it doesn't train on this content and deletes inputs and outputs within 30 days [S83].
- Pro and Max use falls under Anthropic's consumer terms; Team and Enterprise under its commercial terms [S83].
- Not for health information covered by HIPAA [S83].

### Microsoft 365 Copilot (Gmail, Google Calendar and Google Contacts) and Google Workspace

**Official?**
- Yes. Microsoft builds Gmail, Google Calendar and Google Contacts connectors for Microsoft 365 Copilot [S84].

**What it can see and do**
- Gmail: search and read messages, threads and labels [S84].
- Google Calendar: check events, invites and attendees [S84].
- Google Contacts: look up names, emails and phone numbers [S84].
- These are "federated" connectors: they fetch live data with your own sign-in and don't copy it into Microsoft 365 [S87].
- Write, update and delete actions started rolling out in early October 2026 for connectors that offer them, and each one needs your approval [S87].

**What you need**
- A Microsoft 365 work account with Copilot Chat [S87].
- Microsoft-published connectors are switched on in a Microsoft 365 tenant unless the admin turns them off [S87].
- Microsoft's pages we read don't say whether a paid Microsoft 365 Copilot licence is required (see gaps) [S87][S89].

**Steps to connect** (Microsoft Learn, 30 September 2026)
1. Open Microsoft 365 Copilot Chat [S87].
2. Select the "..." menu, then "Settings" [S87].
3. Select "Sources" in the left pane [S87].
4. Find Gmail (or Google Calendar or Google Contacts), select "Connect", and sign in [S87].
5. Ask your question in Copilot Chat [S87].

**To disconnect**
- Turn the source off in Copilot Chat settings or in the Researcher agent [S87].
- Microsoft 365 admins manage connectors under "Copilot connectors" > "Your connections" [S87].
- On Google's side, remove the app's access on the linked apps page [S57].

**Limits**
- The Researcher agent stays read-only [S87].
- Copilot can only see and change what your Google account is allowed to [S87].

### Microsoft 365 Copilot (Google Drive connector) and Google Workspace

**Official?**
- Yes. Microsoft builds a Google Drive connector that copies an index of Drive files into Microsoft 365 for Copilot and Microsoft Search [S85].

**What it can see and do**
- Lets people search and summarise Google Drive files from Copilot [S85].
- It keeps Google Drive's sharing permissions when set up as Microsoft recommends [S85].
- Comments and folder details aren't indexed [S85].

**What you need**
- A Google Workspace admin to create a Google Cloud service account with domain-wide delegation and read-only scopes [S86].
- A Microsoft 365 admin to deploy the connector [S86].

**Steps to connect** (Microsoft Learn, 18 November 2025)
1. Google admin: set up the service account and add the four read-only scopes Microsoft lists [S86].
2. Sign in to the Microsoft 365 admin center and select "Copilot" > "Connectors" [S86].
3. On the "Gallery" tab, select "Google Drive" [S86].
4. Enter a display name, your Google Workspace domain, an admin email and the service account key [S86].
5. Choose "Create"; indexing starts straight away [S86].

**To disconnect**
- Microsoft's deployment page doesn't describe removal (see gaps) [S86].

**Limits**
- Microsoft's default setting shows files that anyone can access in Google Drive to all Microsoft 365 users in your tenant [S86].
- Microsoft recommends "Only people with access to this data source" [S86].
- Permission changes only sync during the daily full crawl [S86].

### Microsoft Copilot for personal accounts and Google Workspace

**Official?**
- Yes. Microsoft's consumer Copilot can connect to Google Drive, Gmail, Google Calendar and Google Contacts [S90].

**What it can see and do**
- Finds files, emails, contacts and calendar events when you ask [S90].

**What you need**
- A personal Microsoft account, on Copilot.com or the Copilot mobile app [S90].

**Steps to connect** (Microsoft Support, no date shown)
1. In Copilot, select "Profile", then "Connectors" [S90].
2. Select "Connect" next to the service [S90].
3. Select "Continue to…" (for example "Continue to Gmail") [S90].
4. Choose the account and approve access [S90].

**To disconnect**
- Microsoft's page only covers switching connectors off per conversation ("+" > "Use connectors") [S90].
- Remove access fully on your Google Account's linked apps page [S57].

**Limits**
- Microsoft says connected data isn't used to train Copilot [S90].
- Whether staff can point this at a work Google account depends on your Workspace admin's third-party app settings (our inference from [S55]).

### Gemini Enterprise and Google Workspace

**Official?**
- Yes, a Google product, sold separately from Workspace [S63].

**What it can see and do**
- An AI assistant and company search tool that works across Google and third-party data, and hosts custom AI agents [S64].
- Prebuilt connectors include Microsoft SharePoint, OneDrive and Outlook, Jira Cloud, Confluence Cloud and ServiceNow, with many more listed [S66].

**What you need**
- A Gemini Enterprise licence; the Business edition covers 1 to 500 users [S65].
- An admin turns it on at Menu > Generative AI > Gemini Enterprise > "Service status" [S63].

**Steps to connect**
- Admins connect data sources and set access per source in Google Cloud; we didn't document the click path [S66].

**To disconnect**
- Set "Service status" to Off [S63].

**Limits**
- The Business edition falls under Google's general Terms of Service and Privacy Policy plus extra Business edition terms; Standard, Plus and Frontline fall under Google Cloud terms [S63].
- We found no Australian price or data-residency statement (see gaps) [S65].

### Google's MCP servers and OpenAI's API connectors (for developers) and Google Workspace

MCP (Model Context Protocol) is a standard way for an AI tool to plug into another service; Google describes its MCP servers as letting AI applications use Google services [S67]. These routes need a developer [S69][S78].

**Official?**
- Yes. Google runs MCP servers for Gmail, Google Drive, Google Calendar, Google Chat and the People API, all in "Developer Preview" [S68].
- OpenAI maintains Gmail, Google Calendar and Google Drive connectors in its API [S78].

**What it can see and do**
- Google's Gmail MCP server can search and read threads, list drafts and labels, create drafts and apply labels; it lists no tool for sending [S69].
- Google's Drive MCP server can search, read and download files, read permissions, and create or copy files [S70].
- OpenAI's Google connectors are built around searching and reading; the Drive one uses a read-only scope [S78].

**What you need**
- For Google's servers: membership of the Workspace Developer Preview Program, a Google Cloud project, and an OAuth client set up as "an AI-powered agent" [S69].
- Google's guide names Google Antigravity and Claude (Pro, Max, Team or Enterprise, as a custom connector) as clients [S69].
- For OpenAI's connectors: your own Google OAuth app supplying an access token [S78].

**Steps to connect** (Google for Developers, 12 October 2026)
1. Enable the Gmail API and the Gmail MCP API in your Cloud project [S69].
2. Set up the OAuth consent screen with the read and compose scopes [S69].
3. Create an OAuth client (Web application, "Use this client for an AI-powered agent") [S69].
4. Add https://gmailmcp.googleapis.com/mcp/v1 to your MCP client [S69].
5. Sign in and test [S69].

**To disconnect**
- Remove the server from your AI tool and revoke its access on your Google Account [S57].

**Limits**
- Google warns that emails can carry hidden instructions that hijack the AI session and lead to data being changed or stolen [S69].
- OpenAI tells developers to trust any server they connect and to keep approvals on for sensitive actions [S78].
- OpenAI's "connector_id" method is deprecated for models released after 1 September 2026 [S78].

### Apps Script and Workspace add-ons (build your own) and Google Workspace

**Official?**
- Yes. Apps Script is Google's JavaScript platform for building tools that work with Workspace [S71].
- Workspace add-ons are Google's documented way to extend Gmail, Calendar, Drive, Docs, Sheets, Slides, Forms, Chat, Meet and Workspace Studio [S73].

**What it can see and do**
- Apps Script can add menus and sidebars to Docs, Sheets and Forms, and connect to Gmail, Calendar and Drive [S71].
- Its Vertex AI service lets a script call Gemini models [S72].
- Add-ons can provide custom steps and starters for Workspace Studio [S73].

**What you need**
- For Gemini from Apps Script: a Google Cloud project with billing turned on and the Agent Platform API (formerly Vertex AI API) enabled [S72].

**Steps to connect**
- This is a route for developers, and there's no one-click connection; see Google's developer guides [S71][S73].

**To disconnect**
- Remove the script or add-on; admins can uninstall add-ons from the Marketplace apps list [S56].

**Limits**
- Google's pages we read don't state what Apps Script costs, beyond needing a billed Cloud project for AI calls [S71][S72].
- Apps Script data is covered by data regions (US or Europe only) [S10].

### Other AI add-ons in the Workspace Marketplace and Google Workspace

**Official?**
- Mostly not. A Marketplace search for "claude" returned around 100 apps, and only "Claude" itself was published by Anthropic [S91].
- A search for "chatgpt" showed "ChatGPT" by OpenAI and no Microsoft apps in the visible results [S92].
- Many of the rest offer GPT, Claude or Gemini inside Sheets, Docs or Gmail and are built by independent developers [S91].

**What it can see and do**
- Whatever access the person installing it approves (our inference from [S55]).

**What you need**
- Your admin's Marketplace and API settings decide whether staff can install them [S56][S55].

**Steps to connect**
- Install from the Marketplace listing. Check the publisher name first, because many similar-looking apps come from independent developers (our advice, based on [S91]).

**To disconnect**
- Remove access on your Google Account's linked apps page [S57].

**Limits**
- Marketplace listings link to each developer's own privacy policy and terms, as the ChatGPT and Claude listings do [S79][S82].

## Jobs it's good for

- **Catch up on a long email thread and reply.** Ask Gemini to summarise it, then use "Help me write". All Business plans [S16][S17][S6].
- **Book a meeting from an email.** "Help me schedule" offers times from your calendar and the other person books one. Business Standard and Plus [S30][S6].
- **Meeting notes without a note-taker.** "Take notes for me" in Meet saves a summary, decisions and action items to Drive. Business Standard and Plus [S27][S6].
- **Tidy a messy shared folder.** "Suggest file moves" in Drive proposes folders, and nothing moves until you accept [S24].
- **Sort customer comments in a sheet.** The =AI() function can categorise text or score sentiment down a column. Business Standard and Plus [S21][S6].
- **Turn a policy document into a form or quiz.** "Help me create" in Forms can start from a Doc or PDF (English only) [S32].
- **A Q&A for new starters.** Load the staff handbook into Gemini Notebook; its answers come only from your sources and show citations [S3][S41].
- **A morning digest of unread email.** Workspace Studio has a ready-made template that recaps unread emails and posts to Chat [S42].
- **File email attachments automatically.** A Workspace Studio flow can save attachments to a Drive folder [S42].
- **Check a deal while writing an email.** Gemini's HubSpot or Salesforce integration answers from the side panel (read only) [S52].
- **Create records in another app from an automation.** Workspace Studio's Beta steps can act in Asana, Mailchimp, Salesforce, HubSpot or monday [S43].
- **Mark up a contract in Docs.** Claude's Docs add-on proposes edits as cards you accept or reject [S83].
- **Build or clean up a spreadsheet by describing it.** ChatGPT for Google Sheets, or Claude in Sheets [S79][S83].
- **Find Google Drive files from Microsoft 365.** Microsoft's Google Drive connector puts them in Copilot search [S85].
- **Plan a lesson (schools).** Gemini in Classroom drafts lesson plans and quizzes for teachers [S62].

## What to watch for

**Permissions: AI sees what the person sees**
- Gemini only retrieves content the user can already access [S9].
- Claude mirrors your Google permissions [S80], and Microsoft's connectors use your own identity and permissions [S87].
- So if a folder is shared with everyone in the company, any staff member's AI tool can surface it (our inference from [S9][S80][S87]).
- Company-managed ChatGPT connections act with the connected account's permissions, which can be wider than a user's own [S77].
- Microsoft's Google Drive connector, left on its default, shows files that anyone can access in Drive to all Microsoft 365 users in your tenant [S86].

**These tools can now change things**
- Gemini in Gmail can delete, archive and label email after you confirm [S16].
- Claude can send email and move or trash Drive files; it asks first by default, but Team and Enterprise owners can let members skip the prompt [S80].
- Microsoft's federated connectors began getting write and delete actions in early October 2026 [S87].
- ChatGPT can send an email from Gmail once you choose to. Where those actions are allowed, it can also change or delete Drive files and Calendar events [S98][S94][S100].
- A Workspace Studio test run does the real thing [S42].

**Data and training**
- Google: Workspace content isn't human-reviewed or used to train models outside your domain without permission [S9].
- Thumbs-up or thumbs-down feedback to Google may be read by people, so leave out personal or confidential details [S18][S21].
- Personal accounts, and editions where the Gemini app is only an "additional service", have different terms and possible human review [S8].
- OpenAI: no training on connected data for Business, Enterprise and Edu [S76]; ChatGPT for Sheets follows each person's own training setting [S79].
- OpenAI, any plan: no training of its general models on data from connected Google apps, apart from feedback and anything that ends up in the chat itself [S93].
- Anthropic: no training on Gmail, Drive or Calendar connector data [S80]; the Docs, Sheets and Slides add-on isn't for health information [S83].

**Where data lives**
- Workspace data regions offer the United States or Europe only [S10].
- Business Starter doesn't get data regions at all [S10].
- Gemini prompts and responses are covered for storage on every data-regions version, but processing is only covered on Enterprise and Assured Controls versions [S10].
- Gemini Notebook isn't covered by data regions, and it keeps its own copy of Drive files you add [S10][S9].
- Google's Privacy Hub doesn't name a country where Gemini processing happens [S9].

**Defaults worth checking**
- Gemini in Workspace apps: on [S7].
- Meet automatic notes: on for Business Standard and Plus from 29 September 2026 [S28].
- Workspace Studio: everyone can build flows [S45].
- Gemini integrations with outside apps: on for people with Gemini [S50].
- Unknown third-party apps: by default people can connect any of them ("Allow users to access any third-party apps") [S55].
- Microsoft's own Copilot connectors, including Gmail: on in Microsoft 365 tenants unless disabled [S87].
- ChatGPT Business: apps are on, and so are Google Drive's Docs, Sheets and Slides actions [S97].

**Admin blind spots the vendors point out**
- API controls can't restrict Gemini's third-party integrations, and blocking one later doesn't stop existing use [S51].
- Allowlisting an app in the Marketplace doesn't override API controls, and the Marketplace excludelist doesn't stop apps installed from elsewhere [S56].
- Setting a service to "Restricted" in API controls stops untrusted apps that were already installed and revokes their access [S55].
- Disabling a company connection in ChatGPT doesn't revoke the authorisation on the other side; that's a separate step [S77].

**Accuracy and checking**
- Google says Gemini may suggest inaccurate information and isn't professional advice [S17][S21].
- In the Gemini app, Gemini may pick an older email over a newer one; check the sources it lists [S35].
- Meet notes can be incomplete for short meetings or with connection problems [S27].
- Charts Gemini makes in Sheets don't update with the data, and =AI() results only refresh when you ask [S20][S21].
- Gemini Notebook "can make mistakes", Google says [S41].

**Costs that catch people out**
- Business Starter doesn't include Gemini in Docs, Sheets, Slides, Drive, Meet or Chat [S1].
- AI limits are per person and don't pool [S15].
- Heavier use of advanced image and video generation needs the paid AI Expanded Access add-on [S14].
- Removing an AI Expanded Access licence mid-month can still be charged for the whole month [S12].
- Workspace Studio limits start being enforced on 1 November 2026 [S15].
- Outside apps reached through integrations may need their own paid plans [S52].
- Claude's Workspace add-on needs a paid Claude plan [S83], and Gemini Enterprise is a separate purchase [S63].

**Students and anyone under 18**
- Under-18 users get a restricted Gemini experience, and some features are 18+ only [S8][S58].
- Under-18 users can't use AI steps in Workspace Studio [S45].
- Google AI Pro for Education can't be assigned to anyone under 18 [S60].

**Hidden instructions in content (prompt injection)**
- Google warns that untrusted emails can contain hidden instructions that hijack an AI connected through its Gmail MCP server [S69].
- Google says Gemini checks for threats before acting and blocks or leaves out malicious content [S9].

**Personal and work accounts**
- Gemini with a personal account runs under consumer terms, with possible human review [S8].
- Microsoft's consumer Copilot can connect to Gmail and Google Drive with a personal Microsoft account [S90].
- Claude Pro and Max use of the Docs, Sheets and Slides add-on is under Anthropic's consumer terms [S83].

## Announced changes

| Date | Change | Source |
|---|---|---|
| 13 Oct 2026 to mid-Nov 2026 | Skills roll out in the Gemini app for everyone | [S48] |
| 13 Oct 2026 | Skills inside Workspace apps delayed "until further notice" | [S48] |
| Early Oct 2026 | Microsoft's federated Copilot connectors start getting write, update and delete actions | [S87] |
| 1 Nov 2026 | Workspace Studio usage limits start being enforced | [S15][S12] |
| 1 Nov 2026 | Promotional access to "Convert Slides to Vids with avatars" ends | [S15] |
| 17 Nov 2026 | Gems move into Settings in the Gemini app; they can still be used | [S49] |
| No sooner than 1 Mar 2027 | Business and enterprise: Gems can't be created, edited or used; remaining Gems become draft skills; Studio flows using "Ask a Gem" stop | [S49] |
| No sooner than 1 Jun 2027 | Education: the same, plus Gems removed from Classroom | [S49] |
| From Sept 2026 | Meet's "Meet Recordings" folder renamed "Legacy Meet Recordings" and moved into a new "Google Meet" folder | [S27] |
| 29 Sep 2026 | Meet automatic note-taking on by default for Business Standard and Plus | [S28] |
| 1 Sep 2026 | OpenAI's API "connector_id" deprecated for models released after this date | [S78] |
| 28 Aug 2026 | ChatGPT allows more than one Google account per person in its Gmail, Google Calendar and Google Contacts plugins | [S98] |
| 25 Aug 2026 | Microsoft's set date for retiring its PowerShell switch for federated connectors, replaced by the "Allowed agent types" setting | [S88] |
| 16 Jul 2026 | NotebookLM renamed Gemini Notebook | [S4] |
| 8 Jun 2026 | ChatGPT can draft and send email through a connected Gmail account, on the web for Plus, Pro, Business and Enterprise | [S98] |
| 20 Apr 2026 | Drive side panel can no longer move files or create folders | [S26] |
| 19 Mar 2026 | Workspace Studio reached all release tracks | [S5] |
| 1 Mar 2026 | AI Expanded Access needed for higher advanced image and video use | [S14] |

## What we couldn't establish

- **Which ChatGPT plans include the Google apps.** OpenAI's help pages say it depends on plan, location and workspace without listing plans. We couldn't confirm Free, Go or Edu, and no OpenAI page we read named a country where the apps are unavailable [S94][S98].
- **How Business plan admins switch Gemini off in one app.** Google's per-app "Feature access" page lists only Enterprise Standard and Plus and some Education editions [S7].
- **Exact usage limits per plan.** Google's limits table has four plan columns but three values in most rows, so we couldn't map every number to a plan with confidence [S15].
- **Where Gemini processes Australian customers' data.** Google names no country, and its data regions cover only the US and Europe [S9][S10].
- **Whether a paid Microsoft 365 Copilot licence is needed** for the Gmail, Google Calendar and Google Contacts connectors [S87][S88][S89].
- **How to remove Microsoft's Google Drive connector.** The deployment page doesn't cover it [S86].
- **Whether Claude's free plan includes the Google connectors.** Anthropic says "all users" but doesn't list plans [S80].
- **Default state of Gemini's third-party integrations.** Google's launch post says on; the admin page doesn't say [S50][S51].
- **Which company's terms cover data sent through Gemini integrations** to apps like HubSpot or Salesforce [S51][S52].
- **Default state of Gemini Notebook and of Workspace Studio's third-party steps.** The admin pages don't state them clearly [S40][S46][S47].
- **Gemini Enterprise prices and Australian data residency.** Google Cloud's pricing URL returned "not found", and its editions page has no prices [S65].
- **The Australian promotional pricing terms.** The pricing page's footnotes disagree about how long introductory prices last [S1].
- **Google Contacts with Gemini.** Contacts isn't in Google's list of Workspace apps the Gemini app can connect to [S36].

## Sources

All pages were read on 15 October 2026. Google's admin help on support.google.com/a now redirects (301) to knowledge.workspace.google.com, which we observed when fetching S36, S55 and S56.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Google Workspace pricing (Australia) | Google | https://workspace.google.com/intl/en_au/pricing | No date shown | 15 Oct 2026 |
| S2 | Google Workspace for business (Australia) | Google | https://workspace.google.com/intl/en_au/business/ | No date shown | 15 Oct 2026 |
| S3 | Gemini Notebook (formerly NotebookLM) for business | Google | https://workspace.google.com/intl/en_au/products/notebooklm/ | No date shown | 15 Oct 2026 |
| S4 | NotebookLM is now Gemini Notebook (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/07/notebooklm-now-gemini-notebook.html | 16 Jul 2026 | 15 Oct 2026 |
| S5 | Workspace Studio (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2025/12/workspace-studio.html | 3 Dec 2025; update 19 Mar 2026 | 15 Oct 2026 |
| S6 | Get started with Google Workspace with Gemini | Google (Docs Editors Help) | https://support.google.com/docs/answer/13952129 | No date shown | 15 Oct 2026 |
| S7 | Manage access to Gemini features in Workspace services | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/gemini/manage-access-to-gemini-features-in-workspace-services | 13 Oct 2026 | 15 Oct 2026 |
| S8 | Turn the Gemini app on or off | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/gemini/turn-the-gemini-app-on-or-off | 13 Oct 2026 | 15 Oct 2026 |
| S9 | Generative AI in Google Workspace Privacy Hub | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/gemini/generative-ai-in-google-workspace-privacy-hub | 6 Oct 2026 (footer 13 Oct 2026) | 15 Oct 2026 |
| S10 | Data covered by Data Regions | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/compliance/data-covered-by-data-regions | 13 Oct 2026 | 15 Oct 2026 |
| S11 | Google Workspace enables the future of AI-powered work for every business | Google (Workspace blog) | https://workspace.google.com/blog/product-announcements/empowering-businesses-with-AI | 16 Jan 2025; updated 28 Apr 2025 | 15 Oct 2026 |
| S12 | AI Expanded Access | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/gemini/ai-expanded-access | 13 Oct 2026 | 15 Oct 2026 |
| S13 | AI tools for business | Google | https://workspace.google.com/products/ai-ultra | No date shown | 15 Oct 2026 |
| S14 | Google Workspace AI Expanded Access (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/02/google-workspace-ai-expanded-access.html | 5 Feb 2026 | 15 Oct 2026 |
| S15 | About AI usage limits | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/workspace-with-gemini/about-ai-usage-limits | 13 Oct 2026 | 15 Oct 2026 |
| S16 | Collaborate with Gemini in Gmail | Google (Gmail Help) | https://support.google.com/mail/answer/14355636 | No date shown | 15 Oct 2026 |
| S17 | Draft emails with Gemini in Gmail | Google (Gmail Help) | https://support.google.com/mail/answer/13955415 | No date shown | 15 Oct 2026 |
| S18 | Collaborate with Gemini in Google Docs | Google (Docs Editors Help) | https://support.google.com/docs/answer/14206696 | No date shown | 15 Oct 2026 |
| S19 | Write & edit with Gemini in Docs | Google (Docs Editors Help) | https://support.google.com/docs/answer/13951448 | No date shown | 15 Oct 2026 |
| S20 | Collaborate with Gemini in Google Sheets | Google (Docs Editors Help) | https://support.google.com/docs/answer/14356410 | No date shown | 15 Oct 2026 |
| S21 | Use the AI function in Google Sheets | Google (Docs Editors Help) | https://support.google.com/docs/answer/15877199 | No date shown | 15 Oct 2026 |
| S22 | Collaborate with Gemini in Google Slides | Google (Docs Editors Help) | https://support.google.com/docs/answer/14355071 | No date shown | 15 Oct 2026 |
| S23 | Get started with Gemini in Google Drive | Google (Drive Help) | https://support.google.com/drive/answer/14217860 | No date shown | 15 Oct 2026 |
| S24 | Let Gemini organize your files | Google (Drive Help) | https://support.google.com/drive/answer/16671865 | No date shown | 15 Oct 2026 |
| S25 | Organize, save, and share your Gemini sources using projects in Drive | Google (Drive Help) | https://support.google.com/drive/answer/14356148 | No date shown | 15 Oct 2026 |
| S26 | Execute basic organizational tasks using Gemini in Drive (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2025/07/execute-basic-organizational-tasks-using-gemini-in-drive.html | 7 Jul 2025; update 20 Apr 2026 | 15 Oct 2026 |
| S27 | "Take notes for me" in Google Meet | Google (Meet Help) | https://support.google.com/meet/answer/14754931 | No date shown | 15 Oct 2026 |
| S28 | New Google Meet 'Take notes for me' settings for admins and end users take effect September 29th (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/09/new-google-meet-take-notes-for-me-settings-for-admins-and-end-users-take-effect-September-29th.html | 22 Sep 2026 | 15 Oct 2026 |
| S29 | Let Google Meet AI take notes for my users | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/meet/let-google-meet-ai-take-notes-for-my-users | 13 Oct 2026 | 15 Oct 2026 |
| S30 | Suggest times to meet with Gemini in Gmail | Google (Gmail Help) | https://support.google.com/mail/answer/16865189 | No date shown | 15 Oct 2026 |
| S31 | Summarize chats in Google Chat | Google (Chat Help) | https://support.google.com/chat/answer/12918975 | No date shown | 15 Oct 2026 |
| S32 | Help me create with Gemini in Google Forms (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2025/06/help-me-create-gemini-google-forms.html | 11 Jun 2025 | 15 Oct 2026 |
| S33 | Get started with Google Vids | Google (Docs Editors Help) | https://support.google.com/docs/answer/15081495 | No date shown | 15 Oct 2026 |
| S34 | Google Chat now available as a data source in the Gemini app (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/02/google-chat-now-available-as-data-source-in-gemini-app.html | 25 Feb 2026 | 15 Oct 2026 |
| S35 | Use apps connected to Gemini with a work or school Google Account | Google (Gemini Apps Help) | https://support.google.com/gemini/answer/14959807 | No date shown | 15 Oct 2026 |
| S36 | Control Gemini App access to Workspace services | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/gemini/turn-google-apps-in-gemini-on-or-off | 13 Oct 2026 | 15 Oct 2026 |
| S37 | Use Gemini Apps with a work or school Google Account | Google (Gemini Apps Help) | https://support.google.com/gemini/answer/14620100 | No date shown | 15 Oct 2026 |
| S38 | Check the availability & requirements of Connected Apps in Gemini Apps | Google (Gemini Apps Help) | https://support.google.com/gemini/table/17434654 | No date shown | 15 Oct 2026 |
| S39 | Where you can use the Gemini web app | Google (Gemini Apps Help) | https://support.google.com/gemini/answer/13575153 | No date shown | 15 Oct 2026 |
| S40 | Turn Gemini Notebook on or off for users | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/gemini-notebook/turn-gemini-notebook-on-or-off-for-users | 13 Oct 2026 | 15 Oct 2026 |
| S41 | Learn about Gemini Notebook | Google (Gemini Notebook Help) | https://support.google.com/gemininotebook/answer/16164461 | No date shown | 15 Oct 2026 |
| S42 | Get started with Google Workspace Studio | Google (Workspace Studio Help) | https://support.google.com/workspace-studio/answer/16444479 | No date shown | 15 Oct 2026 |
| S43 | Take actions in third-party services with flows (Beta) | Google (Workspace Studio Help) | https://support.google.com/workspace-studio/answer/16658279 | No date shown | 15 Oct 2026 |
| S44 | Learn about Google Workspace Studio limits | Google (Workspace Studio Help) | https://support.google.com/workspace-studio/answer/16765942 | No date shown | 15 Oct 2026 |
| S45 | Allow people to create and use flows | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/studio/allow-or-block-flows | 13 Oct 2026 | 15 Oct 2026 |
| S46 | Require approval for flows | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/studio/require-user-approval-for-external-studio-flows | 13 Oct 2026 | 15 Oct 2026 |
| S47 | Set up Workspace Studio | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/studio/get-started-workspace-studio-set-up-guide-for-admins | 13 Oct 2026 | 15 Oct 2026 |
| S48 | An update on the launch of skills in the Gemini app and Workspace (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/10/an-update-on-launch-of-skills-in-gemini-app-and-workspace.html | 13 Oct 2026 | 15 Oct 2026 |
| S49 | About the transition to skills | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/gemini-app/about-the-transition-to-skills | 30 Sep 2026 (footer 13 Oct 2026) | 15 Oct 2026 |
| S50 | Connect to more tools with Gemini in Google Workspace (Workspace Updates) | Google | https://workspaceupdates.googleblog.com/2026/09/connect-to-more-tools-with-gemini-in-Google-Workspace.html | 15 Sep 2026; update 30 Sep 2026 | 15 Oct 2026 |
| S51 | Support access to Workspace Integrations | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/support-access-to-workspace-integrations | 13 Oct 2026 | 15 Oct 2026 |
| S52 | Use integrations with Gemini in Workspace | Google (Gmail Help) | https://support.google.com/mail/answer/16796422 | No date shown | 15 Oct 2026 |
| S53 | Turn access to Google Workspace with Gemini Beta on or off | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/workspace-with-gemini/turn-access-to-google-workspace-with-gemini-beta-on-or-off | 13 Oct 2026 | 15 Oct 2026 |
| S54 | Learn about smart features & controls for Google Workspace & other Google products | Google (Gemini Apps Help) | https://support.google.com/gemini/answer/15604322 | No date shown | 15 Oct 2026 |
| S55 | Control which apps access Google Workspace data | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/apps/control-which-apps-access-google-workspace-data | 13 Oct 2026 | 15 Oct 2026 |
| S56 | Manage the Marketplace app allowlist for your organization | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/apps/manage-the-marketplace-app-allowlist-for-your-organization | 13 Oct 2026 | 15 Oct 2026 |
| S57 | Manage links between your Google Account & apps from other developers | Google (Google Account Help) | https://support.google.com/accounts/answer/13533235 | No date shown | 15 Oct 2026 |
| S58 | Gemini for Education (Australia) | Google for Education | https://edu.google.com/intl/ALL_au/ai/gemini-for-education/ | No date shown | 15 Oct 2026 |
| S59 | Gemini for Google Workspace FAQ (Education) | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/workspace-with-gemini/gemini-for-google-workspace-faq-education | 13 Oct 2026 | 15 Oct 2026 |
| S60 | Google AI Pro for Education | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/workspace-with-gemini/ai-pro-for-education | 13 Oct 2026 | 15 Oct 2026 |
| S61 | Control access to Google services by age | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/getting-started/editions/control-access-to-google-services-by-age | 13 Oct 2026 | 15 Oct 2026 |
| S62 | Learn about Gemini in Google Classroom | Google (Classroom Help) | https://support.google.com/edu/classroom/answer/15410566 | No date shown | 15 Oct 2026 |
| S63 | Turn Gemini Enterprise on or off for users | Google (Workspace Admin Help) | https://knowledge.workspace.google.com/admin/generative-ai/gemini-enterprise/turn-gemini-enterprise-on-or-off-for-users | 13 Oct 2026 | 15 Oct 2026 |
| S64 | What is Gemini Enterprise? | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs | 14 Oct 2026 | 15 Oct 2026 |
| S65 | Gemini Enterprise editions | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/editions | 14 Oct 2026 | 15 Oct 2026 |
| S66 | Introduction to connectors and data stores | Google Cloud | https://docs.cloud.google.com/gemini/enterprise/docs/connectors/introduction-to-connectors-and-data-stores | 14 Oct 2026 | 15 Oct 2026 |
| S67 | Google Cloud MCP servers overview | Google Cloud | https://docs.cloud.google.com/mcp/overview | 13 Oct 2026 | 15 Oct 2026 |
| S68 | Supported products (Google Cloud MCP servers) | Google Cloud | https://docs.cloud.google.com/mcp/supported-products | 13 Oct 2026 | 15 Oct 2026 |
| S69 | Configure the Gmail MCP server | Google for Developers | https://developers.google.com/workspace/gmail/api/guides/configure-mcp-server | 12 Oct 2026 | 15 Oct 2026 |
| S70 | MCP Reference: drivemcp.googleapis.com | Google for Developers | https://developers.google.com/workspace/drive/api/reference/mcp | 16 Jul 2026 | 15 Oct 2026 |
| S71 | Google Apps Script overview | Google for Developers | https://developers.google.com/apps-script/overview | 3 Sep 2026 | 15 Oct 2026 |
| S72 | Vertex AI Service (Apps Script) | Google for Developers | https://developers.google.com/apps-script/advanced/vertex-ai | 3 Sep 2026 | 15 Oct 2026 |
| S73 | Add-ons overview (Google Workspace add-ons) | Google for Developers | https://developers.google.com/workspace/add-ons/overview | 9 Oct 2026 | 15 Oct 2026 |
| S74 | Apps (OpenAI Academy) | OpenAI | https://academy.openai.com/public/clubs/work-users-ynjqu/resources/connectors | 28 Oct 2025; last updated 4 Sep 2026 | 15 Oct 2026 |
| S75 | Plugins (ChatGPT Learn) | OpenAI | https://learn.chatgpt.com/docs/plugins | No date shown | 15 Oct 2026 |
| S76 | Plugin controls (ChatGPT Learn) | OpenAI | https://learn.chatgpt.com/docs/enterprise/apps-and-connectors | No date shown | 15 Oct 2026 |
| S77 | Workspace connections (ChatGPT Learn) | OpenAI | https://learn.chatgpt.com/docs/enterprise/shared-connections | No date shown | 15 Oct 2026 |
| S78 | MCP servers (API docs, connectors) | OpenAI | https://developers.openai.com/api/docs/guides/tools-connectors-mcp | No date shown | 15 Oct 2026 |
| S79 | ChatGPT (Google Workspace Marketplace listing, by OpenAI) | Google Workspace Marketplace / OpenAI | https://workspace.google.com/marketplace/app/chatgpt/870214997678 | Listing updated 1 Jun 2026 | 15 Oct 2026 |
| S80 | Use Google Workspace connectors | Anthropic (Claude Help Center) | https://support.claude.com/en/articles/10166901-use-google-workspace-connectors | "Updated over 2 weeks ago" | 15 Oct 2026 |
| S81 | Use connectors to extend Claude's capabilities | Anthropic (Claude Help Center) | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated over 2 weeks ago" | 15 Oct 2026 |
| S82 | Claude (Google Workspace Marketplace listing, by Anthropic) | Google Workspace Marketplace / Anthropic | https://workspace.google.com/marketplace/app/claude/12459801340 | Listing updated 14 Oct 2026 | 15 Oct 2026 |
| S83 | Use Claude in Google Docs, Sheets, and Slides | Anthropic (Claude Help Center) | https://support.claude.com/en/articles/16951679-use-claude-in-google-docs-sheets-and-slides | "Updated yesterday" | 15 Oct 2026 |
| S84 | Microsoft-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft | 30 Sep 2026 | 15 Oct 2026 |
| S85 | Google Drive connector overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/google-drive-overview | 15 Dec 2025 | 15 Oct 2026 |
| S86 | Deploy the Google Drive connector | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/google-drive-deployment | 18 Nov 2025 | 15 Oct 2026 |
| S87 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | 30 Sep 2026 | 15 Oct 2026 |
| S88 | Manage federated connector availability | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-federated-connectors | 28 Apr 2026 | 15 Oct 2026 |
| S89 | Copilot connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview | 6 Oct 2026 | 15 Oct 2026 |
| S90 | Connecting Microsoft Copilot to other services (Copilot connectors) | Microsoft Support | https://support.microsoft.com/en-us/microsoft-copilot/connecting-microsoft-copilot-to-other-services | No date shown | 15 Oct 2026 |
| S91 | Search results for "claude" | Google Workspace Marketplace | https://workspace.google.com/marketplace/search/claude | No date shown | 15 Oct 2026 |
| S92 | Search results for "chatgpt" | Google Workspace Marketplace | https://workspace.google.com/marketplace/search/chatgpt | No date shown | 15 Oct 2026 |
| S93 | Google app data controls FAQ | OpenAI | https://help.openai.com/en/articles/10408842-google-app-data-controls-faq | "Updated: 20 days ago" (25 Sep 2026, UTC) | 15 Oct 2026 |
| S94 | Google Drive app and setup in ChatGPT | OpenAI | https://help.openai.com/en/articles/10929079-google-drive-app-and-setup-in-chatgpt | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
| S95 | Connected apps in ChatGPT | OpenAI | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S96 | Connecting and managing app accounts in ChatGPT | OpenAI | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S97 | Admin controls, security, and compliance for plugins and apps | OpenAI | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S98 | ChatGPT release notes | OpenAI | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
| S99 | Gmail (ChatGPT plugin listing) | OpenAI | https://chatgpt.com/plugins/plugin_connector_1p_95d39881713c8191931482a62d6edff9 | No date shown; version 0.1.10 | 15 Oct 2026 |
| S100 | Google Calendar (ChatGPT plugin listing) | OpenAI | https://chatgpt.com/plugins/plugin_connector_1p_f8509de903288191b14a160c6c5d20b0 | No date shown; version 1.2.7 | 15 Oct 2026 |
| S101 | ChatGPT for Excel and Google Sheets | OpenAI | https://help.openai.com/en/articles/20001063-chatgpt-for-excel-and-google-sheets | "Updated: 2 months ago" (16 Aug 2026, UTC) | 15 Oct 2026 |
