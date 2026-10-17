# SEQTA: the AI inside it, and the AI that connects to it

Researched 17 October 2026 from vendor documentation. Every line is tagged with its source.

## The short version

- SEQTA is a learning management system for schools. Staff use SEQTA Teach. Students and parents have their own portals and apps, called SEQTA Learn and SEQTA Engage. [S1] [S6]
- SEQTA was made by Education Horizons, which "became part of Tes in 2025". SEQTA's web pages and help centre now sit with Tes. [S2] [S1] [S20]
- Its built-in AI is SEQTA AI Assist. It drafts lesson plans for teachers, and it sums up the feedback each student has received. [S5]
- Tes says AI Assist comes with a standard SEQTA subscription at no extra cost. A school administrator switches each part on or off. [S5] [S7]
- Tes says lesson-plan drafting sends no personally identifiable information to the AI. It tells teachers never to type any into the AI fields. [S5]
- The feedback summaries draw on six months of teacher feedback about each student. Students see them in SEQTA Learn, and Tes says parents see them in SEQTA Engage. [S7] [S4]
- We found no official SEQTA connection for ChatGPT, Claude, Microsoft Copilot or Google Gemini, and no SEQTA listing in any of their directories. [S27] [S28] [S29] [S32]
- Tes's own suggestion is to use AI tools alongside SEQTA with publicly available curriculum content, "without any need to share a school's protected data". [S25]
- Tes doesn't name the AI model behind AI Assist or say where it runs. Its Australian terms say school data "may be hosted or otherwise accessed outside of Australia, including in the United Kingdom". [S5] [S23]

## The tool, and the plans that matter

Tes describes SEQTA as "the all-in-one learning management system for progressive schools", joining up student learning, wellbeing and attendance. [S2]

- Tes says Education Horizons "became part of Tes in 2025". The same page lists Synergetic, a school management system, alongside SEQTA. [S2]
- Tes is a UK company, Tes Global Limited, with an Australian office in Sydney. [S21]
- We found no SEQTA prices. The SEQTA page offers a demo instead. [S1]
- SEQTA's help centre has start-of-year checklists written for WA Department of Education schools and for Catholic Education WA schools. [S18] [S19]

The parts of SEQTA, and where AI shows up:

| Part | Who uses it | AI in it | Cost of the AI |
|---|---|---|---|
| SEQTA Teach | Teachers and staff | AI Assist for Lesson Planning, on the Planner page | Included in the SEQTA Teach subscription |
| SEQTA Learn | Students (portal and app) | Summarised Assessment Feedback on the dashboard | Included |
| SEQTA Engage | Parents and carers (portal and app) | Summarised Assessment Feedback, according to Tes's blog | Included |
| SEQTA Analyse | Staff and school leaders | Dashboards. No AI described. | Not applicable |
| SEQTA Tutor and SEQTA Kiosk | Staff and students | Extra-curricular records, and signing in and out. No AI described. | Not applicable |

Sources for the table: [S1] [S3] [S4] [S6] [S7]

- **Where it runs.** Schools can use SEQTA Cloud, which Tes hosts on Amazon Web Services (AWS). [S11]
- Schools can also run SEQTA on their own servers or in their own cloud account, where Tes recommends AWS or Azure. [S13]
- Tes says SEQTA supports single sign-on, role-based access and auditing. [S1] [S10] [S12]

## AI built in

### SEQTA AI Assist for Lesson Planning

**What it does**

- Drafts a plan for one lesson. The teacher reviews and edits it before saving. [S6]
- Tes says the draft comes "complete with lesson titles, materials needed, learning objectives and differentiated learning ideas". [S3]
- It fills in the subject, the Essential Learning and the syllabus links from the programme where they exist. The teacher sets the year level and the lesson length, which defaults to 50 minutes. [S6]
- The teacher can add Additional Details, such as "Include a group activity". [S6]
- It uses Australian Curriculum version 9 subcodes automatically. For other curricula, Tes suggests pasting the outcome's wording into Additional Details. Its examples come from the NSW K-10 curriculum and WACE 2024. [S6]
- The draft opens in the Lesson Editor. Tes's help says "AI might produce inaccurate results." [S6]

