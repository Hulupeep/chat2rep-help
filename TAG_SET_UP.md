# Tagging Guide

**Tags make your notes searchable and unlock automation magic.**

---

## How Tags Work

Chat2Repo works best when ChatGPT automatically adds small tags at the end of your messages. These tags let Chat2Repo:
1. **Organize** — Route content into the right folders
2. **Search** — Find anything by topic, type, or project
3. **Automate** — Trigger GitHub Actions based on tags

**STEP 1:** Get ChatGPT to add #tags at the end of relevant chats
**STEP 2:** [Create GitHub Actions based on your tags](githubactions)

---

## Quick Start: Default Tag Set

Copy/paste this into ChatGPT's **Custom Instructions → "How should ChatGPT respond?"**

> "At the end of relevant responses, add 2-4 hashtags from these categories:
> - Content type: #Spec #Ideas #Notes #Review #NextActions
> - Work type: #Planning #Design #Research #Writing #Feedback
> - Project: #Project:YourProjectName
>
> Only add tags when relevant. Place all tags at the very end."

---

## Default Tag Categories

### Content Type Tags
*What* the message represents:

| Tag | Use for |
|-----|---------|
| `#Spec` | Specifications, requirements, architecture |
| `#Journeys` | User journeys, flows, interactions |
| `#Ideas` | Raw ideas, brainstorming |
| `#Notes` | Miscellaneous notes, insights |
| `#Review` | Summaries, critiques, analysis |
| `#NextActions` | Action items, steps to take |

### Work Type Tags
The *purpose* of the content:

| Tag | Use for |
|-----|---------|
| `#Planning` | Planning and outlining |
| `#Design` | UI/UX or conceptual design |
| `#Research` | Research findings, references |
| `#Writing` | Content writing, drafts |
| `#Feedback` | Comments, suggestions, revisions |

### Project Routing
Route content to the right project folder:

`#Project:ShortName`

Examples: `#Project:Website` `#Project:MobileApp` `#Project:Marketing`

---

## Tags for Teachers

A complete tag system for educators:

### By Resource Type
| Tag | Use for |
|-----|---------|
| `#LessonPlan` | Full lesson plans |
| `#Starter` | Starter activities |
| `#Plenary` | Plenary/exit ticket activities |
| `#Homework` | Homework tasks |
| `#ExamQuestions` | Assessment questions |
| `#Rubric` | Marking criteria, success criteria |
| `#ParentEmail` | Parent communication templates |
| `#Worksheet` | Student worksheets |
| `#Scheme` | Schemes of work |

### By Year Group
`#Year7` `#Year8` `#Year9` `#Year10` `#Year11` `#SixthForm` `#KS3` `#KS4` `#KS5`

### By Subject (English examples)
`#Shakespeare` `#Macbeth` `#Othello` `#Poetry` `#CreativeWriting` `#Grammar` `#Reading`

### By Approach
`#Differentiation` `#SEN` `#EAL` `#Stretch` `#Scaffolded`

### Teacher Custom Instructions

Add this to ChatGPT's Custom Instructions:

> "At the end of teaching resources, add relevant hashtags:
> - Type: #LessonPlan #Starter #ExamQuestions #Homework #Rubric
> - Year: #Year7 through #Year13, or #KS3 #KS4 #KS5
> - Topic: Subject-specific tags like #Shakespeare #Poetry #Algebra
> - Approach: #Differentiation #SEN #EAL when applicable"

### Example Teacher Prompts

**Lesson planning:**
> "Create a 50-minute lesson on photosynthesis for Year 8 with differentiated tasks #LessonPlan #Biology #Year8 #Differentiation"

**Question generation:**
> "Write 10 exam-style questions on Macbeth Act 1 #ExamQuestions #Macbeth #Year11"

[See the full Teachers Guide →](TEACHERS)

---

## Tags for Writers

### By Project Stage
| Tag | Use for |
|-----|---------|
| `#idea` | Story ideas, concepts |
| `#outline` | Plot outlines, structures |
| `#draft` | Draft chapters, scenes |
| `#character` | Character development |
| `#worldbuilding` | Setting, world details |
| `#research` | Background research |

### By Project
Name your projects: `#novel` `#shortStory` `#theHeist` `#summerProject`

---

## Tags for Developers

### By Type
| Tag | Use for |
|-----|---------|
| `#bug` | Bug analysis, fixes |
| `#feature` | Feature planning |
| `#architecture` | System design |
| `#debug` | Debugging sessions |
| `#api` | API design, docs |

### By Technology
`#react` `#typescript` `#python` `#node` `#sql`

---

## Create Your Own Tag Set

Want a personalized system? Ask ChatGPT:

> "Help me create a custom tag system for Chat2Repo. Organize tags into:
> 1. Content Type (what it is)
> 2. Work Type (what it's for)
> 3. Project Routing (#Project:Name)
>
> Then turn it into Custom Instructions I can paste into ChatGPT."

---

## Best Practices

1. **Keep tags short** — `#idea` not `#thisIsAnIdea`
2. **Be consistent** — Pick a format and stick to it
3. **Use 2-4 tags** — Enough to find it, not noise
4. **Tag type + topic** — `#LessonPlan #Poetry` tells you what AND about what
5. **Set defaults** — Put common tags in Options so they're automatic

---

## Next Step: Automation Magic

Once your notes are tagged, GitHub Actions can do amazing things automatically.

[**Set up GitHub Actions →**](githubactions)

---

[← Back to Home](.) | [Installation](INSTALL) | [How to Use](GUIDE) | [For Teachers](TEACHERS)
