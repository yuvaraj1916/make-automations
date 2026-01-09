# AI-Powered Multi-Platform Social Media Automation

> Exported from Make.com | Automation Blueprint

## Description
This Make.com automation automatically generates **platform-specific social media content** and publishes it to **LinkedIn, Facebook Pages, and Telegram**.  
The automation uses **Google Sheets as the content source** and **Google Gemini AI** to summarize and adapt content according to each platform’s posting format.

---

## Workflow Overview
1. User adds a **link (URL)** to Google Sheets
2. Content is summarized using **Google Gemini AI**
3. A router splits the flow for multiple platforms
4. Platform-specific content is generated using separate Gemini AI modules
5. Content is automatically posted to social media platforms

---

## Trigger
- **Google Sheets**  
  - New row added with a link to be summarized and posted

---

## Data Source (Google Sheets)
The Google Sheet contains:
- **Content Link (URL)** – Link to the article/post to summarize
- *(Optional)* Additional metadata such as title or category

---

## AI Processing
- **Google Gemini AI (Summary Generator)**
  - Summarizes the original content from the provided link

- **Google Gemini AI (Platform Content Generators)**
  - LinkedIn-optimized post
  - Facebook-optimized post
  - Telegram-optimized message

Each AI module generates content according to platform tone and formatting.

---

## Routing Logic
- **Router Module**
  - Splits the automation into multiple paths
  - Each path handles a different social media platform

---

## Actions (Posting Modules)
- **LinkedIn**
  - Posts platform-ready content to LinkedIn profile/page

- **Facebook Pages**
  - Publishes formatted content to a Facebook Page

- **Telegram**
  - Sends content using Telegram Bot API

---

## Apps & Services Used
- Make.com
- Google Sheets
- Google Gemini AI
- LinkedIn
- Facebook Pages
- Telegram Bot

---

## Use Case
- Automate content distribution across multiple social platforms
- Save time by generating platform-specific posts automatically
- Maintain consistent posting with optimized formatting per platform
- Ideal for creators, marketers, and personal branding

---

## Import Instructions
1. Download the automation `.json` file
2. Open Make.com
3. Create a new scenario
4. Click **Import Blueprint**
5. Upload the JSON file
6. Reconnect all apps and credentials

---

## Notes
- API keys and credentials are **not included**
- Platform permissions must be configured manually
- Content format can be customized inside Gemini AI prompts

---

## Version
- Automation Blueprint v1.0