**Where to find it**

- In SEQTA Teach, on the **Planner** page. Choose **Start with AI**, or **Go Manual** to plan without it. [S6]
- Fill in the details and click **Draft lesson plan**. **Draft a new lesson plan** throws away the current draft. [S6]
- It isn't available for programmes that aren't attached to a class. [S6]

**Which plans have it**

- "SEQTA AI Assist is available to all schools as part of their standard subscription to SEQTA", and using it "does not incur an additional cost". [S5]
- Tes's blog says it's included in the SEQTA Teach subscription. [S3]

**What happens to your data**

- Tes says AI Assist "does not communicate any PII (Personally Identifiable Information) with the AI components that draft the lesson plans". [S5]
- Tes's blog says "No details regarding students, teachers or the school are available to SEQTA AI Assist", and that the AI components "cannot access or read any data inside SEQTA". [S3]
- Never put personal details in the Essential Learning or Additional Details fields. [S5]
- AI Assist runs through a Tes service at ai.seqta.com, which Tes lists as an AWS load balancer. [S8]
- Tes doesn't name the AI model, say where it runs, or say whether what teachers type is used to train it. For more, it points to its General Terms of Business, Data Processing Agreement and Privacy Notice. [S5]
- **Admin switch.** Go to **Administration workspace > Application Settings > Application settings** and search for "AI assist". You need the **DATA: EDIT** permission. Once it's on, everyone with permission to edit programmes can use it. A school can switch it off at any time. [S5]

**In Australia**

- It's built around the Australian Curriculum, version 9. [S6]
- Tes plans to add all Australian Curriculum versions and state-level curricula "as soon after first release as possible". [S6]

### SEQTA AI Assist: Summarised Assessment Feedback

**What it does**

- Tes calls it "an AI powered addition to SEQTA designed to aid students in assimilating teacher feedback". [S7]
- It gathers each student's feedback from the last 6 months, across all subjects, and sums it up in at most 10 bullet points. The most frequent themes come first. [S7]
- The summary changes as teachers add new feedback. [S7]

**Where to find it**

- On the student's dashboard in SEQTA Learn. [S7]
- Tes's help lists the feature as "Summarised Assessment Feedback for students and parents". Its blog says it's "live and accessible to parents through SEQTA Engage". [S5] [S4]

**Which plans have it**

- "SEQTA AI Summarised Assessment Feedback is included as part of your SEQTA subscription." [S4]

**What happens to your data**

- This feature works from the feedback teachers wrote about each student. Tes's no-PII statement covers lesson-plan drafting, and the feedback article doesn't say what's sent to the AI. [S5] [S7]
- Tes's blog says only authorised users, "such as teachers and parents", can see the feedback. [S4]
- **Admin switch.** In **Dashboard Management** (you need **DASH: EDIT**), choose **Available**, **Required** or **Unavailable**. Students can hide the summary when it's Available, can't when it's Required, and no summary is created when it's Unavailable. [S7]
- Once it's on, every student with SEQTA Learn access is included. It can't be limited to certain teachers, and the 6-month window is fixed. [S7]

**In Australia**

- Tes describes it on its Australian blog. [S4]

## Outside AI that connects

We checked each AI maker's directory on 17 October 2026 and found no SEQTA connector. SEQTA's public help centre had no articles on ChatGPT, Claude, Copilot, Gemini or MCP. [S27] [S28] [S29] [S32] [S20]

- We found no SEQTA MCP server and no public API documentation. MCP (Model Context Protocol) is the standard most AI connectors now use. [S20]
- Tes's integration page says SEQTA works with "a wide array of educational tools and platforms", but names no AI assistant. [S12]
- Tes's own suggestion is that generative AI "can be used alongside existing learning management systems – without the need for complex technical integrations". [S25]
- Tes says teachers can draft plans from "publicly available curriculum content, without any need to share a school's protected data". [S25]

### Claude and SEQTA

**Official?**

