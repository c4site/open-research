# Shopify: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- Shopify's built-in AI assistant is called Sidekick. It's listed on all four main plans on Shopify's Australian pricing page, and Shopify says it's available globally. [S1] [S47]
- Sidekick can answer questions about your sales and edit products for you. It shows you changes for review before it applies them. [S3] [S4]
- Shopify has official connections for Claude, ChatGPT, Microsoft Copilot and Gemini. If you approve write access, each can change products, collections, stock levels and discount codes. [S21] [S22] [S23] [S24] [S25]
- Even with write access, none of them can issue refunds, cancel orders, change payment settings or edit your live theme. [S27]
- Google lists the Shopify app in Gemini as US only and English only, for personal Google accounts. Going by Google's table, Australian users can't use it yet. [S81]
- Shopify also shows your products to shoppers inside ChatGPT, Microsoft Copilot and Google's AI Mode and Gemini. It's on by default, but every one of those channels needs you to sell to US customers. [S31] [S33] [S34] [S35]
- Once you share store data with an outside AI, Shopify says it no longer processes that data and the AI company's terms apply. [S27]
- Shopify says store data is never used to train foundation models or shared with other merchants. Its sub-processor list names AI providers for Sidekick, including Anthropic, OpenAI and Microsoft, all in the US. [S9] [S42]
- On the Australian pricing page, Basic is $56 a month paid monthly and Plus starts at $3,700. The Agentic plan costs $0 a month, for brands that only want to sell in AI channels. [S1]

## The tool, and the plans that matter

Shopify describes itself as an all-in-one commerce platform. You use it to run an online store and take payments, and to sell on social channels and in person. [S1]

These are the prices on Shopify's Australian pricing page as read on 17 October 2026, in AUD. The page doesn't say whether they include GST. [S1]

| Plan | Paid monthly | Paid yearly (per month) | AI rows in Shopify's comparison table | Online card rate with Shopify Payments |
|---|---|---|---|---|
| Basic | $56 | $50 | "Sidekick, AI assistant for commerce", "Millions of tokens", "Sell in AI chats" | 1.7% + 30¢ |
| Grow | $149 | $134 | Same rows. Generating custom apps with Sidekick starts here. | 1.55% + 30¢ |
| Advanced | $575 | $519 | Same rows as Grow | 1.35% + 30¢ |
| Plus | Starts at $3,700 | Not shown | Same rows as Grow | 1.15% + 30¢ |
| Agentic | $0 | Not applicable | "For selling in AI channels". Your products go into Shopify Catalog and you choose which AI channels to sell in. | From 1.7% + 30¢ |

Sources for the table: [S1] [S7]

- New stores get a three-day free trial, then $1 a month for three months on Basic, Grow and Advanced. [S1]
- POS Pro for shop counters is an add-on at $129 a month per location. [S1]
- The comparison table puts "Website builder", "Millions of tokens" and "Sidekick, AI assistant for commerce" under a heading called "AI features" on all four main plans. Shopify doesn't explain what the token allowance covers. [S1]
- Shopify's Sidekick page says Sidekick is included with your plan and "Features and usage limits vary by plan." [S8]
- The Agentic plan is for merchants who don't already use Shopify for their online store. It has no monthly subscription fee, but payment fees apply when a customer buys through an AI channel's checkout. [S38]
- On the Agentic plan your online store stays password-protected and you can't sell through its checkout. To do that you move to a paid plan. [S38]
- Shopify's help pages also mention a Starter plan. It wasn't on the Australian pricing page we read. [S12] [S37] [S1]

**Words used in this guide**

- **Sidekick** is Shopify's AI assistant inside the Shopify admin, the back office where you run your store. [S3]
- **Agentic storefronts** is Shopify's name for selling your products inside AI chat apps. [S30]
- **Shopify Catalog** is the product listing Shopify shares with those AI apps. [S36]
- An **API** is the door Shopify opens so other software can read or change your store. An **MCP server** is a standard way for an AI assistant to use that door. Shopify's connectors for Claude, ChatGPT, Gemini and Copilot all act through the Shopify Admin API. [S22] [S23] [S24] [S25]

## AI built in

Shopify's help centre now groups its AI features under "AI-powered tools", and names several of them after Sidekick. Some older help links still carry the earlier name, Shopify Magic. [S2]

### Sidekick (the AI assistant)

**What it does**

- Shopify calls Sidekick "an AI-enabled commerce assistant in your Shopify admin". It works within the context of your store. [S3]
- It can analyse data, manage orders, edit products and work with third-party apps. [S3]
- It writes blog posts and product descriptions, and it can create images. [S3]
- It can fill in forms across the admin, and create discounts, collections, customer segments, custom reports and Shopify Flow automations. Fields it fills are highlighted in purple for you to review. [S6]
- Longer tasks can keep running after you close the chat. Sidekick tells you when they're ready for review. [S3]
- Sidekick Pulse puts recommendations on your admin Home without you asking. [S3] [S43]
- Store owners can describe an app and have Sidekick build it. These apps work only inside your admin, but they can change customer-facing data, so Shopify says to test them first. [S7]
- Since June 2026, other apps can plug into Sidekick through App Extensions. Shopify named more than 15 launch partners, including Klaviyo and Loop. [S43]
- When an app changes something through Sidekick, Shopify's developer rules say the merchant confirms the change. [S57]
- Shopify's Sidekick page lists recent additions: creating customers and companies (10 February 2026), and customising checkout and customer account settings (13 October 2026). [S8]
- On 1 October 2026 Shopify started rolling out Canvas, a design space where Sidekick edits your theme's files directly. Shopify's Ben Sehl said "We're early here". [S44]

**Where to find it**

- In the Shopify admin, go to **Sidekick** or click the Sidekick icon. On the refreshed admin design, type into the Sidekick field and press Enter. [S4]
- In the Shopify mobile app, tap the Sidekick icon on any store page. Sidekick doesn't work in a mobile browser. [S4]
- On Apple Watch you can ask quick questions by voice. It can't make changes there. [S4]
- You can talk to Sidekick by voice or share your screen with it. [S3]

**Which plans have it**

- The Australian pricing page lists Sidekick on Basic, Grow, Advanced and Plus. [S1]
- Shopify says Sidekick costs nothing extra. [S8]
- Generating apps needs Grow, Advanced or Plus. The store shares an hourly limit and a weekly limit, and staff need the **App development** > **Develop** permission. [S7]
- Image generation has a monthly limit and a short-term limit that depend on your plan. Shopify doesn't publish the amounts. [S6]

**What happens to your data**

