# Canva: the AI inside it, and the AI that connects to it
Researched 15 October 2026 from vendor documentation. Every line is tagged with its source.

Most of Canva's help pages show no "last updated" date, so the Sources table records the day we read each one. Where a Canva newsroom post shows no date on screen, we took the date from the page's own publishing data, which is in UTC.

## The short version

Canva's AI is on every plan, including Free, but the free plan gets about 20 AI uses a month. [S1][S2]
Paid plans get more, and the newest tools, like chatting with Canva AI to change a design or making video clips, use the allowance fastest. [S2]
Canva says it doesn't use content from Business, Teams, Enterprise or Education accounts to improve its AI, and Free and Pro users control this in their Privacy Settings. [S40][S42]
On team and school plans, admins choose who gets each AI feature, but Canva AI itself can't be fully switched off. [S36][S8]
Outside assistants can work inside your Canva account through Canva's "AI Connector", and Canva gives setup guides for ChatGPT, Claude, Gemini and Microsoft Copilot. [S56]
A connected assistant can read your designs, and it can also create and edit designs and export files. [S56][S57]
The connector works on every Canva plan, but some actions need a paid or Enterprise plan, and Canva's own pages disagree about which. [S56][S57][S77]
A team admin can switch the connector off for the whole team, and in Canva Education "AI connectors" are blocked by default. [S56][S38]
Canva warns that its AI can make mistakes, and that AI charts start with sample data you have to replace. [S10][S28]
Canva also says it can't give you permission to use recognisable people or brands in AI images, so getting that permission is up to you. [S15]

## The tool, and the plans that matter

Canva is an online design tool. Its AI sits on the homepage and inside the editor, including in Canva's Docs, Sheets and Code tools. [S3][S4]
If you're billed outside the US and UK, your contract is with Canva Pty Ltd, an Australian company. [S42]

**Words used in this guide**

- **Canva AI** is Canva's built-in assistant. You chat with it to create or change designs. [S3]
- **Magic Studio** was Canva's 2023 name for its set of AI tools. [S47] Many help pages still say a tool "is part of Magic Studio", but Canva's current AI page doesn't use the name. [S22][S10]
- The **AI allowance** is your monthly budget of AI use. Canva sorts its AI tools into Standard, Premium and Ultra tiers, which use the allowance at different rates. [S1][S2]
- An **API** is a doorway that other software uses to read or change things in your Canva account. Canva now calls its APIs the Canva REST APIs. They used to be the Connect APIs. [S83]
- **MCP** (Model Context Protocol) is a shared standard that lets AI assistants use other software. Canva's AI Connector is "powered by the Canva MCP Server". [S59][S81]
- Canva uses the word "connectors" for two different things. The **AI Connector** lets outside assistants like ChatGPT into your Canva account. [S56] **Connectors in Canva AI** go the other way, letting Canva's own AI read from apps like Gmail or Slack. [S65][S81]
- A **Brand Kit** stores your brand's colours and fonts, among other things. [S67] A **Brand Template** is a reusable team layout, and **Autofill** fills one with your own data. [S57][S85]