- No official connection found. Anthropic's directory list on 17 October 2026 had no SEQTA connector. [S27]

**What it can see and do**

- Nothing in SEQTA. There's no documented route for Claude to read SEQTA data. [S27] [S20]

**What you need, steps, disconnecting**

- Not applicable. Tes suggests using AI tools alongside SEQTA's planning tools, working from public curriculum content. [S25]

**Limits**

- Tes's guidance for school AI policies lists "uploading Personally Identifiable Information [PII]" as a prohibited use. [S26]

### ChatGPT and SEQTA

**Official?**

- No official connection found. OpenAI's public plugin pages list no SEQTA plugin. [S28]
- Tes's blog uses ChatGPT as its example of a generative AI tool that can streamline teacher planning. [S25]

**What it can see and do**

- Nothing in SEQTA. [S28]

**What you need, steps, disconnecting**

- Not applicable. The same public-content approach applies. [S25]

**Limits**

- The same policy advice applies: keep personally identifiable information out. [S26]

### Microsoft Copilot and SEQTA

**Official?**

- No official connection found. Microsoft's federated connector list, its partner connector gallery and a Microsoft Marketplace search for "seqta" show no SEQTA listing. [S29] [S30] [S31]

**What it can see and do**

- Nothing documented. [S29]
- SEQTA links to Microsoft 365 in other ways. It can create a Microsoft Teams team for each class and keep the members in step with SEQTA enrolments. "Data travels from SEQTA to MS Teams, but not back to SEQTA." [S15]
- Staff and students can also attach OneDrive files in SEQTA. [S16]
- Tes doesn't describe either link as AI. Copilot inside your school's Microsoft 365 is covered in our separate Microsoft 365 guide. [S15] [S16]

### Google Gemini and SEQTA

**Official?**

- No official connection found. Gemini's connected apps list names no SEQTA app. [S32]
- Gemini's custom apps, which can reach other services, are for people 18 and over in the US. Google says "For now, this feature isn't available if you sign in with a work or school Google Account." [S33]

**What it can see and do**

- Nothing documented. [S32]
- SEQTA's Google Drive integration lets people attach Drive files in SEQTA. Tes doesn't describe it as AI. Gemini inside your school's Google Workspace is covered in our separate Google Workspace guide. [S17]

### SEQTA's own data route: the Cloud Database Backup Service

**Official?**

- We found no public SEQTA API documentation. [S20]
- For SEQTA Cloud schools, Tes offers a daily database backup that "has been introduced to replace direct database access". [S14]

**What it can see and do**

- The backup includes student records, attendance, wellbeing, academic results, marks and grades, and timetable data. [S14]
- It leaves out credentials, system settings, direct messages, forum posts, notifications and correspondence logs. [S14]
- Tes says: "Unlike the SEQTA user interface, which may apply role-based permissions and visibility restrictions, the backup provides access to the full set of included data". [S14]
- It's a daily copy. Tes says it "is not intended for use cases that require near real-time access to information". [S14]

**What you need**

- SEQTA Cloud hosting, the right SEQTA administrator permissions, and Tes switching the feature on for your school. [S14]
- Somewhere secure to keep it. Backups are always encrypted, and Tes says the school is responsible for them once downloaded. [S14]

**Steps to connect** (Tes help article, updated 4 September 2026)

1. Ask Tes to enable the Database Backup Service for your school. [S14]
2. In SEQTA, go to **Administration Settings**, open **Database Backup Settings**, turn on **Enable Database Backups** and save. [S14]
3. After the next daily backup, an authorised administrator uses an API to download the file. [S14]

**To disconnect**

- Not described in the service article. [S14]

**Limits**

- Tes runs the schedule. You can't change the time or frequency. [S14]
- Our reading: if a school feeds this backup into an AI tool, SEQTA's role-based permissions don't come with it. Anyone who can query that tool could reach all of the data. [S14]

### Zapier, Make and Power Automate

- Tes doesn't document any of them for SEQTA. Searches of SEQTA's help centre found no articles about them. [S20]

## Jobs it's good for

