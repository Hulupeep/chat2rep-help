 

# **Add ChatGPT Tags and generate some magic**

Chat2Repo works best when ChatGPT automatically adds small tags at the end of your messages.
These tags let Chat2Repo route each chat into the correct folders and THEN let GitHub Actions automate useful tasks.

#### STEP 1: Tags - Get Chatgpt To add #tags at the end of relevant chats. 

#### **STEP 2: Magic -[Create Github actions based on your tags.](githubactions.md) **



#### Step 1: Tags

---

##### **OPTION 1 — Use the Default Tag Set (Recommended for Everyone)**

Copy/paste this into ChatGPT’s **Custom Instructions → “How should ChatGPT respond?”**

##### **Default Tag Categories**

**1. Content Type Tags**
Used to describe *what* the message represents.

* `#Spec` — specifications, requirements, architecture
* `#Journeys` — user journeys, flows, interactions
* `#Ideas` — raw ideas, brainstorming
* `#Notes` — miscellaneous notes, insights
* `#Review` — summaries, critiques, analysis
* `#NextActions` — action items or steps to take

**2. Work Type Tags**
Used to describe the *purpose* of the content.

* `#Planning` — planning and outlining
* `#Design` — UI/UX or conceptual design
* `#Research` — research findings or references
* `#Writing` — content writing or drafts
* `#Feedback` — comments, suggestions, revisions

**3. Project Routing Tag**
Used to route content into the correct project folder.

* `#Project:{ShortName}`
  Example: `#Project:Website`, `#Project:MobileApp`, `#Project:Marketing`

### **Rules**

* Only add tags when they clearly match the message
* Place all tags **at the very end** of the response
* Keep responses clear and structured so Chat2Repo can process them

This set works for **any project**, **any user**, **any industry**, with zero customization needed.

---

##### **OPTION 2 — Generate Your Own Tag Set (Advanced Users)**

If you want a personalized tagging system, ChatGPT can help you design it.

Paste this into ChatGPT:

**“Help me create a custom tag system for Chat2Repo.
Organize tags into:

1. Content Type (e.g., specs, ideas, notes),
2. Work Type (e.g., planning, design, research, writing),
3. Project Routing (#Project:{ShortName}).
   Explain what each tag means and when I should use it.”**

Then refine:

**“Refine this tag set to match my workflow. Ensure the tags are only added when relevant and always placed at the end of responses.”**

Finally generate your Custom Instructions:

**“Turn this tag system into a concise Custom Instructions section I can paste into ChatGPT respecting the character limit of 1,500 given there is content there alread.”**

Paste the result into ChatGPT’s Custom Instructions panel.

---

Next: C  **STEP 2: Magic -[Create Github actions based on your tags.](githubactions.md) **