**What each plan gets** (Australian pricing page and Canva's AI usage page, read 15 October 2026)

| Plan | Who it's for | Price shown in AUD | Monthly AI allowance |
|---|---|---|---|
| Free | One person [S1] | A$0 [S1] | Up to 20 uses of Standard or Premium tools. No Ultra tools. [S1][S2] |
| Pro | One person [S1] | A$165 a year [S1] | Standard tools don't count (fair use applies). Up to 200 Premium uses, or up to 20 Ultra uses. [S2] |
| Business | Individuals and small teams [S55] | A$280 a year per person [S1] | Standard tools unlimited (fair use). Up to 400 Premium uses, or up to 40 Ultra uses. [S2] |
| Enterprise | Organisations [S1] | No price shown ("Let's talk") [S1] | Same as Business. [S2] |
| Canva Education | K–12 schools and teachers [S1][S39] | Free for eligible teachers and schools [S39] | Standard tools unlimited (fair use). Up to 200 Premium uses, or up to 20 Ultra uses. [S2] |
| Canva for Nonprofits | Eligible non-profits [S1] | Free for one team of up to 50 people. Extra seats are 50% off Enterprise pricing. [S1] | Same as Pro. [S2] |
| Canva Teams | Existing subscribers only [S54] | Closed to new sign-ups and upgrades [S54] | Same as Pro. [S2] |
| Canva Campus | Higher education [S1] | No price shown [S1] | Not stated |
| Pro Lite | Canva says it's "currently available in India and Indonesia" [S105] | Not on the Australian pricing page [S1] | Same as Free. [S105] |

- The pricing page has a monthly and yearly switch ("Save from 16%"), but we could only read the yearly figures. [S1]
- Canva's allowance figures are "up to" estimates that assume simple prompts and one type of tool. Real use with advanced tools is usually lower. [S2]
- On Teams, Business, Nonprofits, Education and Enterprise, each member has their own allowance. Allowances aren't shared or pooled across the team. [S2]
- Paid and Nonprofit allowances reset monthly on your billing date, including on yearly plans. [S2]
- Free resets at 12:00 a.m. UTC on the first of each month. [S2] That's 8 am on the 1st in Perth (our conversion).
- Pro and Business free trials get the Free allowance: up to 20 Standard or Premium uses, and no Ultra. [S2]
- To see what's left: profile icon > **Settings** > **Billing**, then look under **AI usage**. [S2]

**What the tiers cover** (Canva's AI usage page)

| Tier | Tools Canva lists | How it's counted |
|---|---|---|
| Doesn't count on paid plans | Translate, Magic Write, Canva AI text answers, Photo and Video Animations, AI Voice [S2] | No allowance used on paid plans. On Free these still draw on the allowance. [S2] |
| Standard | Image Upscaler, image generation with Canva AI, Magic Formulas [S2] | Cheapest. Doesn't count on paid plans, subject to fair use. [S2] |
| Premium | Magic Layers, generating a design or elements with Canva AI, Canva Code interactives, Music and Sound Effect Generator, Form generator, Affinity's premium AI features [S2] | Draws on the allowance. [S2] |
| Ultra | Conversational design with Canva AI 2.0, creating a video clip, creating an image with Canva AI [S2] | Uses the most. Not available on Free. [S2] |

- The usage page lists "Create an image with Canva AI" under more than one tier. [S2] Dream Lab's page says you can pick a quality tier, and higher tiers use more allowance. [S16] It appears the tier depends on the quality you choose (our inference).
- Canva AI 2.0 uses more of the allowance when a task includes larger design files or needs more steps. [S2]
- Tasks that call on several AI tools cost more, and harder tasks may use more advanced models. [S2]

**When you run out**

- On Free, Standard and Premium tools keep working with short pauses between generations. Ultra tools stop until the reset. [S2]
- On Pro and Teams you can keep using AI tools, with short pauses between tasks. [S2]
- Enterprise, Education and Nonprofits can keep using Premium features with short pauses. [S2]
- Canva notifies you as you get close to the limit. [S2]

**Buying more AI**

- **AI Pass** is a monthly add-on for Pro, Teams, Business and Nonprofits plans managed on the web. [S52]
- It isn't available on Free, Education or Enterprise, on free trials, on prepaid plans, or on plans billed through the Apple App Store or Google Play. [S52]
- Canva's AI Pass page says it gives Pro, Teams and Nonprofits 40 times more AI, and Business 20 times more. [S52] The pricing page describes AI Pass as "40x" for Pro and Business. [S1]
- AI Pass is charged per person. On Teams and Business, only owners and admins can buy it. [S52]
- To buy it: profile icon > **Settings** > **Billing** > under **AI usage**, **Get more** > **Purchase AI Pass**. [S52]
- To cancel it: **Settings** > **Billing** > next to AI Pass, **Remove** > **Remove AI Pass**. It stays until the end of the billing cycle. [S52]
- **AI top-ups** are for Business only. Each adds one month's Business allowance and lasts 30 days. Unused allowance doesn't roll over, and only one top-up can be active at a time. [S53]
- A manual top-up "can't be cancelled once purchased". [S53] Automatic top-ups need a web subscription and have a spend cap. [S53]
- The Australian pricing page shows no price for either add-on. [S1] See "What we couldn't establish".

**Where your data lives**

- Canva's Trust Center says "Canva stores your data in the United States". [S40]
- The same page says Canva group companies process data in Australia, New Zealand, the Philippines, the United Kingdom and Singapore, as well as Europe and the US. [S40]
- Canva's Privacy Policy (25 August 2026) says your information "will be stored and processed in" the United States, Australia, Singapore, the EU, the UK, the Philippines and New Zealand. [S41]
- Canva's sub-processor list (17 April 2026) names the outside companies used for "Canva AI Services": Amazon Web Services (US and EU), and Anthropic, ElevenLabs, Features & Labels, Google, Nanonoble and OpenAI (all US). [S49]
- Leonardo.AI, a Canva group company, is listed for "Canva & Affinity AI Services" in Australia and the United States. [S49]
- Canva Austria GmbH, another group company, is listed for "Canva and Affinity Photo and Video AI Services" in the EU and US. [S49]
- The list says Nanonoble doesn't process customer personal data for Canva Education, Canva Enterprise, or customers with a signed Order Form. [S49]
- We didn't find an option to keep Canva data in Australia only. See "What we couldn't establish".

## AI built in

Three things apply to most features in this section.

**Who controls it.** On Teams and Business, Magic and AI features are on for every member by default. [S36]
Admins change this at profile icon > **Settings** > under **Controls and permissions**, **Permissions** > **Magic and AI**, then choose who can use each feature. [S36]
The same controls are available to Enterprise and Education owners and admins. [S36]
The **Magic and AI** list, in Canva's words: Magic Write, Magic Design, Magic Activities, Magic Edit, Magic Media, Transform into Doc, Dream Lab, Help Assistant for AI-generated design advice, Canva AI, Magic Insights, Canva Code, AI Shapes, AI Charts, Use team content to generate AI responses, Canva AI Music and Sound Effects, and Image to Video. [S36]
Changes apply to new designs. Magic features already used in existing designs stay available. [S36]
Some people may not get a feature even when it's switched on, because availability depends on the language set in Canva. [S36]
Canva's FAQ says Canva AI "is a core feature and can't be fully turned off", though team and school admins can control access to it. [S8]

**Schools are set up differently.** "Only administrators and teachers have access by default." [S36] See "Schools and students" under What to watch for.

**The data rules are shared.** Canva says it "won't use your user content to improve AI-powered features" unless your Privacy Settings allow it. [S40]
Content from Teams, Business, Enterprise and Education accounts isn't used to improve AI features. [S40][S42][S46]
Inputs may go to Canva's outside "Technology Partners" so they can run the feature. [S43]
The feature blocks below only add what's specific to each one. "What to watch for" has the detail.

### Canva AI (the assistant)

**What it does.** A chat assistant for creating and editing designs, images, videos and code, and for brainstorming. [S3]
Canva calls the original single-prompt version "Canva AI 1.0". "Canva AI 2.0" lets you create and edit by chatting inside the editor. [S3]
In the editor it reads your design and changes it on the canvas, for example "Make all headlines blue". [S5]
It can search the web for current information and apply your Brand Kit. [S3][S4]
It can also run tasks on a daily, weekly or monthly schedule, up to 10 at a time. Each run starts a new chat and you get a notification when it's done. [S3]
Canva announced Canva AI 2.0 on 16 April 2026 as a research preview, saying general availability would roll out "over the coming weeks". [S11]
Its help pages still say 2.0 features are rolling out gradually. [S9]

**Where to find it.** From the homepage, select **Canva AI** in the side navigation. [S3]
Type or speak your prompt, then press Enter or select **Submit**. The plus icon adds context: **Upload**, **Add from Canva**, **Apply brand** or **Connect**. [S7]
In the editor, select the **Canva AI** tab in the sidebar and describe the change. The **Stop** button interrupts it. [S5]
Or select an element and choose **Ask Canva** in the editor toolbar, which opens Canva AI in the side panel. [S6]
Chat history is under the icon in the top corner. Scheduled tasks are under the panel icon > **Tasks**. [S3]

**Plans and cost.** Canva AI itself is on every plan, including Free. [S10]
Canva's help pages say the 2.0 features, including Memory Library and Connectors, come with Pro, Teams, Business and Nonprofit. [S3][S4]
Free and Education users get "Canva AI 1.0" features, plus tools like Magic Write and Background Remover with limited monthly use. [S3]
The page on editing by conversation lists Pro, Business and Enterprise instead, and says it "isn't available for everyone just yet". [S5]
The Australian pricing page marks Canva AI 2.0 as "Soon" for Enterprise. [S1]
Conversational design is an Ultra tool, the most expensive tier, and Free can't use Ultra tools. [S2]
**Ask Canva** only uses your allowance when a request uses a premium AI feature. It doesn't appear in the toolbar on Free or Education. [S6]

**On by default, and who controls it.** On by default for Teams and Business members. Admins use the **Canva AI** control under **Magic and AI**. [S36]
Education users need their school's Canva admin to turn Canva AI on. [S4]
The admin list also has **Use team content to generate AI responses**. [S36] Going by its name, it appears to control whether Canva AI can draw on your team's content. The page doesn't explain it.

**Your data.** Canva's FAQ says "Some features may use your inputs to improve performance". [S8]
It says Google Workspace data is handled under Google's API Services User Data Policy, including its Limited Use rules. [S8]
The pages we read don't say how long Canva keeps Canva AI conversations. [S8][S41]

**In Australia.** Canva doesn't name Australia as restricted, and English is supported. [S3]
Canva does say Canva AI "may not yet be available in your country or region", and isn't available in every language yet. [S4]

### Memory Library

**What it does.** Learns your style preferences, such as colours and tone, from your work in Canva and your Canva AI prompts. It keeps them in an "About Me" page, which is a Canva Doc. [S12]
It doesn't keep chat details or the context of ongoing projects. [S12]
Canva's FAQ says it is rolling out gradually. [S8]

**Where to find it.** Home > **Canva AI** > **Memory**. If there's no About Me page yet, select **Create About Me**. [S12]

**Plans and cost.** Pro, Teams, Business and Nonprofit. Education isn't listed. [S12]

**On by default, and who controls it.** The page doesn't say whether it starts on or off. [S12]
To turn it off (desktop only): account icon > **Your account** > **AI personalization**, then under **Memory**, turn off the **About Me** toggle. [S12]
The page doesn't describe an admin control for it. [S12]

**Your data.** You can edit the About Me page, or delete it with **File** > **Organize** > **Move to trash**. No retention period is stated. [S12]
Canva's Privacy Policy says you manage your Memories in your AI personalisation settings. [S41]

**In Australia.** The page says it may be unavailable in some regions, without naming them. [S12]

### Connectors in Canva AI (Canva reading your other apps)

**What it does.** Lets Canva AI use information from apps you connect as context for designs and content. [S65]
Canva's help names Slack, Gmail, Zoom, Notion, Asana, Google Drive, HubSpot and Gong. [S65]
Canva's 2.0 announcement also listed Google Calendar, Microsoft, Atlassian and Linear. [S11]
**Can it act?** No. The connections are read-only. Canva AI can't edit, delete or create anything in those apps. [S65]
Canva's developer docs add that they bring in text only, with no images or video. [S81]
You can be limited to five active apps at a time. Canva AI may miss an app unless your prompt names it or the information you need. [S65]
Canva builds all these connectors itself and isn't taking submissions from other companies. [S81]
You can also import files from Google, Dropbox and OneDrive into Canva AI. It takes CSV, DOC, DOCX, XLS, XLSX, TXT, MD, PDF, JPG and PNG files, up to 10 MB each and three at a time. [S66]

**Where to find it.** See the steps below. The editor route works on desktop and the web. It isn't available in the mobile app. [S65]

**Steps to connect** (Canva Help Centre, no date shown; read 15 October 2026):

1. On the homepage, go to **Canva AI**, select the plus icon and choose **Connect apps**. [S65]
2. Pick an app. If your account isn't linked yet, select **Connect** and follow the prompts. [S65]
3. Turn the app on with its toggle, type a prompt that names the app or the information you need, and select **Submit**. [S65]

**Plans and cost.** Part of the 2.0 features for Pro, Teams, Business and Nonprofit. [S3]
The pricing page lists "Canva AI connectors" as new for Pro and Business, and "Soon" for Enterprise. [S1] It doesn't say which kind of connector it means, though it sits next to Canva AI 2.0 (our reading).

**On by default, and who controls it.** Each person connects their own apps. Some apps may need organisation or admin approval. [S65]
In Canva Education, "AI connectors are blocked for all Education users" by default. [S38] That page doesn't say whether it means these connectors, the AI Connector for outside assistants, or both.

**Your data.** Canva AI only sees what your connected account is allowed to see in that app. [S65]
Imported files are added to your Uploads folder. [S66]
To disconnect: plus icon > **Connect apps** > **Manage apps** > the app > **Disconnect**. That disconnects it everywhere in Canva. Toggling an app off only stops Canva AI using it. [S65]

**In Australia.** No country limits stated. Some apps are still rolling out. [S65]

### Generate a design from a description (Magic Design)

**What it does.** Canva AI drafts designs from a written description. [S7]
It covers presentations, posters, cards, flyers, invitations, business cards, postcards, documents, social media graphics and short social videos. [S7]
It shows up to eight templates. **Web Research** pulls in current information, and **Brand Hub** applies your brand styles. [S7]
The admin control for it is still called **Magic Design**. Designs that follow your brand need both **Magic Design** and **Canva AI** switched on. [S36]

**Where to find it.** Homepage > **Canva AI** > describe the design (optionally pick a design type or use the microphone) > **Submit**. Then select **Edit** to open it, or **Download**. [S7]

**Plans and cost.** It counts toward your AI usage. [S7] "Generating a design or elements with Canva AI" is a Premium tool. [S2]

**On by default, and who controls it.** On by default for Teams and Business. [S36] Owners and admins decide who gets it, and students should ask their teacher. [S7]
If an admin turns off Magic Design, a connected assistant like ChatGPT can't generate designs for anyone on that team either. [S57]

**Your data.** Uploads must be a supported format within Canva's size limit. [S7] The shared data rules at the start of this section apply.

**In Australia.** No country limits stated. Some people may not have access depending on their Canva language. [S7]

### Magic Write

**What it does.** Writes copy from a prompt, or reworks text already in your design. [S13]
Options for existing text include **Rewrite**, **Shorten**, **More formal**, **Change voice** and **Generate quiz**. [S13]
It can also draft presenter notes from your slides or from a custom prompt. [S13]

**Where to find it.** In a design, select the Quick actions icon (or type **/**) > **Magic Write**. [S13]
For existing text, right-click it or select it, then choose **Magic Write** from the toolbar. [S13]
For presentations: **Notes** > **Generate notes**. From the homepage: **Canva AI** > **Draft a doc**. [S13]

**Plans and cost.** On paid plans it doesn't count toward the monthly allowance. On Free it does. [S2]

**On by default, and who controls it.** Team admins and brand designers decide who on a team can use it, and teachers decide for their class. Canva Education admins and teachers can turn it on for students. [S14]

**Your data.** Canva's "Learn about Magic Write" page says Canva built it in partnership with OpenAI. [S14]
The same page says it "only uses data and information up to mid-2021", with a 1,500-word input limit and about 2,000 words of output. [S14]
That page may not have been updated for newer models. We couldn't confirm either way (our inference).
It warns the output may be inaccurate or unoriginal, and that its filters may occasionally miss offensive or harmful content. [S14]

**In Australia.** It supports 103 languages, matching the Canva interface. No country limits stated. [S14]

### Translate and Magic Switch

**What it does.** Translates whole pages or selected text into "100+ languages". [S27]
A **Tone of voice** setting (Original, Conversational, Informative, Professional, Friendly or Inspirational) works in 19 of them. [S27]
Each run is limited to 2,000 characters and one language. [S27]
By default it duplicates the page so your original is kept, and shrinks text to fit. [S27]
Magic Switch sits under **Resize** and includes a **Translate** option. [S27]

**Where to find it.** Right-click a text box > **Translate text** > choose **Translate to** > **Translate**. [S27]
Or **Resize** > under **Magic Switch**, **Translate** > set **Translate to** and **Apply to page** > **Translate** > **Open**. [S27]
Or select the page > **Edit** > **Translate**. The settings there include **Reduce font size to fit** and **Duplicate page when translating**. [S27]

**Plans and cost.** On paid plans Translate doesn't count toward the allowance. On Free it does. [S2]

**On by default, and who controls it.** Translate isn't in the **Magic and AI** admin list. [S36] The pages we read don't describe a separate admin switch for it.

**Your data.** The page doesn't name the translation provider. [S27]
It gives no accuracy warning, but notes "Translate doesn't work with all fonts". [S27]

**In Australia.** No country limits stated. [S27]

### Images: Magic Media, Dream Lab and AI image apps

**What it does.** Magic Media makes images, graphics and 4-second videos from a text prompt. [S15]
Dream Lab makes four images per prompt. You can add a reference image to guide the style or layout, and refine results with follow-up instructions. **Boost resolution** adds detail. [S16]
Canva AI can also create images from a prompt. [S2]
Paid plans also offer DALL·E (by OpenAI) and Imagen (by Google Cloud) as AI image generation apps. [S20]

**Where to find it.** Magic Media: in the editor side panel select **Magic Media**, or search for it under **Apps**. Choose the **Images**, **Graphics** or **Videos** tab, describe what you want, then generate. [S15]
Dream Lab: homepage > **More** > **Dream Lab** > type a prompt > **Generate**. It isn't inside the editor. [S16]

**Plans and cost.** These all count toward your AI usage. [S15][S16]
Reference images and **Boost resolution** in Dream Lab also use allowance. [S16]
DALL·E and Imagen need a paid Canva plan. [S20]

**On by default, and who controls it.** Admins control **Magic Media** and **Dream Lab** separately. [S36]
Enterprise organisation admins have a setting to "Set permissions for team members to access Dream Lab". [S37]
If Dream Lab is missing, your admin or school may have turned it off. [S17]
Canva's student app rules block "generative AI" apps for students by default and allow them for teachers. [S38] It appears DALL·E and Imagen fall in that group (our inference).

**Your data.** Dream Lab's page doesn't name its model. [S16] Leonardo.AI, a Canva group company, is listed for Canva AI services in Australia and the US. [S49]
Dream Lab puts a visible label on generated images showing AI made them. [S16]
Canva's AI terms say you must not remove or change provenance tags or metadata, including C2PA data, on AI content. [S43]
Canva says you own images you make if you follow its terms, but whether AI images can be copyrighted depends on where you are. [S16][S51]

**Canva's warnings.** Canva can't give you permission to use recognisable people, characters or brands. You need permission from whoever holds the rights. [S15][S16][S20]
Prompts are checked automatically, and you can report an image with the **Report** button. [S15][S16]
Canva's own advice: "Always use your best judgement and be a good human when sharing AI-generated content." [S15]

**In Australia.** No country limits stated. Dream Lab isn't available on canva.cn, and Magic Media may not appear for some language settings. [S16][S15]

### Video: Create a video clip and Image to Video

**What it does.** "Create a video clip" makes 8-second clips with sound, or 6-second clips without, from a text prompt. [S18]
When it launched in June 2025, Canva said it was built with Google's Veo 3 model. [S107] The current help page doesn't name a model. [S18]
Image to Video adds movement to a still image, making a silent 5-second clip. Some come out at 3 seconds. [S19]
Magic Media's **Videos** tab makes 4-second clips. [S15]

**Where to find it.** Video clip: homepage > **Canva AI** > **Video clip** > describe it > optionally **Attach a reference image**. Then download it or select **Use Canva Editor**. [S18]
Image to Video: select an image > **Edit** > under **Tools**, **Image to Video** > **Smart** or **Custom** > **Generate 5 second video**. [S19]

**Plans and cost.** Creating a video clip is an Ultra tool, so Free can't use it. [S2] At launch it was for paid plans and Nonprofits, with 5 a month to start. [S107]
Image to Video is a premium feature that counts toward your allowance. Free users can use it until their allowance runs out. [S19]

**On by default, and who controls it.** Image to Video is off by default for Education students, and school admins can turn it on. [S19] Admins have an **Image to Video** control. [S36]

**Your data.** Video clip prompts must be in English, and you can't change the audio in clips with sound. [S18]
Image to Video doesn't fully support animating faces. It won't take premium stock media or images with transparent backgrounds. [S19]
Neither page mentions labels or watermarks. [S18][S19]

**In Australia.** No Australian restriction stated. Image to Video isn't available in China. [S19]

### Photo editing: Magic Edit, Magic Grab, Magic Eraser, Magic Expand

**What it does.**
- **Magic Edit** adds, replaces or changes objects in a photo. You brush or click an area and describe the change. [S21] On our reading, the result contains content the camera didn't capture.
- **Magic Grab** lifts an object out of a photo so you can move or resize it, keeping the background. [S22]
- **Magic Eraser** removes unwanted objects. [S23]
- **Magic Expand** extends a photo past its edges. [S24]

**Where to find it.** Select the photo > **Edit** in the editor toolbar, then under **Tools**:
- **Magic Edit**: choose **All**, **Brush** or **Click**, describe the change, then **Generate**. [S21]
- **Magic Grab**: **See all** > **Magic Grab** > **Click** or **Brush** > **Grab**. [S22]
- **Magic Eraser**: **Brush**, **Click**, **Foreground** or **Text** > **Erase**. [S23]
- **Magic Expand**: **See All** > **Magic Expand** > pick a size or drag a crop handle > **Expand**. [S24]

**Plans and cost.** None of these four pages says which plans include the tool. Each points to Canva's AI usage page. [S21][S22][S23][S24] The usage page doesn't list them by name. [S2]

**On by default, and who controls it.** Admins control **Magic Edit** under **Magic and AI**, and Education admins and owners can turn it on for students. [S21][S36]
The admin list doesn't name Magic Grab, Magic Eraser or Magic Expand. [S36]

**Your data.** The shared data rules apply.

**Canva's warnings.** Magic Edit: avoid prompts for flags, text, faces or hands, which may not look right. Celebrities and popular brands may be blocked. Results may not match the lighting, or may look pixelated. [S21]
Magic Expand may not work well on faces or hands, or on images with transparent backgrounds. [S24]
Magic Grab doesn't work on images in frames or grids. [S22]

**In Australia.** No country limits stated. [S21][S22][S23][S24]

### Magic Layers

**What it does.** Splits a flat image into separate layers you can edit. Text becomes editable text and objects become separate elements, with the background kept behind them. [S25][S26]
It works best on graphics and illustrations. Photo-realistic images may separate poorly. [S25]
It takes single-page PNG or JPG files up to 5000 pixels on the longest edge. It won't process vector graphics or PDFs, or images of licensed characters or brands. [S25]

**Where to find it.** Home > **Magic Layers** > **Select Media**. Or in the editor, select an image > **Edit** > **Magic Layers**. [S25]

**Plans and cost.** A Premium tool that uses your monthly allowance. [S2][S25] The pricing page lists it on Free and Pro. [S1]

**On by default, and who controls it.** The admin list has no separate Magic Layers control. [S36]

**Your data.** The shared data rules apply.

**In Australia.** Canva launched it in public beta in the US, the UK, Canada and Australia on 11 March 2026. [S26]
Since 8 June 2026 it also works inside ChatGPT and Gemini, turning images made there into editable Canva designs. [S69]

### AI charts

**What it does.** Makes an editable chart from a description, from sample data, from your own CSV file, or from a connected source such as HubSpot, Google Analytics, World Bank, Statista or Canva Sheets. [S28]
Charts made from a description are filled with sample data that matches the description. [S28]
Data doesn't update by itself. You have to refresh or re-upload it, and uploads are CSV only. [S28]

**Where to find it.** In a design, go to **Elements**, type a chart description, open the dropdown next to **Generate images** and select **Generate a chart**. [S28]
For your own data: **Elements** > plus icon > **Upload** a CSV, or **Import** from a source and select **Add to Canva AI**. [S28]

**Plans and cost.** The page doesn't say. [S28] Canva's 2 September 2026 update said Sheets data can become a chart "with a prompt". [S74]

**On by default, and who controls it.** Admins have an **AI Charts** control. [S36]

**Your data.** Canva's warning: "Always verify and update the data with your own information before sharing." [S28]
The page says the feature may still be rolling out. [S28]

**In Australia.** Not available in China. No other country limits stated. [S28]

### Canva Code

**What it does.** Builds interactive designs and websites from a description. [S29]
You can make whole pages, such as landing pages or dashboards, or small elements like quizzes and calculators to put in other designs. [S29]
Canva Code 2.0 added templates, HTML import, visual editing and buying a custom domain. [S31]
**Show code** then **Copy code** lets you reuse the code outside Canva. [S29]

**Where to find it.** Homepage > **Code** opens the editor. Describe your design on the **Canva AI** tab. [S29]
For an element: **Canva AI** > describe it > **</> Code** > **Use in a design**, then choose a design type under **Add as an element to**. [S29]
Select **Preview** to test it, then publish it as a website. [S29]

**Plans and cost.** Since 14 July 2026, Canva says Canva Code 2.0 "is now available to free, pro, business, enterprise, and education users." [S31]
It counts toward your AI usage. [S29] Canva Code interactives are a Premium tool. [S2]

**On by default, and who controls it.** Admins and brand designers decide who on a team can use it, and teachers decide for their class. [S29]
It may be switched off in your team's or class's settings. [S30] The admin control is **Canva Code**. [S36]

**Your data.** "Only you can see your Canva Code conversations." [S29]
Who can see a published site depends on the settings you choose when you publish. [S29]
Canva says you own your inputs and outputs under its AI Product Terms. [S29]
The help page doesn't say how to check what it builds for security or accessibility. It also doesn't cover how forms collect data. [S29]

**In Australia.** Available in every language Canva supports, except for users on canva.cn. [S29]

### AI in Canva Sheets

**What it does.**
- **Canva AI for Sheets** edits a sheet from plain-language prompts. It can add and format data, sort, chart, summarise, translate and write formulas. [S32]
- **Magic Formulas** writes a formula for one cell from a description. [S33]
- **Magic Insights** turns selected data into charts and a written summary. It can also suggest formulas. [S34]

**Where to find it.** Canva AI for Sheets: open a sheet, select **Canva AI** in the editor and type a prompt. [S32]
Magic Formulas: select a cell, type **=**, choose **Magic Formulas**, describe the calculation, then **Insert**. [S33]
Magic Insights: select the cells > **Actions** > **Magic Insights** > type a question or leave it blank > **Generate insights**. [S34]

**Plans and cost.** The Canva AI for Sheets page contradicts itself. One section calls it premium and another calls it standard. [S32]
The Magic Formulas page calls it "a premium AI tool", but the usage page lists it as Standard. [S33][S2]
Magic Insights counts toward your AI usage. [S34]

**On by default, and who controls it.** Admins have a **Magic Insights** control. [S36] Canva lists Magic Insights among "the only features enabled for students" in Education. [S36]

**Your data.** Canva's warnings:
- Magic Formulas: "AI can make mistakes, so double-check results for accuracy." [S33]
- Canva AI for Sheets supports only some formulas, and complex ones "may not behave as expected". Number formats such as currency and dates vary by region, so check them. [S32]
- Magic Insights charts use a copy of your data, which may be regrouped or filtered. They don't update when the sheet changes. [S34]

**In Australia.** Canva AI for Sheets works in English locales only. [S32]

### Help Assistant

**What it does.** A chat tool that answers questions about using Canva, including billing, and points you to support. [S35]
Canva says "It's always best to double-check the responses for accuracy." [S35]

**Where to find it.** Select **Help Assistant** on the homepage or in the editor. It's also in Settings. [S35]

**Plans and cost.** The page doesn't mention the allowance. [S35]

**On by default, and who controls it.** Admins can limit it to Canva help, or allow design advice too. Students get Canva-related help by default. [S35][S36]

**Your data.** The page has no notes on data. [S35]

**In Australia.** No country limits stated. [S35]

### Audio and other built-in tools

Canva's usage page lists more AI tools than we could research one by one. [S2]
- AI Voice and Photo and Video Animations don't count toward the allowance on paid plans. [S2]
- The Music and Sound Effect Generator and the Form generator are Premium tools. Image Upscaler is a Standard tool. [S2]
- Admins have separate controls for **Canva AI Music and Sound Effects**, **AI Shapes**, **Transform into Doc** and **Magic Activities**. [S36]
- Canva's AI page also lists a Shape Generator, Magic Background, Style Match and a 3D Content Generator. [S10]
- Canva's 2 September 2026 update added AI-generated presenter notes for presentations. [S74]
We haven't checked these tools' own help pages.

### Canva AI inside Affinity

Canva says the core Affinity and Cavalry apps "remain free to use". [S72]
Its ProSuite announcement (16 September 2026) says the Canva AI Studio in Affinity "unlocks with a Canva premium plan". [S72]
About those features it says: "Your work isn't used to train these features." [S72]
Affinity's premium AI features count toward your Canva allowance and aren't available on Free. [S2]
In Education, only admins and teachers can use Canva AI tools inside Affinity for now. [S36]
Teachers get Affinity with Canva Education, and schools can opt out. [S39]

### Canva Shield (Canva's name for its AI safety and privacy layer)

**What it is.** Canva calls it a "collection of robust trust, safety and privacy tools". [S45]
It covers privacy controls, automatic review of prompts and outputs, reporting, and indemnity for some Enterprise customers. [S45]

**Indemnity.** Canva says "Eligible enterprise customers are indemnified for AI output, at no extra cost" when they use its Magic Studio products. [S45]
Its AI page says this is for "enterprise customers with over 100 seats". [S10]
The pricing page shows AI output indemnity isn't included on Free or Pro. [S1]
We couldn't find indemnity wording specific to AI output in Canva's Master Services Agreement. [S48]

**Moderation.** Canva automatically checks certain prompts and reviews outputs. [S44]
It aims to block medical advice, self-harm topics, sexually explicit content, and political topics "including content about politicians and elections". [S44]

## Outside AI that connects

Every official connection below uses Canva's **AI Connector**, which Canva says is "powered by the Canva MCP Server". [S59]
Each person signs in with their own Canva account, and the assistant can only do what that person could do in Canva. [S78]
Canva gives setup guides for ChatGPT, Claude, Gemini and Microsoft Copilot. [S56] Its list of assistants and tools that can connect is longer (see "Other assistants Canva lists"). [S58]

### Canva's AI Connector (what every connection shares)

**Official?** Yes, built by Canva. [S59]

**What it can see and do.** Canva says a connected assistant "can read design details and folders, and create and edit designs". [S56]
It can reach projects you have permission to view, including folders shared with you. [S59]
Canva's list of actions includes generating a design, creating a blank design, searching designs, and reading a design's details, pages, text and presenter notes. [S57]
It also includes resizing, importing PDF, PowerPoint, Word and Google Slides files from a link, exporting, merging and copying designs, making folders and moving items, viewing comments, and searching and autofilling Brand Templates. [S57]
Exports can be PDF, PNG, MP4, PowerPoint, JPG and other formats. [S57]
Canva's developer list adds uploading assets, adding comments and replies, generating images, removing backgrounds, and step-by-step design editing. [S77]
**Can it delete?** Neither list includes a tool for deleting designs. [S57][S77]
Which actions you actually get depends on the assistant. [S57]

**What you need.**
- Any Canva plan can connect, including Free and Education. [S56][S59]
- Your assistant may need its own paid plan. [S59]
- On Teams, Business, Nonprofit, Education or Enterprise, your admin decides whether people can connect. [S56]
- Some actions need more than a free plan, and Canva's pages disagree about which:

| Action | Canva Help Centre | Canva's AI Connector page | Canva developer docs | Google's Gemini help |
|---|---|---|---|---|
| Search Brand Templates | Paid plans, including Education [S56][S57] | Enterprise only [S59] | Pro and above [S77] | Enterprise only [S96] |
| Autofill a Brand Template | Enterprise [S57][S60], but another page says "all Canva plans except Pro Lite and Canva Free" [S56] | Enterprise only [S59] | Pro and above [S77] | Enterprise only [S96] |
| Resize a design | Not stated | Paid plans [S59] | Pro and above. Free gets a limited trial. [S77] | Enterprise only [S96] |

- Exports from Free accounts are standard quality. Pro and above get higher quality, lossless PNG and transparent backgrounds. [S77]

**Before anyone connects: the admin switch** (Canva Help Centre, no date shown; read 15 October 2026):

1. Go to **Admin Dashboard**. [S56]
2. Select **Controls and Permissions**, then **Third-party integrations**. [S56]
3. Turn Canva's **AI Connector** on or off. [S56]

"When it's off, nobody on the team can connect an assistant." Existing connections stop working. [S56]
The connector "counts as a third-party integration" and "uses the same permissions as the Canva Connect API". [S56]
Team admins can currently only switch it on or off for the whole team. [S58]
Canva's advice: "If your organisation isn't comfortable granting these permissions, leave it off." [S56]

**To disconnect from Canva's side.** In your Canva settings, go to **Your profile** > **Integrations connected to Canva** and select **Disconnect** next to **Canva AI Connector**. [S59]
"The AI assistant loses access immediately, but your designs stay in Canva." [S59]
You can also remove it in the assistant's own settings, as each block below shows. [S59]

**Limits.**
- AI actions like generating designs "may use your monthly Canva AI credits". [S56] Canva's usage page confirms your allowance can be spent generating designs inside connected assistants. [S2]
- Canva says "We'll introduce usage limits in the future." [S56]
- Each person can make up to 300 requests a minute across all their AI tools. Some actions have lower caps, such as 10 image generations a minute. [S77]
- Your assistant may have its own message or token limits. [S56]
- You only see Brand Templates that have been shared with you. [S56]
- In Education, Canva says only "teachers and students in higher education levels" can use what the connector unlocks. [S59] It doesn't make clear whether school (K–12) teachers are included.

### ChatGPT and Canva

**Official?** Yes. Canva calls it the "Canva plugin" in ChatGPT, running on its AI Connector. [S60]
On 8 June 2026 Canva said the Canva app in ChatGPT was "available to all users globally". [S69]
OpenAI's plugin directory lists it as Canva, made by Canva Pty Ltd., version 17.0.1. [S109]

**What it can see and do.** It creates designs from your description and shows options in the chat. You pick one to keep editing in Canva. [S60]
You can also ask it to find your existing designs, resize or copy a design, import a design from a link, or turn an image into an editable design. [S60]
Magic Layers works inside ChatGPT for images made there. [S69]
Only designs you select are saved to your Canva account. To keep one, choose **Save** or **Open in Canva**. [S60]
Searching Brand Templates needs a paid Canva plan, and autofill needs Enterprise. [S60]
OpenAI's listing also mentions removing backgrounds and checking designs against your Brand Kit. Bulk Create needs a Canva Enterprise plan, and making designs or images uses Canva AI credits. [S109]

**What you need.** A ChatGPT account and any Canva account, including Free and Education. [S60]
Canva says a ChatGPT Business or Enterprise admin must turn on **Apps & Connectors** first. [S60] OpenAI's own pages say apps start switched on in Business. In Enterprise and Edu, new plugins and apps generally stay off until an admin reviews them under **Admin console** > **Plugins**. [S112]
On a Canva team, your admin may need to allow the AI Connector. [S60]
OpenAI says its plugin directory is open on every ChatGPT plan, while using a particular plugin depends on your plan, workspace, role and region. [S110] Its Canva page doesn't list plans or countries. [S108]

**Steps to connect** (Canva Help Centre, no date shown; read 15 October 2026):

1. Open ChatGPT and select **Settings**. [S60]
2. Select **@ Plugins**. [S60]
3. Select Canva and follow the prompts to connect your Canva account. Sign in to the right Canva account and authorise Canva if asked. [S60]
4. Check it worked: in **@ Plugins**, Canva should show as connected. [S60]
5. To use it, turn Canva on in a chat. Describe what you want, including the type of design and any text, and say you want it in Canva. [S60]
6. Select an option to open it in Canva and keep editing. [S60]

OpenAI's help centre labels the same route **Settings** > **Plugins**, then **Install plugin** if it's shown and **Connect**. [S111]

**To disconnect** (Canva Help Centre):
- For now: **@ Plugins** > find **Canva** > more icon > **Manage** > more icon > **Disconnect**. [S60]
- For good: **@ Plugins** > find **Canva** > more icon > **Uninstall**. [S60]
- OpenAI's help centre gives **Settings** > **Plugins** > Canva > the account's **•••** menu (or **Connection**) > **Disconnect**. It warns that uninstalling a plugin can disconnect every account connected through it. [S111]
- Or from Canva's side, as above. [S59]

**Limits.**
- Canva warns that ChatGPT sometimes makes links that "look like Canva links but don't point to a real design". Open the design from ChatGPT's preview, or find it in your Canva projects. [S60]
- If you see "Access Restricted by Team Admin", your Canva admin needs to allow the AI Connector. [S60]
- Canva's terms say third-party services run under their own terms. [S42] OpenAI's listing says ChatGPT may share relevant chats and memories with Canva, under Canva's terms and privacy policy. It also says ChatGPT follows your training settings for data from connected apps. [S109]
- On Free, Go, Plus and Pro, OpenAI may use information from apps to train its models if **Improve the model for everyone** is on. Business, Enterprise and Edu aren't used for training by default. [S104]

### Claude and Canva

**Official?** Yes. Canva is in Claude's connector directory, "Made by Canva" and marked "Anthropic verified". The listing says it was added in November 2025. [S91]
The connector's address is https://mcp.canva.com/mcp. [S91]
Claude's help lists Canva as an interactive connector that can "Create and edit designs" inside the chat. [S93]
Since 25 January 2026 you can apply your Brand Kit when making designs with Claude, and Canva said Claude was "the first AI assistant" to support this. [S67]

**What it can see and do.** Claude's listing sums it up as "Search, create, autofill, and export Canva designs". [S91]
The listing shows 17 tools, including search-designs, get-design-content, generate-design, export-design, create-folder, move-item-to-folder and add-comment-thread-to-design. [S91]
Canva says that in Claude its design tools are grouped into two, read_design and edit_design, and some tools only appear in "Agent mode". [S57]

**What you need.** Claude's directory connectors work for all users on Claude, Cowork, Claude Desktop and the Claude mobile apps. Installing them on mobile is in beta. [S92]
Any Canva plan, including Free. [S56]
On Claude Team or Enterprise, an Owner or Primary Owner has to add the connector for the organisation first. Each person then signs in to Canva themselves. [S92]
Claude is offered in Australia. [S95]

**Steps to connect** (Claude Help Center, "Updated over 2 weeks ago" when read on 15 October 2026):

1. In Claude, go to **Customize** > **Connectors** and click **+** next to **Connectors**. [S92]
2. Find Canva in the directory and click it. [S92]
3. Click **Connect**, then sign in to Canva and approve access. [S92]
4. In a chat, click **+** (or type **/**), hover over **Connectors** and turn **Canva** on. [S92]

Canva's own help page describes this as **Settings** > **Connectors** > **Canva**, then turning **Canva** on under **Connectors** in a new chat. [S61]

**For Team and Enterprise owners** (Claude Help Center):

1. Go to **Organization settings** > **Connectors**. [S92]
2. Click **Browse connectors**, find Canva and click **Add to your team**. [S92]
3. If you want, set each tool to **Always allow**, **Needs approval** or **Blocked**. Members can't override these. [S92]

Owners can also turn off just the interactive parts of a connector under **Organization settings** > **Connectors**. Its text-based functions keep working. [S93]

**For Canva Enterprise: Cross app access (beta).** Canva Enterprise organisations that use Okta for single sign-on can give everyone the connector in Claude Team or Enterprise through their existing sign-on. [S64]
Steps (Canva Help Centre, no date shown; read 15 October 2026):

1. In Canva, open **Settings** > **Security** > **Cross app access** and turn on **Enable Cross app access**. [S64]
2. Only if your ID-JAG issuer URL differs from your SAML **Identity Provider Issuer**: select **Add ID-JAG Issuer**, enter the **ID-JAG Issuer URL** and select **Add Issuer**. [S64]
3. Set up Okta with Okta's guide, and in Claude follow Anthropic's "Authorize MCP connectors for your entire organization". [S64]
4. Check the toggle is on, your issuer is listed, and the Canva connector shows as active in Claude. [S64]

Members then don't need to set up the connector themselves. [S64]

**To disconnect.**
- In Claude: **Customize** > **Connectors** > select Canva and disconnect it. [S92]
- Canva's page: **Settings** > **Connectors** > more icon next to Canva > **Disconnect**, then confirm. To pause it for one chat, turn **Canva** off under **Connectors** in that chat. [S61]
- Cross app access: at **Settings** > **Security** > **Cross app access**, delete the issuer or turn off **Enable Cross app access**. [S64]
- Or from Canva's side, as above. [S59]

**Limits.**
- Anthropic says raw content from connectors, including remote MCP servers, isn't used to train its models on Free, Pro and Max plans, even with Model Improvement turned on (16 March 2026). [S94]
- That page covers consumer plans only. It doesn't cover Team or Enterprise. [S94]
- Claude's directory carries the warning "Only use connectors from developers you trust". [S91]

**Claude Design.** On 17 April 2026 Canva announced that drafts made in Claude Design, from Anthropic Labs, can be turned into editable Canva designs. [S71] Canva gave no plans or setup steps. [S71]

**For developers.** Canva publishes "skills" for Claude Code, Cursor and Codex that use the same connector. They cover jobs like resizing for social media and checking a design against a brand kit. [S90]

### Gemini and Canva

**Official?** Yes. Canva gives setup steps, and Google documents Canva as a Gemini connected app. [S62][S96]

**What it can see and do.** Google's help lists three areas. [S96]
- Create designs from a prompt or a Gemini image, then edit things like text and background colours. [S96]
- Search and manage assets: find designs, list folders and pages, create folders and move things between them. [S96]
- Comments: list comments and replies, add comments and reply to them. [S96]
Canva adds that Gemini can use your Brand Kit and summarise existing designs. [S68] It can also turn Gemini images into editable layouts with Magic Layers. [S69]
**What it can't do.** Manage Brand Kit assets, export designs to other formats, see reviews, or see your billing. [S96]
These need a Canva Enterprise team: resizing, searching Brand Templates, autofilling them, and reading their data fields. [S96]

**What you need.** A personal Google Account. Google says it "isn't available if you sign in to a work or school Google Account". [S96]
**Keep Activity** must be on. [S96]
The Gemini web or mobile app, in English. It doesn't work in Gems or Live chats. [S96]
A Canva account linked to your Google Account. [S96]

**Steps to connect** (Gemini Apps Help, no date shown; read 15 October 2026):

1. Go to gemini.google.com or open the Gemini mobile app. [S96]
2. Ask Gemini to do something in Canva, and mention "Canva" or add **@Canva** to your prompt. [S96]
3. If Canva isn't connected, you'll get the option to connect it. Link your Canva account to your Google Account if asked. [S96]
4. Follow the on-screen instructions. [S96]

Or from Gemini's settings on a computer (Gemini Apps Help, no date shown):

1. On gemini.google.com, click **Customize** in the sidebar. If you can't see it, click **More** first. [S97]
2. At the top, click **Connectors**. [S97]
3. Find Canva and click **Add**, then follow the on-screen instructions. [S97]

Canva's own page gives a different path: **Settings** > **Personal Intelligence** > **Connected Apps** > **Other** > **Canva**, then turn on the toggle. [S62] Menus may differ between accounts (our inference).

**To disconnect.** In Gemini: **Customize** > **Connectors** > Canva > **More options** > **Disconnect**. [S97]
Canva's page: under **Connected Apps** > **Other**, turn Canva off, or select **Learn more** > **Unlink** to disconnect fully. [S62]
Disconnecting doesn't delete anything already in your Gemini Apps Activity. [S98]

**Limits and data.**
- Google says Gemini "saves and uses info from Connected Apps", including to provide and improve Gemini (Gemini Apps Privacy Hub, 13 October 2026). [S98]
- Chats seen by Google's human reviewers are kept for up to 3 years. Gemini Apps Activity auto-deletes after 18 months by default. [S98]
- Canva said on 8 June 2026 that its Gemini connected app was "available to all users globally". [S69] Google's page lists English only and names no countries. [S96]
- **Gemini Spark** is a Gemini feature that runs scheduled tasks and skills. Google began rolling out Canva support for it on 1 July 2026. [S99]
- Google's 17 June 2026 rollout of Spark excluded Australia. Its 14 July rollout to Google AI Ultra subscribers didn't list Australia as excluded. [S99]
- **AI Mode in Google Search** can suggest Canva templates and send generated visuals to Canva (Canva, 16 July 2026). [S68] We couldn't confirm it's offered in Australia.

### Microsoft Copilot and Canva

**Official?** Yes. It's the **Canva agent**, installed from Copilot's **Agent store**. [S63]
Microsoft lists Canva as a ready-to-deploy partner agent in Agent 365, which IT can deploy from the Microsoft 365 admin center (Microsoft Learn, 1 October 2026). [S100]

**What it can see and do.** Canva's page only says to use the agent's suggested prompts or type your own. In Cowork you use **/** commands. [S63]
Microsoft says the Agent 365 version lets people create and share Canva designs from Teams and Outlook. [S100]
It adds design collaboration requests and feedback notifications in Teams, and lets admins track all Canva agent activity in the admin center. [S100]

**What you need.**
- A Microsoft 365 work or school account. Microsoft says Copilot Chat users can use no-cost agents from the Agent Store once an admin enables them. [S102] Microsoft's page doesn't say whether the Canva agent is one of those.
- The Cowork route needs a Microsoft 365 Copilot licence. Cowork and usage-based billing must also be switched on. [S103]
- Some agents need IT approval first. You'll see **Request approval** instead of **Add**. [S101]
- On a Canva team, your admin may need to allow third-party integrations and the AI Connector. [S63]

**Steps to connect: Copilot Chat** (Canva Help Centre, no date shown; read 15 October 2026):

1. Open Microsoft Copilot and select **Agent store**. [S63]
2. Search for **Canva agent**, select it and install it. [S63]
3. Select **New chat**, select the plus icon, then **Chat with an agent**. [S63]
4. Type **Canva** and select the agent. [S63]
5. Use the suggested prompts or type your own request. You may be asked to sign in to Canva and authorise it. [S63][S56]

**Steps to connect: Cowork** (Canva Help Centre, no date shown; read 15 October 2026):

1. On a task thread, select the plus icon and open **manage plugins**. [S63]
2. Search for **Canva agent** and install it. [S63]
3. Select **Canva agent** and turn it on with the toggle. [S63]
4. Type **/** to use the Canva agent's skills. [S63]

**To disconnect.** Chat: **Agent store** > **Canva agent** > **Uninstall** or **Remove**, then confirm. [S63]
Cowork: **manage plugins** > **Canva agent** > turn it off, or select **Remove**. [S63]
If your admin installed the agent for everyone, you may not be able to remove it yourself. [S63]

**Limits.** Your organisation may restrict the Agent store. [S63]
The pages we read don't cover how Microsoft handles Canva content, or whether the agent is offered in Australia. See "What we couldn't establish".

### Other assistants Canva lists

- Canva's list of assistants and tools that can connect: AWS, Atlassian Rovo, ChatGPT, Claude, Codex, Copilot, Cursor, Dust, Fireflies AI, Gemini, Glean, Kimi, Langdock, Lovable, Make, Manus, Perplexity Computer, Poke, Snowflake Intelligence, Superhuman Go and xAI (Grok). [S58]
- Canva's AI Connector page also names Amazon Quick Suite. [S59]
- **Meta's Muse**: Canva announced a connector on 29 September 2026, and says "Canva is available in Muse to users in the US and Canada." [S70] Going by that, it isn't offered in Australia yet.
- We haven't researched these other connections.

### AI apps inside Canva's Apps Marketplace

- Canva offers DALL·E (OpenAI) and Imagen (Google Cloud) as image generation apps on paid plans. Canva's text-to-image terms and Acceptable Use Policy apply. [S20]
- Canva's usage page says "Generations made through third-party AI apps in the Marketplace aren't included" in your Canva allowance, and outside subscriptions or limits may apply. [S2]
- The DALL·E and Imagen page instead calls them a premium AI tool with limited use on paid plans. [S20]
- Leonardo.Ai is a paid add-on for Business and Enterprise. Canva says Leonardo.Ai Essential is no longer a built-in benefit of either plan. [S73]
- Admins on Enterprise and Teams can set who uses any app: **Settings** > **Apps** > **Manage** tab > search for the app > more menu > **Override access**. [S106]
- The choices are **Everyone**, **Team admins and Team brand designers**, **Team admins only** or **No one**. [S106]
- In Education, students under 18 need administrator approval to use third-party apps. [S38]

### Building your own: Canva's developer routes

These are for developers. Canva now groups them as one "Canva Developers SDK", and its developer site presents them as routes for AI agents. [S83][S89]
- **Canva REST APIs** (formerly the Connect APIs) let your own software create and sync designs and other content, and export finished designs. [S84]
- They sign people in with OAuth 2.0 and PKCE. [S88]
- The autofill API needs a Canva Pro (including Education and Nonprofits), Teams or Enterprise account with multi-factor authentication turned on. [S85]
- **Apps inside Canva** (formerly the Apps SDK) run inside the Canva editor. Public apps must pass Canva's review before they appear in the Apps Marketplace. [S87]
- Private apps for your own team are only available on Enterprise. Your own admins approve them, without Canva's review. [S86]
- **Canva MCP for developers** lets your own AI app use the same server as the AI Connector, with OAuth sign-in. [S78]
- Apps that identify themselves with a Client ID Metadata Document join a waitlist. Apps made in Canva's Developer Portal don't need to. [S78]
- Canva's usage policy says Canva data, prompts and outputs "must not be used to train, fine-tune, evaluate, or improve external AI models". [S79]
- The same policy requires each user to sign in with their own Canva account, and says background or bulk access must be opt-in and off by default. [S79]
- Canva bans bulk extraction of designs, reverse engineering, building a competing product, and AI training through its MCP. [S80]
- The **Canva Dev MCP server** is a separate local tool that helps coding assistants build Canva apps. It runs on your computer and doesn't send your code or prompts anywhere except your AI tool. [S82]
- In Claude Code it's added with `claude mcp add canva-dev -- npx -y @canva/cli@latest mcp`. [S82]

## Jobs it's good for

Each job below uses only what Canva's documentation says the tools can do. Check the output every time.

**Small workplaces**

- Draft a flyer or social post from a description, then edit it by hand. [S7] Canva AI can apply your Brand Kit if your admin allows it. [S3][S36]
- Rewrite copy you've already written, or change its tone. [S13]
- Draft presenter notes from your slides. [S13]
- Translate a notice into another language while keeping the original page. [S27] Canva gives no accuracy warning, so have a fluent speaker check it (our advice). [S27]
- Remove a distracting object from a product photo, or move the product within the frame. [S23][S22]
- Turn your own CSV of figures into a chart, replacing any sample data first. [S28]
- Write a spreadsheet formula from a plain description, then test it on numbers you already know (our advice). [S33]
- Build a simple quiz or landing page and publish it as a website. [S29][S31]
- Ask ChatGPT, Claude or Gemini to find designs, using a prompt like Canva's own example, "Find all presentations that mention Q2 marketing strategy". [S57][S60][S96]
- Bring meeting notes or email threads into Canva AI as background for a design brief. The connection only reads. [S65]
- Turn one design into versions for different platforms through a connected assistant (paid plans). [S59][S77]
- Fill a Brand Template from a spreadsheet to make many designs at once. Most of Canva's pages say this needs Enterprise. [S57][S90]

**Schools**

- Teachers draft handouts and quizzes with Magic Write's **Generate quiz**. [S13]
- Teachers build interactive study tools with Canva Code. Students can build their own only if an admin turns Canva Code on. [S29][S30][S36]
- Translate letters home into community languages, then have them checked (our advice). [S27]
- Summarise class data in Canva Sheets with Magic Insights. [S34]
- Students can ask Help Assistant how to do things in Canva. Design advice for students stays off unless an admin allows it. [S35]

## What to watch for

### Your allowance and costs

- The free plan's 20 uses go quickly, and Ultra tools aren't on Free at all. [S2]
- Each person has their own allowance on team plans. Nothing is pooled. [S2]
- Conversational design and video clips are Ultra tools and use the most. [S2]
- Bigger files and multi-step Canva AI 2.0 tasks use more. [S2]
- Designs generated inside ChatGPT, Claude, Copilot and other connected assistants can come out of your Canva allowance. [S2]
- Third-party AI apps in the Marketplace have their own limits and subscriptions. [S2]
- Free trials of Pro and Business only get the Free allowance. [S2]
- A manual AI top-up can't be cancelled once bought. [S53]
- AI Pass is charged per person, per month. [S52]
- "Fair use limits apply", even where Canva says unlimited. [S1][S2]
- Check your balance at profile icon > **Settings** > **Billing** > **AI usage**. [S2]

### Your data and AI training

- **Free and Pro.** Canva's Privacy Settings let you control whether your data can improve its AI features. [S40]
- Canva's Terms of Use (19 August 2026) say the setting covers your general usage data and your own content. [S42]
- We couldn't find a current Canva page saying whether this setting starts on or off. When Canva launched Magic Studio on 4 October 2023, it said "By default, Canva doesn't use your content" to train its AI. [S47]
- Canva's AI page links to a privacy settings page where you can check yours. [S10]
- **Business, Teams and Enterprise.** Canva's Trust Center says it doesn't use "business, team or enterprise content" to improve AI, and the setting is greyed out for these accounts. [S40]
- It says the option for admins to opt in is "coming soon". [S40]
- Canva's Master Services Agreement (21 May 2026), for customers who sign an Order Form, says Canva won't train its AI on customer material unless a customer administrator opts in "via the admin settings". [S48]
- **Education.** "We will not use User Content of Canva Education for AI training." [S41][S42] Education users can't change this setting. [S40]
- **Creators** who publish templates on Canva control whether their content is used to improve AI features. [S40]
- **The Canva AI beta.** If you've accepted an invitation to Canva's AI beta, your "AI consent settings in your Account Settings do not apply" to beta data (terms updated 15 April 2026). [S50]
- Beta inputs and outputs can be used to train Canva's models, and Canva staff can view them. [S50]
- To leave the beta, turn off the **CanvaAI Beta** toggle on your Canva privacy settings page. [S50]
- **Who else handles it.** Canva may pass inputs to outside "Technology Partners" to run a feature. [S43] Its sub-processor list names Anthropic, OpenAI, Google, ElevenLabs and others for AI services, mostly in the United States. [S49]
- For schools, Canva's Privacy Policy lists OpenAI among providers that process student data "for the sole purpose of delivering" Canva AI products. [S41]
- **Memory Library** builds a profile from your designs and prompts. Turn it off under **AI personalization** if you don't want that. [S12]
- **Connected assistants.** Content an assistant reads from Canva is handled under that company's terms as well as Canva's. [S42] Canva "makes no representations or warranties" about third-party services. [S42]
- We found no statement of how long Canva keeps AI prompts and outputs. [S41][S43]

### Admin controls

- Canva AI can't be fully switched off, but admins can control who uses each feature. [S8][S36]
- Enterprise organisation admins set defaults for every team and choose whether team admins can override them, under **Permissions** > **Team management** > **Team Overrides**. [S37]
- Enterprise organisation defaults can be **Everyone**, **Team admins and team brand designers**, **Team admins only** or **No one**. [S37]
- Turning the AI Connector off stops everyone on the team and breaks existing connections. [S56]
- If an app category is blocked for the admin role, it's hidden from admins too. [S106]
- A language setting can hide features even when admins have switched them on. [S36]

### Schools and students

- Canva Education is free for eligible K–12 teachers and schools anywhere in the world. [S39]
- "Teachers need to get parental consent for children below 13." [S39]
- Canva's AI Safety page says its AI products are for people 13 and over "unless used as part of Canva Education" under teacher supervision. [S44]
- In July 2025 Canva said its "AI for All Ages" policy lets students under 13 explore its AI tools in teacher- and admin-controlled settings. [S76]
- Default access: "Only administrators and teachers have access by default." [S36]
- The same page says "Magic Media, Dream Lab, and Magic Insights are the only features enabled for students." [S36] It doesn't say whether that means they're on by default, or that they're the only ones that can be turned on.
- Other Canva pages say admins and teachers can turn on Magic Write and Magic Edit for students. [S14][S21]
- Image to Video is off for students by default. [S19]
- "AI connectors are blocked for all Education users" by default. [S38]
- Generative AI apps and social media apps are blocked for students and allowed for teachers by default. Admins can change this. [S38]
- Students under 18 need administrator approval for third-party apps. [S38]
- Canva in Gemini doesn't work with school Google accounts. [S96]
- Canva AI tools inside Affinity are for admins and teachers only, for now. [S36]
- Student accounts inactive for more than 12 months get a deletion notice, and are deleted if nobody logs in within 3 months. [S41]
- Canva's World Teachers' Day post (5 October 2026) says student accounts that don't need an email address are expanding worldwide from October. [S75]

### Accuracy and checking

- Canva's AI page says to review outputs "especially where accuracy is important because AI can make mistakes". [S10]
- Canva's AI terms say it "has not verified the accuracy of the Output", and recommend independent professional advice before you act on it. [S43]
- The same terms ban using its AI to give "tailored advice that requires a license", such as legal or medical advice. [S43]
- AI charts start with sample data. [S28]
- Magic Formulas results need double-checking. [S33]
- Magic Write's help page says its data stops at mid-2021. [S14]
- Help Assistant's answers need double-checking. [S35]
- ChatGPT can make links that look like Canva links but go nowhere. [S60]
- Translate gives no accuracy warning. [S27]
- Canva Code's help page says nothing about checking security or accessibility. [S29]
- Canva's Master Services Agreement says output "may not be accurate, reliable, complete, unique, or exclusive", and customers must provide human oversight. [S48]

### Copyright, likeness and disclosure

These points come from Canva's "How to use Magic Studio safely and legally" page unless another source is shown.
- You can use AI-created work for personal and commercial purposes if you follow the AI Product Terms. [S51]
- "As between you and Canva", you own what the AI creates. But many places, including the US, don't give AI-made works copyright protection. [S51]
- Others may get similar results from similar prompts, so Canva can't guarantee your work is unique. [S51][S43]
- Don't prompt for existing brands, characters or people without permission. Get permission before using a recognisable person's image. [S51]
- Canva says it's "best practice" to tell your audience when content was made with AI help. [S51]
- Don't remove provenance tags or metadata, such as C2PA data, from AI content. [S43]
- Canva "does not guarantee" that AI images, designs or text are "cleared for use", especially if they resemble existing work. [S10]
- Canva says it "makes no copyright claim" over content you generate with Canva AI. [S10]

### Connections to outside assistants

- A connected assistant can create and edit designs as well as read them. [S56]
- It can reach anything you can view, including folders shared with you. [S59]
- Where the assistant allows it, turn the connector on only in the chats that need it. Claude lets you do this per chat. [S61][S92]
- Only the designs you pick in ChatGPT are saved, so check your Canva projects. [S60]
- When someone leaves, disconnect from both sides (our advice). [S59]

## Announced changes

Newsroom dates come from each page's publishing data, in UTC.

| Date | What changed | Source |
|---|---|---|
| 4 Oct 2023 | Magic Studio launched. Canva said it doesn't use your content to train its AI by default. | [S47] |
| 18 Jun 2025 | "Create a Video Clip" launched, built with Google's Veo 3, for paid plans and Nonprofits, starting at 5 a month. | [S107] |
| 22 Jul 2025 | "AI for All Ages" policy for students under 13 in teacher- and admin-controlled settings. | [S76] |
| 30 Oct 2025 | Canva Business launched. Canva Teams closed to new sign-ups and upgrades. | [S55][S54] |
| Nov 2025 | Canva connector added to Claude's directory. | [S91] |
| 25 Jan 2026 | Brand Kits work in the Claude connector. | [S67] |
| 11 Mar 2026 | Magic Layers in public beta in the US, the UK, Canada and Australia. | [S26] |
| 15 Apr 2026 | Canva AI Beta Program Terms updated. | [S50] |
| 16 Apr 2026 | Canva AI 2.0 announced as a research preview, with general availability "over the coming weeks". | [S11] |
| 17 Apr 2026 | Canva in Claude Design announced. Canva's sub-processor list updated. | [S71][S49] |
| 21 May 2026 | Master Services Agreement updated. | [S48] |
| 8 Jun 2026 | Magic Layers inside ChatGPT and Gemini. Canva says both connections are available to all users globally. | [S69] |
| 26 Jun 2026 | AI Product Terms take effect. | [S43] |
| 1 Jul 2026 | Google starts rolling out Canva support in Gemini Spark. | [S99] |
| 9 Jul 2026 | OpenAI replaces ChatGPT's App Directory with a Plugin Directory. Existing app connections carry on. | [S113] |
| 14 Jul 2026 | Canva Code 2.0 available to Free, Pro, Business, Enterprise and Education users. | [S31] |
| 16 Jul 2026 | Canva in Gemini expanded, and Canva added to AI Mode in Google Search. | [S68] |
| 19 Aug 2026 | Terms of Use take effect. | [S42] |
| 25 Aug 2026 | Privacy Policy updated. | [S41] |
| 2 Sep 2026 | Visual Suite updates, including charts from Sheets data and AI presenter notes, "rolling out now to all Canva users globally". | [S74] |
| 16 Sep 2026 | Canva ProSuite announced (Affinity, Cavalry, Flourish and Leonardo.Ai). Canva AI Studio in Affinity needs a premium plan. Cavalry AI tools "coming soon". | [S72] |
| No date shown | Leonardo.Ai Essential is no longer a built-in benefit of Business or Enterprise. | [S73] |
| 29 Sep 2026 | Canva connector for Meta's Muse, US and Canada only. | [S70] |
| 1 Oct 2026 | Microsoft lists Canva as a ready-to-deploy Agent 365 partner agent. | [S100] |
| 5 Oct 2026 | Student accounts without email addresses expanding worldwide from October. | [S75] |

**Announced with no date**

- Admin opt-in to AI training for Business, Teams and Enterprise is "coming soon". [S40]
- Usage limits for the AI Connector: "We'll introduce usage limits in the future." [S56]
- Canva AI 2.0 and Canva AI connectors are marked "Soon" for Enterprise on the pricing page. [S1]
- More admin controls over student AI access in Affinity. [S36]
- Memory Library and Canva AI 2.0 features are rolling out gradually. [S8][S9]
- Canva isn't accepting third-party connectors for Canva AI yet, and gives no timeline. [S81]
- Usage limits for the autofill API will be introduced later. [S85]
- New Cavalry AI tools (Remove Background, Generate Vector and Image to Layers) are "coming soon". [S72]

## What we couldn't establish

- **Which ChatGPT plans can use the Canva plugin.** OpenAI's pages say it depends on plan, workspace, role and region, and its Canva page lists no plans. [S110][S108] A search-engine snippet said Free and Go plans can't use plugin extensions. OpenAI's release note introducing extensions names no plans, so we couldn't confirm it. [S113]
- **Today's default for Canva's AI-training setting** on Free and Pro, and the setting's exact label. Canva's current pages don't state the default, and the setting sits behind a sign-in. The only "off by default" statement we found is from October 2023. [S40][S47]
- **Admin opt-in for AI training.** The Trust Center says it's "coming soon" for Business, Teams and Enterprise, while the Master Services Agreement already refers to opting in "via the admin settings". We couldn't find that setting in Canva's admin help. [S40][S48][S36]
- **Plan rules for connector actions.** Canva's pages disagree on Brand Template search, autofill and resize. See the table under "Canva's AI Connector". [S56][S57][S59][S77][S96]
- **Who gets conversational design.** Help pages list either Pro, Teams, Business and Nonprofit, or Pro, Business and Enterprise. The pricing page marks Enterprise "Soon". [S3][S5][S1]
- **AI Pass for Business.** The help page says 20 times more AI and the pricing page says 40 times. [S52][S1]
- **Which tier some tools sit in.** Magic Formulas is Standard on the usage page and premium on its own page. "Create an image with Canva AI" appears under more than one tier, and Canva AI for Sheets contradicts itself. [S2][S32][S33]
- **Whether DALL·E and Imagen use your Canva allowance.** The usage page says Marketplace AI apps don't, while the DALL·E and Imagen page calls them a limited premium AI tool. [S2][S20]
- **Student defaults in Canva Education.** One sentence calls Magic Media, Dream Lab and Magic Insights "the only features enabled for students" without saying whether they're on by default. [S36]
- **What "AI connectors are blocked" covers in Education**, and whether K–12 teachers can use the AI Connector. [S38][S59]
- **AUD prices for monthly plans, AI Pass and AI top-ups.** The Australian pricing page shows yearly prices and no add-on prices. [S1] Canva's AI Pass help page gives a price in US dollars only, so we haven't quoted it. [S52]
- **How long Canva keeps AI prompts, outputs and Canva AI chats.** Not stated in the pages we read. [S8][S41][S43]
- **An Australia-only hosting option.** We didn't find one. The Trust Center says data is stored in the US, while the Privacy Policy lists Australia among several storage and processing countries. [S40][S41]
- **Which model powers each feature.** Canva names OpenAI for Magic Write, on a page that may be out of date, and named Google's Veo 3 for video clips at launch. The sub-processor list names the AI companies but not which feature each one serves. [S14][S107][S49]
- **The AI indemnity's contract terms.** The 100-seat threshold comes from Canva's AI marketing page, and we couldn't find indemnity wording for AI output in the Master Services Agreement. [S10][S48]
- **Microsoft's side.** Which licence the Canva agent needs, whether it counts as a no-cost agent for Copilot Chat, what it can read and change, whether it's offered in Australia, and how Microsoft handles the content. A Microsoft Tech Community post about partner apps in Copilot wouldn't load for us. [S63][S100][S102]
- **Claude Team and Enterprise data terms** for connector content. Anthropic's training page covers consumer plans only. [S94]
- **Whether every action in a connected assistant uses your Canva allowance.** Canva says AI actions "may", and that limits are coming. [S56][S2]
- **AI Mode in Google Search in Australia.** Not stated. [S68]
- **Tools we didn't research one by one:** AI Voice, the Music and Sound Effect Generator, Magic Animate, alt text suggestions, Magic Activities, Transform into Doc, AI Shapes, Background Remover, Image Upscaler, Canva Grow, and signing in to Leonardo.Ai with a Canva account.
- **The other assistants on Canva's list**, including Amazon Quick Suite and Perplexity Computer. Not researched. [S58][S59]
- **Our web search allowance ran out** partway through. After that we checked leads only by opening vendor pages we already had addresses for.

## Sources

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Canva pricing (English, Australia) | Canva | https://www.canva.com/en_au/pricing/ | No date shown | 15 Oct 2026 |
| S2 | Understanding your AI usage | Canva Help Center | https://www.canva.com/help/ai-access/ | No date shown | 15 Oct 2026 |
| S3 | Get started with Canva AI | Canva Help Centre | https://www.canva.com/en_au/help/using-canva-ai/ | No date shown | 15 Oct 2026 |
| S4 | What's new in Canva AI | Canva Help Centre | https://www.canva.com/en_au/help/new-canva-ai/ | No date shown | 15 Oct 2026 |
| S5 | Use Canva AI to refine designs through conversation | Canva Help Center | https://www.canva.com/help/canva-design-assistant/ | No date shown | 15 Oct 2026 |
| S6 | Use Ask Canva for AI-powered design edits | Canva Help Center | https://www.canva.com/help/edit-designs-with-ask-canva/ | No date shown | 15 Oct 2026 |
| S7 | Generate unique designs instantly with AI | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-design/ | No date shown | 15 Oct 2026 |
| S8 | Canva AI Frequently Asked Questions | Canva Help Center | https://www.canva.com/help/new-canva-ai-faq/ | No date shown | 15 Oct 2026 |
| S9 | Fix issues and improve results with Canva AI | Canva Help Center | https://www.canva.com/help/fix-canva-ai-issues/ | No date shown | 15 Oct 2026 |
| S10 | Canva AI 2.0 (product page) | Canva | https://www.canva.com/canva-ai/ | No date shown | 15 Oct 2026 |
| S11 | Introducing Canva AI 2.0: Reimagining how the world creates | Canva Newsroom | https://www.canva.com/newsroom/news/canva-create-2026-ai/ | No date shown; page data 16 Apr 2026 | 15 Oct 2026 |
| S12 | Use Memory Library to personalize Canva AI | Canva Help Center | https://www.canva.com/help/living-memory/ | No date shown | 15 Oct 2026 |
| S13 | Use Magic Write to generate text | Canva Help Centre | https://www.canva.com/en_au/help/use-magic-write/ | No date shown | 15 Oct 2026 |
| S14 | Learn about Magic Write | Canva Help Centre | https://www.canva.com/en_au/help/about-magic-write/ | No date shown | 15 Oct 2026 |
| S15 | Use Magic Media to create photos, graphics, and videos | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-media/ | No date shown | 15 Oct 2026 |
| S16 | Generate images with Dream Lab | Canva Help Centre | https://www.canva.com/en_au/help/generate-with-dreamlab/ | No date shown | 15 Oct 2026 |
| S17 | Dream Lab access restrictions | Canva Help Centre | https://www.canva.com/en_au/help/dreamlab-access-restrictions/ | No date shown | 15 Oct 2026 |
| S18 | Create a video clip in Canva AI 1.0 | Canva Help Centre | https://www.canva.com/en_au/help/video-clip/ | No date shown | 15 Oct 2026 |
| S19 | Transform your image into a video | Canva Help Centre | https://www.canva.com/en_au/help/image-to-video/ | No date shown | 15 Oct 2026 |
| S20 | Use AI image generation apps | Canva Help Centre | https://www.canva.com/en_au/help/ai-image-generation-apps/ | No date shown | 15 Oct 2026 |
| S21 | Use Magic Edit to add, replace, and modify photos | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-edit/ | No date shown | 15 Oct 2026 |
| S22 | Make your photo selectable and customisable with Magic Grab | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-grab/ | No date shown | 15 Oct 2026 |
| S23 | Erase or retouch photos | Canva Help Centre | https://www.canva.com/en_au/help/magic-eraser/ | No date shown | 15 Oct 2026 |
| S24 | Expanding images | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-expand/ | No date shown | 15 Oct 2026 |
| S25 | Turn images into editable layers with Magic Layers | Canva Help Centre | https://www.canva.com/en_au/help/editable-magic-layers/ | No date shown | 15 Oct 2026 |
| S26 | Introducing Magic Layers, bringing creative control to AI content | Canva Newsroom | https://www.canva.com/newsroom/news/magic-layers/ | No date shown; page data 11 Mar 2026 | 15 Oct 2026 |
| S27 | Translate your Canva designs | Canva Help Centre | https://www.canva.com/en_au/help/translate-canva-designs/ | No date shown | 15 Oct 2026 |
| S28 | Generate charts with AI | Canva Help Centre | https://www.canva.com/en_au/help/ai-charts/ | No date shown | 15 Oct 2026 |
| S29 | Create interactive designs with Canva Code | Canva Help Centre | https://www.canva.com/en_au/help/canva-code/ | No date shown | 15 Oct 2026 |
| S30 | Canva Code access restrictions | Canva Help Center | https://www.canva.com/help/canva-code-restrictions/ | No date shown | 15 Oct 2026 |
| S31 | Vibe coding that matches your vision: Canva Code 2.0 is now available to all | Canva Newsroom | https://www.canva.com/newsroom/news/Canva-Code/ | No date shown; page data 14 Jul 2026 | 15 Oct 2026 |
| S32 | Use Canva AI 2.0 for Sheets | Canva Help Center | https://www.canva.com/help/canva-sheets-assistant/ | No date shown | 15 Oct 2026 |
| S33 | Use AI to write functions and formulas for Canva Sheets | Canva Help Center | https://www.canva.com/help/use-magic-formulas/ | No date shown | 15 Oct 2026 |
| S34 | Analyse and summarise Canva Sheets data with Magic Insights | Canva Help Centre | https://www.canva.com/en_au/help/magic-insights/ | No date shown | 15 Oct 2026 |
| S35 | Get quick help with Help Assistant | Canva Help Centre | https://www.canva.com/en_au/help/ai-powered-assistant/ | No date shown | 15 Oct 2026 |
| S36 | Change access to Magic and AI features | Canva Help Centre | https://www.canva.com/en_au/help/magic-features-admin-controls/ | No date shown | 15 Oct 2026 |
| S37 | Manage access and feature controls for your organisation | Canva Help Centre | https://www.canva.com/en_gb/help/admin-controls-for-enterprise/ | No date shown | 15 Oct 2026 |
| S38 | App Restrictions for Students | Canva Help Centre | https://www.canva.com/en_au/help/app-restrictions-c4e/ | No date shown | 15 Oct 2026 |
| S39 | About Canva Education | Canva Help Centre | https://www.canva.com/en_au/help/about-canva-for-education/ | No date shown | 15 Oct 2026 |
| S40 | Trust Center: Privacy | Canva | https://www.canva.com/trust/privacy/ | No date shown | 15 Oct 2026 |
| S41 | Privacy Policy | Canva | https://www.canva.com/policies/privacy-policy/ | Last updated 25 Aug 2026 | 15 Oct 2026 |
| S42 | Terms of Use | Canva | https://www.canva.com/policies/terms-of-use/ | Effective 19 Aug 2026 | 15 Oct 2026 |
| S43 | AI Product Terms | Canva | https://www.canva.com/policies/ai-product-terms/ | Effective 26 Jun 2026 | 15 Oct 2026 |
| S44 | AI Safety at Canva | Canva | https://www.canva.com/policies/ai-safety/ | No date shown | 15 Oct 2026 |
| S45 | Canva Shield (Safe AI) | Canva | https://www.canva.com/safe-ai-canva-shield/ | No date shown | 15 Oct 2026 |
| S46 | Canva Shield: Safe, fair and secure AI | Canva Newsroom | https://www.canva.com/newsroom/news/safe-ai-canva-shield/ | No date shown; page data 5 Jan 2026 | 15 Oct 2026 |
| S47 | Introducing Magic Studio: the power of AI, all in one place | Canva Newsroom | https://www.canva.com/newsroom/news/magic-studio/ | No date shown; page data 4 Oct 2023 | 15 Oct 2026 |
| S48 | Canva Master Services Agreement | Canva | https://www.canva.com/policies/msa/ | Last updated 21 May 2026 | 15 Oct 2026 |
| S49 | Canva List of Subprocessors (PDF, linked from https://www.canva.com/policies/subprocessors/) | Canva | https://content-management-files.canva.com/assets/en/f6022a49-58d4-40d8-88d3-803529880cc0 | Last updated 17 Apr 2026 | 15 Oct 2026 |
| S50 | Canva AI Beta Program Terms | Canva | https://www.canva.com/policies/beta-service-terms/ | Last updated 15 Apr 2026 | 15 Oct 2026 |
| S51 | How to use Magic Studio safely and legally | Canva Help Centre | https://www.canva.com/en_au/help/using-magic-studio-safely-and-legally/ | No date shown | 15 Oct 2026 |
| S52 | Understanding AI Pass | Canva Help Centre | https://www.canva.com/en_au/help/ai-pass/ | No date shown | 15 Oct 2026 |
| S53 | Understanding AI top-ups | Canva Help Center | https://www.canva.com/help/ai-top-ups/ | No date shown | 15 Oct 2026 |
| S54 | About Canva Teams | Canva Help Centre | https://www.canva.com/en_au/help/about-canva-teams/ | No date shown | 15 Oct 2026 |
| S55 | Meet Canva Business: A powerful new plan for small businesses with big ambitions | Canva Newsroom | https://www.canva.com/newsroom/news/introducing-canva-business/ | No date shown; page data 30 Oct 2025 | 15 Oct 2026 |
| S56 | Connect Canva to an AI assistant (also read at /help/mcp-agent-setup/) | Canva Help Centre | https://www.canva.com/en_au/help/mcp-agent-setup/ | No date shown | 15 Oct 2026 |
| S57 | Actions you can take in AI assistants connected to Canva MCP | Canva Help Center | https://www.canva.com/help/mcp-canva-usage/ | No date shown | 15 Oct 2026 |
| S58 | Connect AI assistants and tools to Canva | Canva Help Center | https://www.canva.com/help/ai-connectors-canva/ | No date shown | 15 Oct 2026 |
| S59 | Design smarter than ever with Canva's AI Connector | Canva | https://www.canva.com/ai-connector/ | No date shown | 15 Oct 2026 |
| S60 | Connect your Canva account to ChatGPT (also read at /help/connect-chatgpt-to-canva/) | Canva Help Centre | https://www.canva.com/en_au/help/connect-chatgpt-to-canva/ | No date shown | 15 Oct 2026 |
| S61 | Connect your Canva account to Claude | Canva Help Center | https://www.canva.com/help/connect-claude-to-canva/ | No date shown | 15 Oct 2026 |
| S62 | Connect your Canva account to Gemini | Canva Help Center | https://www.canva.com/help/connect-gemini-to-canva/ | No date shown | 15 Oct 2026 |
| S63 | Connect your Canva account to Microsoft Copilot (also read at /help/connect-copilot-to-canva/) | Canva Help Centre | https://www.canva.com/en_au/help/connect-copilot-to-canva/ | No date shown | 15 Oct 2026 |
| S64 | Manage Cross app access for Enterprise | Canva Help Center | https://www.canva.com/help/manage-cross-app-access | No date shown | 15 Oct 2026 |
| S65 | Connect third-party apps to Canva AI | Canva Help Center | https://www.canva.com/help/connect-apps-canva-ai/ | No date shown | 15 Oct 2026 |
| S66 | Import files from third-party apps to Canva AI | Canva Help Center | https://www.canva.com/help/import-to-canva-ai/ | No date shown | 15 Oct 2026 |
| S67 | Create on-brand Canva designs directly inside Claude | Canva Newsroom | https://www.canva.com/newsroom/news/claude-ai-connector/ | No date shown; page data 25 Jan 2026 | 15 Oct 2026 |
| S68 | Canva expands design creation inside Google Gemini and AI Search | Canva Newsroom | https://www.canva.com/newsroom/news/google-gemini/ | No date shown; page data 16 Jul 2026 | 15 Oct 2026 |
| S69 | Make AI images your own: Magic Layers is now inside the world's biggest AI assistants | Canva Newsroom | https://www.canva.com/newsroom/news/magic-layers-ai-assistants/ | No date shown; page data 8 Jun 2026 | 15 Oct 2026 |
| S70 | Canva expands design with Muse, from Meta | Canva Newsroom | https://www.canva.com/newsroom/news/canva-meta-muse/ | No date shown; page data 29 Sep 2026 | 15 Oct 2026 |
| S71 | Introducing Canva in Claude Design by Anthropic Labs | Canva Newsroom | https://www.canva.com/newsroom/news/canva-claude-design/ | No date shown; page data 17 Apr 2026 | 15 Oct 2026 |
| S72 | Craft, upgraded: introducing the Canva ProSuite | Canva Newsroom | https://www.canva.com/newsroom/news/canva-prosuite-launch/ | No date shown; page data 16 Sep 2026 | 15 Oct 2026 |
| S73 | Canva ProSuite for Business and Enterprise | Canva | https://www.canva.com/business/pro-suite/ | No date shown | 15 Oct 2026 |
| S74 | Big updates just landed in the Visual Suite | Canva Newsroom | https://www.canva.com/newsroom/news/visual-suite-100-updates/ | No date shown; page data 2 Sep 2026 | 15 Oct 2026 |
| S75 | This World Teachers' Day: celebrating what teachers make possible | Canva Newsroom | https://www.canva.com/newsroom/news/world-teachers-day-2026/ | No date shown; page data 5 Oct 2026 | 15 Oct 2026 |
| S76 | Bringing free education tools to 100 million people | Canva Newsroom | https://www.canva.com/newsroom/news/100-million-education-milestone/ | No date shown; page data 22 Jul 2025 | 15 Oct 2026 |
| S77 | MCP tools and rate limits | Canva Developers | https://www.canva.dev/docs/apps/mcp/tools.md | No date shown | 15 Oct 2026 |
| S78 | Access and permissions (Canva MCP) | Canva Developers | https://www.canva.dev/docs/apps/mcp/access.md | No date shown | 15 Oct 2026 |
| S79 | Usage Policy (Canva MCP server) | Canva Developers | https://www.canva.dev/docs/apps/mcp/usage-policy.md | No date shown | 15 Oct 2026 |
| S80 | Prohibited use (Canva MCP) | Canva Developers | https://www.canva.dev/docs/apps/mcp/prohibited-use.md | No date shown | 15 Oct 2026 |
| S81 | Connectors in Canva AI | Canva Developers | https://www.canva.dev/docs/apps/mcp/canva-ai.md | No date shown | 15 Oct 2026 |
| S82 | Dev MCP server | Canva Developers | https://www.canva.dev/docs/apps/dev-mcp-server/ | No date shown | 15 Oct 2026 |
| S83 | Canva Developers SDK documentation | Canva Developers | https://www.canva.dev/docs/apps/ | No date shown | 15 Oct 2026 |
| S84 | About Canva's REST APIs | Canva Developers | https://www.canva.dev/docs/connect/ | No date shown | 15 Oct 2026 |
| S85 | Autofill guide (REST APIs) | Canva Developers | https://www.canva.dev/docs/apps/rest-apis/autofill-guide.md | No date shown | 15 Oct 2026 |
| S86 | Managing team apps | Canva Developers | https://www.canva.dev/docs/apps/managing-team-apps.md | No date shown | 15 Oct 2026 |
| S87 | App review process | Canva Developers | https://www.canva.dev/docs/apps/app-review-process.md | No date shown | 15 Oct 2026 |
| S88 | Authentication (REST APIs) | Canva Developers | https://www.canva.dev/docs/apps/rest-apis/authentication.md | No date shown | 15 Oct 2026 |
| S89 | Canva for AI agents | Canva Developers | https://www.canva.dev/agents/ | No date shown | 15 Oct 2026 |
| S90 | canva-sdks/canva-skills | Canva (GitHub) | https://github.com/canva-sdks/canva-skills | No date shown | 15 Oct 2026 |
| S91 | Canva connector listing | Anthropic (claude.com) | https://claude.com/connectors/canva | "Added November 2025" | 15 Oct 2026 |
| S92 | Use connectors to extend Claude's capabilities | Claude Help Center (Anthropic) | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated over 2 weeks ago" (no calendar date) | 15 Oct 2026 |
| S93 | Use interactive connectors in Claude | Claude Help Center (Anthropic) | https://support.claude.com/en/articles/13454812-use-interactive-connectors-in-claude | 11 Aug 2026 | 15 Oct 2026 |
| S94 | Is my data used for model training? | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | 16 Mar 2026 | 15 Oct 2026 |
| S95 | Supported countries and regions | Anthropic | https://www.anthropic.com/supported-countries | Effective 12 May 2026 | 15 Oct 2026 |
| S96 | Create designs & build websites with your creative apps in Gemini Apps | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/17081444?hl=en | No date shown | 15 Oct 2026 |
| S97 | Use & manage Connected Apps in Gemini | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/13695044?hl=en | No date shown | 15 Oct 2026 |
| S98 | Gemini Apps Privacy Hub | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/13594961?hl=en | Last updated 13 Oct 2026 | 15 Oct 2026 |
| S99 | What's new for Gemini Spark | Gemini Apps Help (Google) | https://support.google.com/gemini/answer/17171264?hl=en-GB | Dated entries; Canva entry 1 Jul 2026 | 15 Oct 2026 |
| S100 | Ecosystem partner agents available in Agent 365 | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-agent-365/third-party-agents | 1 Oct 2026 (updated 2 Oct 2026) | 15 Oct 2026 |
| S101 | Get more agents in the Microsoft Copilot app | Microsoft Support | https://support.microsoft.com/en-US/Microsoft-365-Copilot/get-more-agents-in-the-microsoft-365-copilot-app | No date shown | 15 Oct 2026 |
| S102 | Prerequisites: Microsoft Copilot agent governance | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/agent-essentials/agent-prerequisites | 17 Jun 2026 (updated 18 Aug 2026) | 15 Oct 2026 |
| S103 | Get started with Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/get-started | 14 Sep 2026 (updated 21 Sep 2026) | 15 Oct 2026 |
| S104 | Connected apps in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/11487775-connected-apps-in-chatgpt | "Updated: 4 days ago" (11 Oct 2026, UTC) | 15 Oct 2026 |
| S105 | About Canva Pro Lite | Canva Help Centre | https://www.canva.com/en_au/help/pro-lite/ | No date shown | 15 Oct 2026 |
| S106 | Manage third-party app integrations (admin controls) | Canva Help Center | https://www.canva.com/help/admin-control-third-party-app-integrations/ | No date shown | 15 Oct 2026 |
| S107 | Google's Veo 3 comes to Canva: Introducing Create a Video Clip | Canva Newsroom | https://www.canva.com/newsroom/news/veo3-canva-ai-video/ | No date shown; page data 18 Jun 2025 | 15 Oct 2026 |
| S108 | Canva plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/canva/ | No date shown | 15 Oct 2026 |
| S109 | Canva (ChatGPT plugin listing) | OpenAI | https://chatgpt.com/plugins/plugin_connector_68df33b1a2d081918778431a9cfca8ba | No date shown; version 17.0.1 | 15 Oct 2026 |
| S110 | Plugins in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001256-plugins-in-chatgpt | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S111 | Connecting and managing app accounts in ChatGPT | OpenAI Help Center | https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt | "Updated: 13 days ago" (2 Oct 2026, UTC) | 15 Oct 2026 |
| S112 | Admin controls, security, and compliance for plugins and apps | OpenAI Help Center | https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-for-plugins-and-apps | "Updated: 17 hours ago" (14 Oct 2026, UTC) | 15 Oct 2026 |
| S113 | ChatGPT release notes | OpenAI Help Center | https://help.openai.com/en/articles/6825453-chatgpt-release-notes | "Updated: 6 days ago" (9 Oct 2026, UTC) | 15 Oct 2026 |