- **A first draft of tomorrow's lesson.** Pick the curriculum links, set the year level and click **Draft lesson plan**. Then edit it in the Lesson Editor. [S6]
- **Lessons for WACE or NSW courses.** Paste the outcome's description into Additional Details. Tes's examples include a WACE Accounting and Finance outcome. [S6]
- **Differentiation ideas.** Each draft includes differentiated learning ideas you can adapt. [S3]
- **Consistent planning across a department.** AI Assist plans sit in SEQTA, so heads of department can review them. [S3]
- **Helping students act on feedback.** The summary pulls six months of feedback across all subjects into at most ten points. [S7]
- **Parent conversations.** Parents can see the same summary in SEQTA Engage. [S4]
- **Planning with an outside AI tool.** Draft from public curriculum content and keep school data out of it, as Tes suggests. [S25]

## What to watch for

**Keep personal details out of the AI fields**

- Tes says to "never include any PII" in the AI Assist fields, such as Essential Learning or Additional Details. [S5]
- Tes's AI policy guidance lists uploading personally identifiable information as a prohibited use. [S26]

**Check every draft**

- Tes says generative AI "can supply inaccurate information". [S5]
- It warns that links or videos the AI suggests "may not be relevant nor appropriate for your students". [S5]

**Feedback summaries are about real students**

- Once the feature is on, every student with SEQTA Learn access is included, and summaries cover all subjects. [S7]
- Tes's own policy guidance puts "feedback drafting, data summary" among the uses that need explicit human oversight. [S26]
- Tes doesn't say which student details reach the AI when it writes these summaries. [S7]

**Where the data sits**

- Tes hosts SEQTA Cloud on AWS. [S11]
- Tes's Australian terms say school data "may be hosted or otherwise accessed outside of Australia, including in the United Kingdom". [S23]
- Tes's privacy notice says personal information will, "where possible", be stored in the UK, the EEA or Australia. [S21]
- Tes's sub-processor list gives AWS hosting locations as "EEA, UK & USA", and names no AI model provider. [S24]
- Tes's Data Processing Agreement says it "will not transfer or authorise personal data to be transferred to a different territory without written consent from the customer". [S22]
- These statements don't line up neatly. Our advice: ask Tes where your school's data and AI requests are processed.

**Locked-down networks**

- AI Assist needs the address ai.seqta.com. Schools that block outbound connections should ask their IT team to allow it. [S5] [S8]
- Tes provides a test address, https://ai.seqta.com/connect, which shows "OK" when the connection works. [S5]

**Who switches what**

- Lesson planning: a SEQTA administrator with **DATA: EDIT**, in Application settings. [S5]
- Feedback summaries: a SEQTA administrator with **DASH: EDIT**, in Dashboard Management. [S7]
- Students can hide their summary when it's set to **Available**. [S7]

**Outside AI tools**

- With no official connection, using an outside AI tool with SEQTA means copying information out by hand. Tes's advice is to stick to public curriculum content. [S25]
- The database backup gives the full included data without SEQTA's role-based limits. Treat any AI project built on it as a privacy project. That's our reading. [S14]

## Announced changes

- **2025:** Education Horizons became part of Tes. [S2]
- **17 June 2026:** SEQTA release v2026.6.2 fixed an error that stopped AI lesson plans being generated. [S9]
- **4 September 2026:** Tes's help article on the Cloud Database Backup Service, which replaces direct database access for SEQTA Cloud schools, was last updated. [S14]
- **Planned, no date:** AI Assist support for all Australian Curriculum versions and state-level curricula, and for programmes not attached to a class. [S6]
- **Planned, no date:** Tes says it will "keep exploring and adding new capability to SEQTA AI Assist". [S3]
- **Planned, no date:** Tes says SEQTA Cloud "lays the foundation for the future of SEQTA as part of Tes360". [S11]
- **Parents and summaries:** one line in Tes's help article marks parents as "(coming soon)", while its blog says the feature is live in SEQTA Engage. [S7] [S4]

## What we couldn't establish

