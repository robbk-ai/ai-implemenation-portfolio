# Email Automation – AI-Powered Triage & Communication

This project demonstrates how to use AI to reduce time spent on email by:
- Automatically **categorizing** messages
- Creating **priority levels**
- Generating **summaries** of long threads
- Drafting **first-pass replies** for review

It’s designed to be tool-agnostic: you can implement it with
- Outlook + Copilot
- Gmail + Gemini
- ChatGPT / other LLM tools

---

## 1. Problem

Knowledge workers spend 1–3 hours per day in email. A large portion of this time is:
- Scanning subject lines
- Opening low-value messages
- Manually writing standard responses
- Trying to remember action items from long threads

The goal of this project is to **turn email into a prioritized task list**, not a constant distraction.

---

## 2. Solution Overview

This workflow uses AI to:

1. **Triage inbox messages**
   - Categorize emails (Urgent, Action Needed, Info Only, Low Priority)
   - Identify who needs to respond and by when

2. **Summarize long threads**
   - Provide a short recap
   - Extract key decisions and open questions

3. **Draft replies**
   - Generate first-draft responses in your tone
   - You review and send

4. **Log action items**
   - Convert important emails into task lists or meeting notes

---

## 3. Triage Workflow (Step-by-Step)

1. Select 5–10 recent emails from your inbox.
2. Paste the subject + body into your AI tool of choice.
3. Use this prompt:

> *You are my email triage assistant. For each email, classify it with:  
> - Category: Urgent / Action Needed / Info Only / Low Priority  
> - Owner: Me / Someone else (specify who if visible)  
> - Due: Today / This week / No deadline / Ignore  
> - Summary: 1–2 sentence summary  
> - Suggested action: what I should do next.*

4. Apply the results:
   - Flag or star Urgent + Action Needed
   - Archive obvious Low Priority
   - Add reminders/tasks for time-bound items

Once the workflow is solid, this becomes a **repeatable daily process**.

---

## 4. Thread Summarization

Prompt template:

> *You are my email summary assistant. Summarize this email thread in 5 bullet points.  
> Highlight:  
> - The main decision(s)  
> - Any open questions  
> - Anything I am responsible for, with dates if mentioned.*

Use this for:
- Long chains with lots of “Reply All”
- Owner/client update threads
- Internal debates where you just need the bottom line

---

## 5. Drafting Replies

Prompt template:

> *You are my email drafting assistant. Write a clear, professional reply in my voice.  
> Goals:  
> - Be concise  
> - Be polite but direct  
> - Confirm any decisions  
> - Ask for missing info if needed  
>  
> Here is the email I am replying to:  
> [PASTE EMAIL]  
>  
> Here is what I want to say in bullet points:  
> - [point 1]  
> - [point 2]  
> - [point 3]*

You review, edit lightly, and send.

---

## 6. Implementation Notes

- **At work (Outlook + Copilot):**
  - Use the built-in “Summarize” and “Draft reply” features.
  - Keep the triage categories consistent (Urgent / Action / Info / Low).
  - Save your favorite prompts as quick snippets.

- **Personal email (Gmail + ChatGPT/Gemini):**
  - Use labels or stars that mirror the AI categories.
  - Batch process emails 2–3 times per day instead of constantly checking.

---

## 7. Future Enhancements

Planned improvements:
- A small prompt library file: `/prompts/email-triage-prompts.md`
- Example before/after screenshots (redacted)
- Time-saved estimates over a week
- A mini case study: “Reduced daily email time from X hours to Y minutes”

---

## 8. Business Impact

This project shows:
- Ability to analyze a common workflow (email)
- Use AI to design a **repeatable, documented process**
- Focus on **time savings and productivity**, not just “playing with AI”
- This approach can be rolled out to any team or client looking to reduce communication overhead.