- Shopify says: "Store data is never used to train foundation models or shared with other merchants." This is from a June 2026 Shopify blog post. We didn't find it in Shopify's terms or privacy policy. [S9] [S40] [S41]
- Shopify says Sidekick can't make changes to your store without your approval. It presents options for you to approve. [S4]
- Every staff member can use Sidekick, limited to their own admin permissions. [S8]
- Sidekick remembers preferences you tell it, and past conversations for about three months. It also draws on what you've done in the admin over roughly the last 12 hours. [S5]
- You can switch memory off for a conversation or delete a conversation. You can also ask Sidekick to forget a detail. [S5]
- Shopify's sub-processor list names Anthropic, Applied Compute, Fireworks.ai, Microsoft and OpenAI for "Conversational artificial intelligence services". All are in the USA, and each handles "Personal data if input to or included in a response by Shopify Sidekick." [S42]
- Shopify's terms let it use your materials to "operate, provide, evaluate, enhance, improve, and promote the Services". The terms don't mention AI training by name. [S40]
- We didn't find a switch that turns Sidekick off for a whole store in the pages we read. [S3] [S4] [S8]

**In Australia**

- Shopify's Campaign Autopilot launch post says "Sidekick is available globally." [S47]
- Shopify says Sidekick follows your store's language settings and can help in several languages. [S8]
- Shopify's privacy policy says personal data of people in Australia is received by Shopify Commerce Singapore Pte. Ltd., and may be sent to other countries including the United States. [S41]

### Writing and image tools in the admin

**What it does**

- A **Generate text** icon writes product descriptions, blog posts, online store pages and Shopify Messaging emails from your prompt. [S2] [S11]
- In the file editor, **Generate** changes an image from a text prompt, and **Color background** swaps the background for a colour or makes it transparent. You can also extend an image past its edges. [S10]
- In the theme editor, Sidekick can build a custom theme block from a description. [S2]
- The Shopify app can generate up to three free themes from a description of your business. [S12]
- Smaller helpers suggest product categories, sort storefront filter values, describe customer segments in plain words, project customer spending in a cohort report and summarise App Store reviews. [S2]
- Tinker is a free Shopify phone app with more than 100 AI tools for images, video and brand assets. Its tools come from OpenAI, Google, Anthropic, Black Forest Labs, xAI and Kling. [S13]

**Where to find it**

- Product descriptions: **Products**, open a product, then click the **Generate text** icon in the description toolbar. It isn't supported on iPhone or Android. [S11]
- Images: open the file in the admin and click **Color background** or **Generate**. In the Shopify app, tap **Background** or **Generate**. [S10]
- Themes: in the Shopify app, go to **Online Store** > **Manage themes** > **Design your store in seconds**, then tap **Generate themes**. This no longer works from the desktop admin. [S12]
- Tinker is on iOS and Android and needs its own account, made with an email address or Google or Apple sign-in. [S13]

**Which plans have it**

- Shopify says many of these features cost nothing extra, but availability varies by plan, device and language. [S2]
- Media generation with Sidekick is on Basic, Grow, Advanced and Plus. Media generation in the file editor is on all plans at no extra cost "for a limited time". [S10]
- Shopify says that when your storefront is in English, you can generate free themes only during the free trial or on Basic, Grow or Advanced. Starter can't generate them. [S12]
- Tinker is free to download and use, with monthly usage limits that refresh automatically. [S13]

**What happens to your data**

- "Shopify doesn't claim ownership over images merchants create using media generation." You can use them for business inside and outside Shopify. [S10]
- Generated images carry an invisible watermark that can't be removed. [S10]
- Shopify says media generation uses several generative models and follows its privacy principles. The page says nothing about training. [S10]
- Generated product text can add benefits you didn't list, so Shopify says to check it closely. You're responsible for what you publish. [S11]
- Tinker keeps some information after you delete your account, for reasons such as fraud prevention and legal compliance. [S13]

**In Australia**

- Text generation works in all languages Shopify supports and writes in the language of your prompt. [S11]
- The pages we read for these tools don't mention country limits. [S10] [S11] [S13]

### Shopify Inbox: the Inbox agent and suggested replies

**What it does**

- The Inbox agent chats with customers on your storefront automatically. It answers questions about products, shipping, returns, sizing and policies. [S16]
- It answers from your product catalogue, store policies, Knowledge Base content and published pages. For a specific product it can also use cited web search for reviews and ratings. [S16] [S17]
- It hands a conversation to your staff when it can't answer or the customer asks for a person. [S17]
- Suggested replies draft answers for your staff to edit and send. They don't drive the agent's automatic replies. [S15]
- AI-suggested instant answers are based on your store policies. You choose which to keep and write the answers yourself. [S14]

**Where to find it**

- The agent's persona sits under **Sales channels** > **Inbox** in the **Persona** section. Click **Edit**, or click **Refine with Sidekick**. [S17]
- Suggested replies: in Shopify Inbox, click the settings icon, then **Message preferences**. Under **Automatically generate a reply**, choose **On** or **Off** and click **Save**. [S15]
- Instant answers: **Sales channels** > **Inbox** > **Chat settings** > **Instant answers**. [S14]

**Which plans have it**

- The Shopify Inbox app is made by Shopify and listed as free. [S19]
- The help pages we read don't name plans for the AI parts. [S14] [S15] [S16]

**What happens to your data**

- The Inbox agent is opt-in. Your conversations stay with your staff until you turn it on. [S16]
- The app asks for access to customer details such as name, email, phone, address and IP address, plus your products, orders and customers. [S19]
- A conversation is capped at 100 agent replies for customers who aren't signed in, and 1,000 for those who are. [S17]
- When you rate the agent's replies, Shopify may suggest persona changes. Shopify says "Updates are never applied automatically." [S18]
- You're responsible for the accuracy of what you send customers, including generated text. [S14] [S15]
- The pages don't say whether conversations are used to train models. [S16] [S18]

**In Australia**

- Suggested replies and AI instant-answer suggestions are English only. Suggested replies also need your online store and admin set to English. [S14] [S15]
- Shopify warns that the instant-answer AI's language data "is largely from North American sources", so expect some American wording. [S14]
- The app listing says Inbox supports 21 languages. [S19]

### Campaign Autopilot (early access)

**What it does**

- It creates and manages marketing for your store across Shopify Messaging email, Shop Campaigns, Meta ads and Microsoft Advertising. [S48]
- It recommends actions based on your store's products and sales data, and you approve or reject them. Shopify says "You decide what goes live." [S48]
- Once you approve a tactic, it manages the campaign within your guardrails. Your monthly budget is a target, and spending can go over it because of delayed attribution. [S49]
- It doesn't change your product prices or store settings. [S49]

**Where to find it**