- **The AI model** behind AI Assist, and who supplies it. Tes's sub-processor list names no AI provider. [S5] [S24]
- **Where AI requests are processed.** Tes lists ai.seqta.com as an AWS load balancer but names no region. [S8]
- **Training.** We found no statement on whether lesson details or student feedback sent to the AI are used to train models. [S5] [S23]
- **What the feedback summaries send to the AI**, including whether student names go with it. [S7]
- **When AI Assist launched.** Tes's pages don't date it. Image file names in its help articles suggest mid to late 2024. That's our inference. [S5] [S7]
- **Whether AI Assist starts switched off.** Tes describes schools enabling it, but no page says it's off by default. [S5] [S3]
- **Usage limits.** Tes's backup article mentions an internal table for "AI credit tracking", and no page explains AI credits. [S14]
- **Hosting.** Tes's statements on where SEQTA data is stored and processed don't agree (see "Where the data sits"). [S11] [S21] [S23] [S24]
- **SEQTA prices.** [S1]
- **How many schools use SEQTA.** Tes's SEQTA pages give no figure. [S1]
- **Whether Tes 360 will bring AI connections.** [S11]
- **A public API.** We found none in SEQTA's public help centre. [S20]
- **Help centre dates.** Tes's help centre shows "Modified on" dates without a year. We read them as 2026 because the weekdays shown match 2026. [S5]
- **SEQTA's security and privacy page** describes encryption, audits and compliance in general terms, without naming certifications. [S10]

## Sources

All sources were read on 17 October 2026.

