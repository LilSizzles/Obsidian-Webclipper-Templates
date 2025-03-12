# 📎 Obsidian-Webclipper-Templates

&nbsp;

![Obsidian Badge](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)
![LLM Badge](https://img.shields.io/badge/LLM_Powered-00B2FF?style=for-the-badge&logo=openai&logoColor=white)
![Research Badge](https://img.shields.io/badge/Research_Tool-FF5722?style=for-the-badge&logo=read-the-docs&logoColor=white)

&nbsp;

---

&nbsp;

## 📋 Overview

This project builds upon [Kepano's](https://bsky.app/profile/stephango.com) work on the Obsidian Webclipper. I've explored his approach to managing an [Obsidian Vault](https://stephango.com/vault) and adapted it to fit my BASB (Building a Second Brain) informed process. I mainly wanted to create one template to cover all the articles I will come in contact with so I can just 'one click' them no matter the website. It still needs work on tightening up the LMM prompts in general though I have found it helpful thus far.

The key enhancements include integration with:
- [Obsidian Properties](https://help.obsidian.md/properties)
- [Dataview](https://blacksmithgu.github.io/obsidian-dataview/) plugin

&nbsp;

---

&nbsp;

## 🤖 LLM Integration

These templates rely on using [Interpreter](https://help.obsidian.md/web-clipper/interpreter) for an LLM to:
1. Ingest webpage content
2. Generate structured outputs for different sections of the template

I currently use **Gemini 2** via Google's [AI Studio](https://aistudio.google.com/prompts/new_chat) with their API, which is cost-effective for these low-volume needs.

&nbsp;

---

&nbsp;

## 🎯 Purpose

As a Psychotherapist and Relational Meditation Researcher, I created these templates to streamline my research process when gathering information from various sources:
- Academic journals
- News articles
- Research papers
- And more

&nbsp;

---

&nbsp;

## 🧩 How It Works

The templates use specific prompt structures enclosed in double curly braces:

&nbsp;

```
{{ "prompt text that the LLM processes and responds to" }}
```

&nbsp;

### Example Prompt

The most complex prompt is used for the "Genre" property field:

&nbsp;

```
{{ "Analyze this article and classify it as exactly ONE of these types (respond with ONLY the type name):

Research: Academic journal articles, scientific studies, scholarly papers, conference proceedings, data-driven analysis with methodology, papers with citations and references

News: Factual reporting of current events, journalistic coverage, breaking news, investigative reporting, objective accounts of recent happenings

Opinion: Editorials, commentary, perspective pieces, viewpoints, subjective analysis, articles expressing personal judgment or stance on issues

Reviews: Critical evaluations of products/services/media, literature reviews, critiques, assessments that judge quality or performance

Informational: Educational content, tutorials, how-to guides, explainers, reference materials, articles that primarily aim to teach or inform without bias

If the article combines multiple types, select the PREDOMINANT category based on primary purpose and structure." | wikilink }}
```

&nbsp;

### Real-World Example

When testing with my personal website ([maxmilne.com article](https://maxmilne.com/index.php/2025/02/04/discovering-interbe-ing-a-personal-and-professional-journey/)), the Genre generated is: `[[meditation]]`.

This is a simple example of how this template works. 

&nbsp;

---

&nbsp;

## 🔗 Required Tools

&nbsp;

| Tool | Purpose | Link |
|------|---------|------|
| Obsidian | Note-taking app | [obsidian.md](https://obsidian.md) |
| Obsidian Webclipper | Browser extension | [Obsidian Help](https://help.obsidian.md/web-clipper) |
| Dataview | Query plugin | [GitHub](https://blacksmithgu.github.io/obsidian-dataview/) |
| Interpreter | LLM interface | [Obsidian Help](https://help.obsidian.md/web-clipper/interpreter) |
| Gemini 2 | LLM model | [Google AI Studio](https://aistudio.google.com/prompts/new_chat) |

&nbsp;

---

&nbsp;

## 📝 Getting Started

1. Install Obsidian and required plugins
2. Add these templates to your Obsidian vault
3. Configure Obsidian Webclipper with your preferred LLM
4. Start clipping and organizing your research!

&nbsp;

---

&nbsp;

*Inspired by BASB methodology and adapted for academic research workflows.* 

---

*Utilisted Claude 3.7 to aeshtetically rearrange the content.*