- **Growth** > **Autopilot** in the Shopify admin. [S48]

**Which plans have it**

- Every Shopify subscription plan except Agentic, with Shopify Payments switched on. [S49]
- Autopilot itself is free. You pay for the ads and messages it runs, and Meta and Microsoft bill ad spend directly. [S47] [S49]
- Shopify announced it in early access on 17 June 2026. [S43] [S47]

**What happens to your data**

- It reads your product catalogue, customer segments, purchase and order history, subscriber lists and campaign results. [S49]
- Data sent to Meta or Microsoft for ads comes under their terms once you connect those channels. [S49]
- The page doesn't say whether your data is used for training. [S49]

**In Australia**

- Shopify says channel availability varies by location. Its launch post said Shop Campaigns were for the US and Canada only. [S47]
- The requirements page doesn't mention Australia. [S49]

## Outside AI that connects

Shopify lists official connections for ChatGPT, Claude, Gemini, Grok, Muse, Perplexity and Microsoft Copilot. It says they can answer questions and manage store data such as products, orders and customers. [S2] [S21]

These rules apply to all of them. [S26] [S27]

- You install each one from inside the AI tool. They aren't on the Shopify App Store. The AI tool then sends you to your Shopify admin to approve a data access level. [S26] [S22]
- Read-only access lets the tool view data. Write access lets it edit data and act for you. You can decline. [S26]
- A tool can only get permissions the person connecting already has. Someone who can view products but not edit them can't give the AI edit rights. [S26]
- You connect one store at a time. After switching stores, start a new conversation. [S26]
- You can't lower an approved access level. To reduce access, uninstall and reinstall. [S26]
- To revoke access, uninstall the integration from your Shopify admin. Shopify's page doesn't give the menu path. [S26]
- Even with write access, these tools can't issue refunds, cancel or capture orders, mark orders paid, process returns or manage gift cards. [S27]
- They also can't change your plan, payments, taxes or domains. They can't edit your live theme, or publish or delete a theme, though they can edit an unpublished one. [S27]
- Shopify doesn't review or approve the actions these tools take for you. If a tool makes a wrong change, you're responsible for it. [S27]
- Once you authorise sharing, the data leaves Shopify and the AI company's terms and privacy policy apply. [S26] [S27]

### Claude and Shopify

**Official?**

- Yes. Anthropic's directory lists the Shopify connector as "Made by Shopify", with an "Anthropic verified" badge. It was added in April 2026. [S58]
- Shopify calls it the "Shopify connector for Claude". [S22]
- Shopify is one of the 37 partner connectors in Anthropic's Claude for Small Business, announced 15 September 2026. [S60] [S61]

**What it can see and do**

- In short, it reads and makes changes. Shopify says it asks you to confirm before Admin API changes, and asks you to confirm the start date and who can use a new discount code. [S22]
- It reads products, collections, inventory, orders, customers and analytics. It also reads store details, pages, blogs, menus, metafields, markets and translations. [S22]
- It can create and update products, in batches of up to 50, and turn a file or link into a digital product. [S22]
- It can create and update collections and set stock levels at a location. It can also create percentage-off discount codes. [S22]
- It can build a storefront preview from a business idea and import products from Shopify Collective suppliers. [S22] [S58]
- It can't edit existing discount codes or create fixed-amount ones. Customer records are read-only. [S22]
- Anthropic's listing shows 25 tools, including create-product, set-inventory, create-discount and graphql_mutation. [S58]
- On Claude Team and Enterprise, Owners can set each tool to **Always allow**, **Needs approval** or **Blocked**. [S59]

**What you need**

- A Claude account, and a Shopify store you own or one you create. Shopify charges no extra fee for the connector. Claude subscription costs go to Anthropic. [S22]
- Shopify says to set it up in a desktop browser. [S22]
- On Claude Team and Enterprise, an Owner adds the connector for the organisation first. Each person then signs in separately. [S59]
- Claude for Small Business is on every paid Claude plan. [S60]

**Steps to connect** (Anthropic's help article, updated 17 October 2026; Shopify's help page, no date shown)