| # | Title | Publisher | URL | Updated (as shown) | Read |
|---|---|---|---|---|---|
| S1 | SEQTA: School learning management system | Tes | https://www.tes.com/en-au/for-schools/seqta | No date shown | 17 Oct 2026 |
| S2 | Education Horizons is now part of Tes | Tes | https://www.tes.com/for-schools/now-tes/education-horizons | No date shown | 17 Oct 2026 |
| S3 | Revolutionising lesson planning with SEQTA AI Assist | Tes (blog) | https://www.tes.com/en-au/for-schools/blog/article/revolutionising-lesson-planning-seqta-ai-assist | No date shown | 17 Oct 2026 |
| S4 | SEQTA's AI-powered summarised assessment feedback | Tes (blog) | https://www.tes.com/en-au/for-schools/blog/article/seqtas-ai-powered-summarised-assessment-feedback | No date shown | 17 Oct 2026 |
| S5 | SEQTA AI Assist | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000142584-seqta-ai-assist | "Modified on Fri, 18 Sep" (2026) | 17 Oct 2026 |
| S6 | SEQTA AI Assist for Lesson Planning | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141704-seqta-ai-assist-for-lesson-planning | "Modified on Thu, 2 Apr" (2026) | 17 Oct 2026 |
| S7 | SEQTA AI Assist: Summarised Assessment Feedback | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141702-seqta-ai-assist-summarised-assessment-feedback | "Modified on Thu, 2 Apr" (2026) | 17 Oct 2026 |
| S8 | SEQTA Required External Hostnames and Network Access | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000151163-seqta-required-external-hostnames-and-network-access | "Modified on Wed, 26 Aug" (2026) | 17 Oct 2026 |
| S9 | SEQTA Suite v2026.6.2 (release notes) | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000150315-seqta-suite-v2026-6-2 | "Modified on Wed, 17 Jun" (2026) | 17 Oct 2026 |
| S10 | Security and privacy (SEQTA) | Tes | https://www.tes.com/en-au/for-schools/seqta/security-and-privacy | No date shown | 17 Oct 2026 |
| S11 | SEQTA Cloud | Tes | https://www.tes.com/en-au/for-schools/seqta/cloud | No date shown | 17 Oct 2026 |
| S12 | Integration and compatibility (SEQTA) | Tes | https://www.tes.com/for-schools/seqta/integration-compatibility | No date shown | 17 Oct 2026 |
| S13 | Set up cloud hosting for SEQTA | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141735-set-up-cloud-hosting-for-seqta | "Modified on Wed, 11 Mar" (2026) | 17 Oct 2026 |
| S14 | SEQTA Cloud Database Backup Service | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000151195-seqta-cloud-database-backup-service | "Modified on Fri, 4 Sep" (2026) | 17 Oct 2026 |
| S15 | Integrating SEQTA with MS Teams | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141305-integrating-seqta-with-ms-teams | "Modified on Fri, 27 Mar" (2026) | 17 Oct 2026 |
| S16 | OneDrive integration setup | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141483-onedrive-integration-setup | "Modified on Tue, 31 Mar" (2026) | 17 Oct 2026 |
| S17 | Google Drive integration setup | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000141288-google-drive-integration-setup | "Modified on Tue, 24 Mar" (2026) | 17 Oct 2026 |
| S18 | Start of Year Check-List DOE WA (Department of Education Western Australia) | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000143512-start-of-year-check-list-doe-wa-department-of-education-western-australia- | "Modified on Wed, 8 Apr" (2026) | 17 Oct 2026 |
| S19 | Start of Year Check-List: CEWA (Catholic Education Western Australia) | Tes (SEQTA help and support portal) | https://seqta.help.tes.com/support/solutions/articles/75000143083-start-of-year-check-list-cewa-catholic-education-western-australia- | "Modified on Thu, 9 Apr" (2026) | 17 Oct 2026 |
| S20 | SEQTA help and support portal (home page, and searches of its knowledge base for AI, MCP, ChatGPT, Claude, Copilot, Gemini, API, Zapier, Make and Power Automate) | Tes | https://seqta.help.tes.com/support/home | No date shown | 17 Oct 2026 |
| S21 | Privacy Notice (Australia edition) | Tes | https://www.tes.com/en-au/policies/privacy-notice | Last updated 3 Aug 2026 | 17 Oct 2026 |
| S22 | Tes Data Processing Agreement | Tes | https://www.tes.com/en-au/policies/data-processing-agreement | Last updated 10 Sep 2026 | 17 Oct 2026 |
| S23 | General Terms of Business (Australia edition) | Tes | https://www.tes.com/en-au/policies/general-terms-business | Last updated 29 Sep 2026 | 17 Oct 2026 |
| S24 | Tes sub-processors | Tes | https://www.tes.com/policies/sub-processors | No date shown | 17 Oct 2026 |
| S25 | Generative AI: Saving teachers time and improving planning | Tes (blog) | https://www.tes.com/en-au/for-schools/blog/article/generative-ai-saving-teachers-time-and-improving-planning | No date shown | 17 Oct 2026 |
| S26 | AI in Australian schools: Practical policy & classroom guidance for school leaders | Tes (blog) | https://www.tes.com/en-au/for-schools/blog/article/ai-australian-schools-practical-policy-classroom-guidance-school-leaders | No date shown | 17 Oct 2026 |
| S27 | Claude site map (Connectors Directory pages; 973 connectors listed, none for SEQTA) | Anthropic | https://claude.com/sitemap.xml | No date shown | 17 Oct 2026 |
| S28 | OpenAI plugin directory pages (13 category site maps, 336 plugin pages, none for SEQTA) | OpenAI | https://openai.com/sitemap.xml | No date shown | 17 Oct 2026 |
| S29 | Federated connectors overview | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview | Last updated on 16 Oct 2026 | 17 Oct 2026 |
| S30 | Partner-built connectors gallery | Microsoft Learn | https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-partners | Last updated on 27 Apr 2026 | 17 Oct 2026 |
| S31 | Microsoft Marketplace search: "seqta" (no SEQTA listing) | Microsoft | https://appsource.microsoft.com/en-us/marketplace/apps?search=seqta | No date shown | 17 Oct 2026 |
| S32 | Use & manage Connected Apps in Gemini (computer) | Google Gemini Apps Help | https://support.google.com/gemini/answer/13695044?hl=en&co=GENIE.Platform%3DDesktop | No date shown | 17 Oct 2026 |
| S33 | Connect & manage custom apps for Gemini Apps | Google Gemini Apps Help | https://support.google.com/gemini/answer/17209137 | No date shown | 17 Oct 2026 |