1. In Claude, go to **Customize > Connectors** and click **+** next to **Connectors**. Shopify's page also links straight to the install page. [S59] [S22]
2. Click Shopify, then **Connect**. [S59]
3. Claude sends you to your Shopify admin. Read the data access it asks for, then approve it. [S22] [S26]
4. In a chat, click **+** (lower left) or type **/**, hover over **Connectors**, and check Shopify is switched on. [S59]
5. Mention Shopify by name in your request. [S22]

Team and Enterprise Owners first go to **Organization settings > Connectors**, click **Browse connectors**, select the connector and click **Add to your team**. [S59]

**To disconnect**

- In Claude, go to **Customize > Connectors** and disconnect Shopify. [S59]
- In Shopify, uninstall the integration from your admin. [S26]

**Limits**

- Batch changes can stop partway. Finish them in your Shopify admin. [S22]
- A storefront preview isn't a store until you claim it, and it may include sample content. [S22]
- Anthropic's listing gives the connector's address as https://setup.shopify.com/mcp. It warns: "Only use connectors from developers you trust." [S58]
- On Claude's Free, Pro and Max plans, Anthropic uses your chats to improve its models if you opt in, or if a chat is flagged for safety review. Raw content from connectors is left out, though it may be included if it's copied straight into the chat. [S62]
- On Claude's commercial plans, Anthropic says it won't use your inputs or outputs for training by default. [S63]
- Shopify's page says nothing about data, privacy or training. [S22]

### ChatGPT and Shopify

**Official?**

- Yes. Shopify calls it the "Shopify plugin for ChatGPT". [S23]
- OpenAI's directory lists it with Shopify as the developer. We read OpenAI's pages only through search-engine copies. [S64] [S65]

**What it can see and do**

- In short, it reads and makes changes. Shopify says it asks you to confirm before Admin API changes, and product drafts open in a panel you can edit before saving. [S23]
- It can list up to 50 recent orders, with tracking, and look up customers with their order count and spend. It answers sales questions as tables and charts. [S23]
- It can create and update products and collections, add photos to products, set stock levels and create percentage-off discount codes. [S23]
- It can turn a file or link into a digital product. That needs Shopify's Digital Products app. [S23]
- Orders and customer records are read-only. It can't change existing discount codes or create fixed-amount ones. [S23]
- OpenAI's listing says the plugin bundles a Shopify app with skills such as Shopify Admin and Shopify Customer. [S65]

**What you need**

- A ChatGPT account. OpenAI says availability depends on your plan and workspace settings, and some connections need admin approval. [S64]
- Shopify charges no extra fee. ChatGPT subscription costs go to OpenAI. [S23]
- Shopify says to set it up in a desktop browser. [S23]

**Steps to connect** (Shopify's help page and OpenAI's plugin docs, neither dated)

1. In ChatGPT on the web or the desktop app, open the **Plugins** tab and search for Shopify. Shopify's page links to the install page at chatgpt.com/plugins/shopify. [S66] [S23]
2. Open its details and select the plus button to install it. [S66]
3. When asked, connect and sign in. You're sent to your Shopify admin to approve the data access. [S66] [S23]
4. Start a new chat and type **@Shopify** with your request. Without it, ChatGPT may give general instructions instead. [S66] [S23]

**To disconnect**

- Select **Uninstall plugin** where it's offered. OpenAI says the connection stays active until you also disconnect it in ChatGPT. [S66]
- In Shopify, uninstall the integration from your admin. [S26]

**Limits**

- Keep requests to one task at a time, and keep analytics questions short. [S23]
- ChatGPT is operated by OpenAI and isn't managed by Shopify. [S23]
- OpenAI says that when ChatGPT sends data through a plugin's server, that service's terms and privacy policy apply. [S66]
- Shopify's page says nothing about privacy or training. [S23]

**Selling to shoppers in ChatGPT**

- Your products reach ChatGPT through Shopify Catalog, on by default for eligible stores. [S33]
- Shopify calls ChatGPT a "discovery-focused referrer". Shoppers pay on your own store's checkout, which opens inside ChatGPT or in a new tab. [S33]
- Your store must sell to customers in the United States. It can be based elsewhere. [S33]
- Shopify says there are no fees for selling in ChatGPT beyond your normal payment processing. [S33]
- OpenAI says it's moving away from its standalone Instant Checkout towards merchant-owned checkout. It says Shopify merchants need no extra setup. [S67]
- ChatGPT Ads for Shopify is a separate app for advertising. OpenAI's help article, seen only as a search-engine copy, says it's available to Shopify customers in the US. [S68]

### Microsoft Copilot and Shopify

**Official?**

- Shopify documents a "Shopify plugin for Microsoft Copilot", listed in Copilot as "Shopify". It works in Copilot Cowork and Microsoft 365 Copilot Chat. [S24] [S21]
- Microsoft's list of partner plugins for Copilot Cowork, updated 15 October 2026, doesn't include Shopify. Microsoft says the catalogue keeps growing. [S69]
- Shopify isn't one of Microsoft's federated Copilot connectors. [S74]
- A May 2026 Microsoft post names Shopify among the apps Copilot has connectors for. [S75]

**What it can see and do**

- In short, it reads and makes changes. Shopify says it confirms before Admin API changes and asks you to confirm new discount codes. [S24]
- It reads products, collections, inventory, orders, customers, discount codes and analytics. [S24]
- It can create and update products, collections and stock levels. It can also create percentage-off codes and edit unpublished themes. [S24]
- Orders and customer records are read-only. It can't build storefront previews, and it returns text rather than tables or charts. [S24]
- In Copilot Cowork it works alongside the email, documents and spreadsheets you've already shared with Copilot. The Shopify agent in Copilot Chat can't read those. [S24]

**What you need**

- A Shopify store you own. If you don't have one, you can create one from the Shopify sign-in screen. [S24]
- Your organisation's Microsoft 365 settings decide whether an admin deploys the plugin, and your admin controls which plugins you can add. [S24]
- Microsoft says people using Cowork plugins need Microsoft 365 Copilot licences. [S71]
- Shopify doesn't name a Copilot licence or Shopify plan. [S24]

**Steps to connect** (Microsoft's Cowork docs, updated 27 August 2026; Shopify's help page, no date shown)

1. In Copilot Cowork, select **+**, then **Customize**. Search for Shopify and open its details. [S70]
2. Add it. If it isn't listed, ask your IT admin, who controls plugins under **Agents** > **Tools** in the Microsoft 365 admin center. [S70] [S69] [S71]
3. When Copilot first needs your store, sign in to Shopify and approve the access. [S24] [S70]
4. In Copilot Chat, open the Shopify agent from **Agents** and mention Shopify in your requests. Shopify says that without opening the agent, Copilot may only view data. [S24]

For agents in the Microsoft Copilot app generally, Microsoft's steps are **All Agents**, select the agent, then **Add**. If you see **Request approval**, your IT admin has to approve it. [S72]

**To disconnect**

- Shopify says to uninstall the integration from your Shopify admin. Revoking Shopify's access doesn't affect Microsoft 365 access, and the reverse is also true. [S24]
- In Cowork, a plugin you added yourself can be removed from **Customize** with **Remove from Cowork**. Admin-deployed plugins can only be removed by the admin. [S70]

**Limits**

- Installing the plugin doesn't give Shopify access to your Microsoft 365 content. [S24]
- Microsoft says prompts, responses and data accessed through Microsoft Graph aren't used to train foundation models. It tells you to check each agent's own privacy statement and terms. [S73]
- Microsoft says customers outside the EU may have their queries processed in the US, the EU or other regions. [S73]

**Selling to shoppers in Copilot**

- Shopify offers direct checkout in Copilot, where shoppers pay without leaving the chat. It's on by default for eligible stores. [S34]
- Your store must sell to US customers, and direct checkout shows only to customers based in the US. [S34]
- Microsoft announced Copilot Checkout on 8 January 2026 and said Shopify merchants would be enrolled automatically after an opt-out window. [S76]
- Microsoft says only English-language merchants selling to US buyers in US dollars are eligible for now, and it takes no commission today. [S77]
- Microsoft also offers Brand agents, a beta AI shopping assistant for your own website that installs from the Shopify App Store. Accepting its terms publishes your catalogue to Microsoft Merchant Center for Bing and Copilot. [S78]
- Microsoft also lists a "Shopify (Independent Publisher)" connector for Power Automate and Copilot Studio. Its listed publisher is "Ray Bennett (MSFT)", and Shopify isn't named. It's in preview, connects with an access token and can cancel orders, including refunds. [S79]

### Google Gemini and Shopify

**Official?**

- Shopify documents a "Shopify connector for Gemini". [S25]
- Google's availability table lists Shopify for "Personal Google Account only", "18 or over", "US only" and "English only". [S81]
- Google's 13 October 2026 post names Shopify among more than 40 apps Gemini connects to. [S83]

**What it can see and do**

- In short, it reads and makes changes, but only if you approve write access. Without it, the connector only reads. [S25]
- It reads store details, products, orders with shipping addresses and tracking, customers with order count and spend, collections, inventory and analytics. [S25]
- It can create and update products, collections and stock levels, and create percentage-off discount codes. [S25]
- Order and customer records are read-only. [S25]
- Shopify says it asks you to confirm before Admin API changes and before creating a discount code. [S25]

**What you need**

- A Shopify store you own. [S25]
- Under Google's table, a personal Google account, aged 18 or over, in the US, using English. [S81]
- Google's article for work and school accounts doesn't mention Shopify. [S82]

**Steps to connect** (Google's general steps for personal accounts, no date shown)

1. Go to gemini.google.com and click **Customize** in the sidebar. [S80]
2. At the top, click **Connectors**. Find Shopify and click **Add**, then follow the instructions. [S80]
3. You can also type **@** in a chat and choose Shopify. [S80] [S25]
4. Approve the data access in your Shopify admin. [S25]

**To disconnect**

- In Gemini, go to **Customize** > **Connectors**, click **More options** next to Shopify, then **Disconnect**. [S80]
- To switch stores, Shopify says to unlink Shopify in Gemini's connected apps settings, then ask for Shopify again. [S25]

**Selling to shoppers in Google AI Mode and Gemini**

- Shoppers can pay through a Shopify-powered checkout inside AI Mode and the Gemini app. [S35]
- Your store must be based in the United States and sell to US customers, and you need a Google Merchant Center account. [S35]
- Google launched the Universal Commerce Protocol (UCP) on 11 January 2026, co-developed with Shopify, for checkout from eligible US retailers. Google said it would expand globally "in the coming months". [S84]

### Selling to shoppers inside AI chats (agentic storefronts)

**What it is**

- Agentic storefronts let customers find and buy your products inside AI channels. Shopify lists ChatGPT, Google AI Mode and Gemini, Microsoft Copilot, and Meta including a surface called Muse. [S30]
- It's on by default for eligible stores. You keep the customer relationship, and orders show which AI channel they came from. [S30]
- Shopify Catalog needs a store on Starter or higher that isn't in private mode, and products with a title, an image and a price above zero. [S37]
- Some categories are excluded, including alcohol, tobacco and vaping, prescription and medical products, and event tickets. [S37]
- Agentic storefronts support direct-to-consumer sales only. [S36]

**How to control it**

- Go to **Sales channels** > **Agentic**. You need to be the store owner, or have the **Products** > **View** and **App and sales channel** > **Agentic** staff permissions. [S31]
- **Allow Shopify to manage for me** is on by default. It keeps all channels active and enrols you in new AI channels automatically. [S31]
- To change things, turn that setting off, then turn **Shopify Catalog access** or **Auto enroll new storefronts** off, or adjust each channel. Click **Save**. [S31]
- After you turn off Catalog access, it can take up to 7 days for your product data to stop being shared. [S31]
- AI channels can still find your products by crawling the web. [S31] [S32]

**What's shared**

- Product data such as titles, descriptions, images, prices and availability goes through Shopify Catalog. [S32]
- When someone orders through a channel with direct checkout, the customer's name, email, phone number and address are shared. [S32]
- Shopify says your private admin data isn't shared. AI channels don't get your full order history or your general customer database. [S32]
- The Supplemental Terms, last updated 6 October 2026, say the AI channel's own terms govern data it collects directly. They don't mention training. [S39]
- The Supplemental Terms let Shopify charge fees on some channels' transactions, while Shopify's help pages say there are no extra fees for ChatGPT, Copilot or Google. [S39] [S33] [S34] [S35]

### Other AI assistants Shopify lists

- Shopify also has connectors for Grok, Muse and Perplexity. [S21]
- Stores built by AI coding tools such as Lovable, Manus, Replit and v0 can be claimed and finished in Shopify. [S21]
- Shopify publishes a file at shopify.com/SKILL.md for AI tools. It only points them to the official Shopify integrations and doesn't read or change your store itself. [S28]

### Shopify's MCP servers and developer tools

These tools are meant for developers and people building their own AI apps. [S29] [S52]

- The **Shopify CLI connector** lets a developer authorise a coding tool on their own computer, such as Claude Code, Codex, Cursor or Visual Studio Code, to use a store's API. Shopify says it "authorizes API access and nothing more." [S29]
- The **Shopify AI Toolkit** connects coding tools to Shopify's docs and API schemas. Its Dev MCP server runs locally and needs Node.js 18 or later. [S52]
- Shopify's **Storefront Catalog MCP** lets shopping agents search one store's products at that store's /api/ucp/mcp address. It follows the UCP specification version 2026-08-25. [S53]
- Shopify removed the older catalog and cart tools from the /api/mcp address. Its policies and FAQ search tool still works there. [S54]
- A **Global Catalog MCP** at catalog.shopify.com lets agents search across Shopify merchants. [S55]
- Shopify adds **WebMCP** tools to every Liquid storefront, so AI agents in Chromium browsers can search products and fill carts. The page doesn't say whether you can switch them off. [S56]

### Automation tools and Shopify

- Shopify Flow is Shopify's own free automation app on Basic, Grow, Advanced and Plus. Its help page doesn't describe AI features, but Sidekick can create Flow workflows. [S50] [S6]
- Zapier lists an app on the Shopify App Store. Its listing says Shopify requires a paid Zapier plan. [S51]
- We didn't find Shopify documentation for Make or Power Automate. [S2] [S21]

## Jobs it's good for

- **A Monday sales check.** Ask Sidekick or a connected AI how last week's sales went. Shopify says short, specific analytics questions work best. [S3] [S22] [S23]
- **Product descriptions.** Use **Generate text** with a title and at least two features, then edit before saving. [S11]
- **Tidying the range.** A connected AI can set up to 50 products at a time to active, draft or archived. [S22] [S23] [S25]
- **A stocktake.** Ask a connected AI to set stock levels at a location, with a reason such as received or damaged. It reads the current count first. [S25] [S22]
- **A launch discount.** Ask for a percentage-off code, then confirm the start date and who can use it. [S22]
- **Clean product photos.** Swap a busy background for a plain colour in the file editor. [S10]
- **After-hours questions.** Turn on the Inbox agent with staff handoff, and keep an eye on its answers. [S16] [S17]
- **Theme changes without risk to your live shop.** Duplicate the theme, let the AI edit the copy, then publish it yourself. [S27]
- **The weekly plan.** Shopify's VP of Product told Anthropic that with Claude for Small Business, merchants "run their store where they already plan the week". [S60]
- **Shop data next to your spreadsheets.** In Copilot Cowork the Shopify plugin works alongside documents you've already shared with Copilot. [S24]

## What to watch for

**Write access means real changes**

- Approve read-only access unless you need the AI to change things. You can't lower the level later without reinstalling. [S26]
- Connected tools change items one at a time, so big batches can stop partway. [S27]
- Shopify doesn't review what these tools do, and you're responsible for any wrong change. [S27]
- Shopify suggests naming exactly what to change and asking the tool to check with you "before doing anything destructive or hard to undo". [S20]

**The AI sees what the login sees**

- A connected AI acts with the permissions of the staff account that approved it. [S26] [S27]
- Sidekick also works within each staff member's permissions. [S8]
- So an owner's login gives the AI the widest reach. That's our inference from the above.

**Your data leaves Shopify**

- Once shared, data is handled under the AI company's terms, and Shopify no longer controls how it's used or kept. [S27]
- Shopify reminds you that you still owe your customers what privacy law requires. [S27]

**Training and where data goes**

- Shopify's no-training statement for Sidekick is in a blog post. Its terms let it use your materials to improve its services. [S9] [S40]
- Sidekick's AI providers are listed as located in the USA. [S42]
- We found no option to keep Shopify's AI processing in Australia. [S41] [S42]
- Your chats on the AI side follow that company's own settings, such as Claude's **Model Improvement** setting. [S62]

**Selling in AI chats is on by default**

- Eligible stores are opted in, and new AI channels are added automatically unless you change **Auto enroll new storefronts**. [S31]
- Orders through direct checkout share the customer's name and contact details with the AI channel. [S32]

**Much of it is US-only for now**

- Selling in ChatGPT and Copilot needs you to sell to US customers, and Google needs a US-based store. [S33] [S34] [S35]
- The Gemini store connector is listed as US only. [S81]
- OpenAI says ChatGPT Ads for Shopify is available to Shopify customers in the US. [S68]

**Check the work**

- Shopify warns that "AI outputs can contain errors" and that the same request won't always give the same result. [S2] [S20]
- Generated product text can claim benefits you never listed. [S11]
- The Inbox agent talks to customers on your behalf, so test its persona and watch early conversations. [S16] [S17]

**Costs**

- Sidekick's usage limits vary by plan, and Shopify doesn't publish the amounts. [S8] [S6]
- Campaign Autopilot is free, but its ad spend can run over your monthly target. [S49]
- The Agentic Storefronts terms allow Shopify to add transaction fees for some channels. [S39]

**Tools Shopify didn't build**

- Anthropic's listing warns to use connectors only from developers you trust. [S58]
- The Independent Publisher connector in Power Automate uses an access token and can cancel orders. Prefer Shopify's own connections. That's our advice. [S79]

**Beta and early access**

- Campaign Autopilot is in early access. Brand agents is in beta, and Shopify says it's early days for Canvas. [S43] [S44] [S78]

## Announced changes

- **8 January 2026:** Microsoft announced Copilot Checkout, rolling out in the US on Copilot.com, with Shopify merchants enrolled after an opt-out window. [S76]
- **11 January 2026:** Shopify opened Shopify Catalog to every brand and said it co-developed UCP with Google. Google said UCP checkout would "soon" reach AI Mode and the Gemini app for eligible US retailers. [S45] [S84]
- **24 March 2026:** Shopify said it had rolled out the Agentic plan globally, and that Shop Pay was "coming soon" to Copilot. [S46]
- **April 2026:** The Shopify connector was added to Claude's directory. [S58]
- **17 June 2026 (Spring '26 Edition):** Sidekick App Extensions, Sidekick Pulse, an AI sales associate in Inbox, and Campaign Autopilot in early access. [S43]
- At the same time Shopify said ChatGPT Ads and Snapchat were coming to Campaign Autopilot, and developers would "soon" earn revenue from Catalog-powered experiences. [S43]
- **15 September 2026:** Anthropic launched Claude for Small Business with Shopify among its partner connectors. [S60]
- **1 October 2026:** Canvas began rolling out. [S44]
- **6 October 2026:** The Agentic Storefronts Supplemental Terms were updated. [S39]
- **13 October 2026:** Sidekick can now customise checkout and customer account settings. [S8]
- **13 October 2026:** Google said Gemini connects to more than 40 apps, including Shopify. [S83]

## What we couldn't establish

- **Whether the Copilot plugin is live.** Shopify documents it, but Microsoft's Cowork plugin list of 15 October 2026 doesn't include it and we found no Microsoft listing. [S24] [S69]
- **What "Millions of tokens" means** on the pricing page, and what happens when you run out. [S1] [S8]
- **Whether prices include GST.** The Australian pricing page doesn't say. [S1]
- **Yearly prices.** One automated read of the pricing page showed lower yearly prices ($42, $114 and $431). Two direct reads of the page showed $50, $134 and $519, which is what we've used. Check the live page before quoting. [S1]
- **Training in writing.** Shopify's "never used to train foundation models" line is in a blog post. We didn't find it in Shopify's terms or privacy policy. [S9] [S40] [S41]
- **OpenAI's pages.** OpenAI's Shopify listing, its product discovery post and its help article blocked automated reading, so we relied on search-engine copies. [S64] [S65] [S67] [S68]
- **Which AI plans the connectors need.** Shopify's pages don't name Claude, ChatGPT or Microsoft plans. [S22] [S23] [S24]
- **The revoke path in Shopify.** Shopify says to uninstall the integration but doesn't give the menu steps. [S26]
- **Whether AI channels may train on Catalog data.** Neither the help pages nor the Supplemental Terms say. [S32] [S39]
- **The Agentic plan in Australia.** Its help page doesn't list countries, though Shopify says it rolled out globally and it's on the Australian pricing page. [S38] [S46] [S1]
- **Channel fees.** The Supplemental Terms allow fees, but the channel pages say there are none. [S39] [S33]
- **Inbox agent languages.** The help pages don't say. The app listing says 21 languages, but suggested replies are English only. [S16] [S19] [S15]
- **A store-wide Sidekick switch.** None found. [S3] [S8]
- **Shopify Magic.** We found no formal notice of the change of name. The help centre now uses "AI-powered tools". [S2]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | Shopify pricing (Australia) | Shopify | https://www.shopify.com/au/pricing | No date shown (a footnote is dated 15 Oct 2026) | 17 Oct 2026 |
| S2 | AI-powered tools | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools | No date shown | 17 Oct 2026 |
| S3 | Sidekick | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/sidekick | No date shown | 17 Oct 2026 |
| S4 | Getting started with Sidekick | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/sidekick/set-up | No date shown | 17 Oct 2026 |
| S5 | Sidekick memory and personalization | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/sidekick/memory | No date shown | 17 Oct 2026 |
| S6 | Generating content with Sidekick | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/sidekick/generate-content | No date shown | 17 Oct 2026 |
| S7 | Generating apps with Sidekick | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/sidekick/generate-apps | No date shown | 17 Oct 2026 |
| S8 | Sidekick | Shopify | https://www.shopify.com/sidekick | No date shown; update entries dated 6 Jan, 10 Feb and 13 Oct 2026 | 17 Oct 2026 |
| S9 | How Enterprise Teams are Using Sidekick to Drive Real Value Right Now | Shopify (Enterprise blog) | https://www.shopify.com/enterprise/blog/sidekick-ai-enterprise | 5 Jun 2026 | 17 Oct 2026 |
| S10 | Media generation in the file editor | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/media-generation | No date shown | 17 Oct 2026 |
| S11 | Automatically generating product descriptions | Shopify Help Center | https://help.shopify.com/en/manual/products/details/product-descriptions/generate | No date shown | 17 Oct 2026 |
| S12 | Adding, previewing, and buying themes | Shopify Help Center | https://help.shopify.com/en/manual/online-store/themes/adding-themes | No date shown | 17 Oct 2026 |
| S13 | Tinker by Shopify | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/tinker | No date shown | 17 Oct 2026 |
| S14 | Set up instant answers for Shopify Inbox | Shopify Help Center | https://help.shopify.com/en/manual/inbox/chat-settings-and-appearance/instant-answers | No date shown | 17 Oct 2026 |
| S15 | AI-generated suggested replies in Shopify Inbox | Shopify Help Center | https://help.shopify.com/en/manual/inbox/chat-settings-and-appearance/suggested-replies | No date shown | 17 Oct 2026 |
| S16 | Shopify Inbox | Shopify Help Center | https://help.shopify.com/en/manual/inbox | No date shown | 17 Oct 2026 |
| S17 | Configuring your Inbox agent persona | Shopify Help Center | https://help.shopify.com/en/manual/inbox/agent-persona | No date shown | 17 Oct 2026 |
| S18 | Training your Inbox agent | Shopify Help Center | https://help.shopify.com/en/manual/inbox/training-your-agent | No date shown | 17 Oct 2026 |
| S19 | Shopify Inbox (app listing) | Shopify App Store | https://apps.shopify.com/inbox | No update date shown; launched 14 Aug 2019 | 17 Oct 2026 |
| S20 | Best practices for using AI-powered tools | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/best-practices | No date shown | 17 Oct 2026 |
| S21 | Building and managing your store with third-party AI tools | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools | No date shown | 17 Oct 2026 |
| S22 | Shopify connector for Claude | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/shopify-connector-for-claude | No date shown | 17 Oct 2026 |
| S23 | Shopify plugin for ChatGPT | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/shopify-plugin-for-chatgpt | No date shown | 17 Oct 2026 |
| S24 | Shopify plugin for Microsoft Copilot | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/shopify-plugin-for-microsoft-copilot | No date shown | 17 Oct 2026 |
| S25 | Shopify connector for Gemini | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/shopify-connector-for-gemini | No date shown | 17 Oct 2026 |
| S26 | Authorizing AI tool access to your store | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/authorizing-access | No date shown | 17 Oct 2026 |
| S27 | Considerations for using third-party AI tools with your Shopify store | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/considerations | No date shown | 17 Oct 2026 |
| S28 | Shopify skill.md for AI tools | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/connecting-ai-tools/shopify-skill-md | No date shown | 17 Oct 2026 |
| S29 | Shopify CLI connector | Shopify Help Center | https://help.shopify.com/en/manual/ai-powered-tools/shopify-cli-connector | No date shown | 17 Oct 2026 |
| S30 | Shopify agentic storefronts | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts | No date shown | 17 Oct 2026 |
| S31 | Managing agentic storefronts | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/agentic-home | No date shown | 17 Oct 2026 |
| S32 | Data sharing and privacy for selling with agentic storefronts | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/data-privacy | No date shown | 17 Oct 2026 |
| S33 | Selling on ChatGPT | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/chatgpt | No date shown | 17 Oct 2026 |
| S34 | Selling on Microsoft Copilot | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/microsoft | No date shown | 17 Oct 2026 |
| S35 | Selling on Google AI Mode and Gemini | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/google | No date shown | 17 Oct 2026 |
| S36 | Shopify Catalog and product discovery for agentic storefronts | Shopify Help Center | https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/products | No date shown | 17 Oct 2026 |
| S37 | Requirements for being included in Shopify Catalog | Shopify Help Center | https://help.shopify.com/en/manual/shopify-catalog/requirements | No date shown | 17 Oct 2026 |
| S38 | Agentic plan | Shopify Help Center | https://help.shopify.com/en/manual/intro-to-shopify/pricing-plans/plans-features/shopify-agentic-plan | No date shown | 17 Oct 2026 |
| S39 | Shopify Agentic Storefronts Supplemental Terms of Service | Shopify | https://www.shopify.com/legal/terms-agentic-storefronts | Last updated 6 Oct 2026 | 17 Oct 2026 |
| S40 | Shopify Terms of Service | Shopify | https://www.shopify.com/legal/terms | Last updated 1 Aug 2026 | 17 Oct 2026 |
| S41 | Shopify Privacy Policy | Shopify | https://www.shopify.com/legal/privacy | Updated 7 Jul 2026 | 17 Oct 2026 |
| S42 | Subprocessors | Shopify Help Center | https://help.shopify.com/en/manual/privacy-and-security/privacy/subprocessors | No date shown | 17 Oct 2026 |
| S43 | Selling everything, everywhere, all at once: The Spring '26 Edition | Shopify News | https://www.shopify.com/news/spring-26-edition-merchant | 17 Jun 2026 | 17 Oct 2026 |
| S44 | Introducing Canvas: Opening the aperture on online store design | Shopify News | https://www.shopify.com/news/introducing-canvas | 1 Oct 2026 | 17 Oct 2026 |
| S45 | The agentic commerce platform: Shopify connects any merchant to every AI conversation | Shopify News | https://www.shopify.com/news/ai-commerce-at-scale | 11 Jan 2026 | 17 Oct 2026 |
| S46 | Millions of merchants can sell in AI chats | Shopify News | https://www.shopify.com/news/agentic-commerce-momentum | 24 Mar 2026 | 17 Oct 2026 |
| S47 | Introducing Campaign Autopilot | Shopify Blog | https://www.shopify.com/blog/introducing-campaign-autopilot | 17 Jun 2026 | 17 Oct 2026 |
| S48 | Automating your marketing with Campaign Autopilot | Shopify Help Center | https://help.shopify.com/en/manual/promoting-marketing/autopilot | No date shown | 17 Oct 2026 |
| S49 | Requirements and considerations for using Campaign Autopilot | Shopify Help Center | https://help.shopify.com/en/manual/promoting-marketing/autopilot/requirements-and-considerations | No date shown | 17 Oct 2026 |
| S50 | Shopify Flow | Shopify Help Center | https://help.shopify.com/en/manual/shopify-flow | No date shown | 17 Oct 2026 |
| S51 | Zapier: Workflow Automation (app listing) | Shopify App Store | https://apps.shopify.com/zapier | No update date shown; launched 26 Apr 2012 | 17 Oct 2026 |
| S52 | Shopify AI Toolkit | Shopify (shopify.dev) | https://shopify.dev/docs/apps/build/ai-toolkit | No date shown | 17 Oct 2026 |
| S53 | Storefront Catalog MCP | Shopify (shopify.dev) | https://shopify.dev/docs/agents/catalog/storefront-catalog | No date shown (cites UCP version 2026-08-25) | 17 Oct 2026 |
| S54 | Migrate from Storefront MCP | Shopify (shopify.dev) | https://shopify.dev/docs/apps/build/storefront-mcp | No date shown | 17 Oct 2026 |
| S55 | Global Catalog MCP | Shopify (shopify.dev) | https://shopify.dev/docs/agents/catalog/mcp | No date shown | 17 Oct 2026 |
| S56 | WebMCP tools | Shopify (shopify.dev) | https://shopify.dev/docs/api/web-mcp | No date shown | 17 Oct 2026 |
| S57 | Sidekick app extensions | Shopify (shopify.dev) | https://shopify.dev/docs/apps/build/sidekick | No date shown | 17 Oct 2026 |
| S58 | Shopify connector | Anthropic (Claude directory) | https://claude.com/connectors/shopify | "Added April 2026" | 17 Oct 2026 |
| S59 | Use connectors to extend Claude's capabilities | Anthropic Help Center | https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities | "Updated today" (17 Oct 2026) | 17 Oct 2026 |
| S60 | Claude for Small Business launches new workflows, integrations, and training programs | Anthropic | https://claude.com/resources/articles/claude-for-small-business-launches-new-workflows-integrations-and-training-programs | 15 Sep 2026 | 17 Oct 2026 |
| S61 | Small Business plugin | Anthropic | https://claude.com/marketplace/plugins/small-business | No date shown | 17 Oct 2026 |
| S62 | Is my data used for model training? (consumer products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | 16 Mar 2026 | 17 Oct 2026 |
| S63 | Is my data used for model training? (commercial products) | Anthropic Privacy Center | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | 18 Aug 2026 | 17 Oct 2026 |
| S64 | Shopify plugin for ChatGPT | OpenAI | https://openai.com/business/plugins/shopify/ | Page blocked automated reading; text seen only as a search-engine copy | 17 Oct 2026 |
| S65 | ChatGPT plugin listing: Shopify | OpenAI | https://chatgpt.com/plugins/plugin_asdk_app_69e65c430b3081919aa4d962ab5d1698 | Page blocked automated reading; text seen only as a search-engine copy (version 4.1.2) | 17 Oct 2026 |
| S66 | Plugins | OpenAI (ChatGPT docs) | https://learn.chatgpt.com/docs/plugins | No date shown | 17 Oct 2026 |
| S67 | Powering Product Discovery in ChatGPT | OpenAI | https://openai.com/index/powering-product-discovery-in-chatgpt/ | Page blocked automated reading; text seen only as a search-engine copy | 17 Oct 2026 |
| S68 | Set up ChatGPT Ads for Shopify | OpenAI Help Center | https://help.openai.com/en/articles/20001523-set-up-chatgpt-ads-for-shopify | Page blocked automated reading; text seen only as a search-engine copy | 17 Oct 2026 |
| S69 | Available plugins for Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-available-plugins | ms.date 15 Oct 2026 | 17 Oct 2026 |
| S70 | Use plugins with Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugins | ms.date 27 Aug 2026 | 17 Oct 2026 |
| S71 | Manage plugins for Copilot Cowork | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-manage-plugins | ms.date 31 Aug 2026 | 17 Oct 2026 |
| S72 | Get more agents in the Microsoft 365 Copilot app | Microsoft Support | https://support.microsoft.com/en-us/topic/get-more-agents-in-the-microsoft-365-copilot-app-5986a0fb-ed6c-4eb7-82c0-e91e105276fb | No date shown | 17 Oct 2026 |
| S73 | Data, Privacy, and Security for Microsoft Copilot | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy | ms.date 9 Jul 2026 (page metadata updated 8 Oct 2026) | 17 Oct 2026 |
| S74 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | ms.date 30 Sep 2026 (page metadata updated 16 Oct 2026) | 17 Oct 2026 |
| S75 | Introducing Microsoft 365 Business with Copilot: The new standard for small business | Microsoft (Copilot blog) | https://www.microsoft.com/en-us/copilot/blog/2026/05/28/introducing-microsoft-365-business-with-copilot-the-new-standard-for-small-business/ | 28 May 2026 | 17 Oct 2026 |
| S76 | Conversations that Convert: Copilot Checkout and Brand Agents | Microsoft Advertising | https://about.ads.microsoft.com/en/blog/post/january-2026/conversations-that-convert-copilot-checkout-and-brand-agents | 8 Jan 2026 | 17 Oct 2026 |
| S77 | Agentic Commerce | Microsoft Advertising | https://about.ads.microsoft.com/en/solutions/technology/agentic-commerce | No date shown | 17 Oct 2026 |
| S78 | Brand agents Overview | Microsoft Learn (Clarity) | https://learn.microsoft.com/en-us/clarity/brand-agents/brand-agents-overview | ms.date 16 Jul 2026 | 17 Oct 2026 |
| S79 | Shopify (Independent Publisher) (Preview) | Microsoft Learn (connectors) | https://learn.microsoft.com/en-us/connectors/shopifyip/ | ms.date 1 Mar 2024 (page metadata updated 25 Apr 2025) | 17 Oct 2026 |
| S80 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S81 | Check the availability and requirements of connected apps in Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/table/17434654?hl=en | No date shown | 17 Oct 2026 |
| S82 | Use apps connected to Gemini with a work or school Google Account | Google Gemini Apps Help | https://support.google.com/gemini/answer/14959807?hl=en | No date shown | 17 Oct 2026 |
| S83 | Gemini 4 Argon is now available in the Gemini app | Google (The Keyword) | https://blog.google/innovation-and-ai/products/gemini-app/gemini-4-argon-availability/ | 13 Oct 2026 | 17 Oct 2026 |
| S84 | New tech and tools for retailers to succeed in an agentic shopping era | Google (The Keyword) | https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/ | 11 Jan 2026 | 17 Oct 2026 |
