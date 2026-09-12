# n8n_gmail_summarizer

# Gmail AI Email Summarizer using n8n and Google Gemini

An automated email summarization workflow built using n8n, Gmail API, Google Gemini, and JavaScript.

This project collects unread Gmail threads, combines their content, analyzes them using Google Gemini AI, and sends a concise summary back to Gmail.

---

## Project Overview

Managing multiple emails can be time-consuming. This project automates the process of reading and summarizing emails using an AI-powered workflow.

The workflow:

1. Fetches unread Gmail threads.
2. Combines email snippets using JavaScript.
3. Sends the combined content to Google Gemini.
4. Generates an intelligent summary.
5. Sends the summary to the user's Gmail account.

The workflow can be triggered manually or scheduled automatically.

---

## Features

- Fetch unread Gmail emails automatically.
- Summarize multiple emails using Google Gemini AI.
- Identify important emails and required actions.
- Highlight urgent tasks and deadlines.
- Ignore unnecessary promotional content.
- Send the generated summary through Gmail.
- Support manual and scheduled execution.
- Low-code automation using n8n.
- Exportable workflow for backup and version control.

---

## Workflow Architecture

```text
                Manual Trigger
                     │
                     ▼
               Schedule Trigger
                     │
                     ▼
          Gmail - Get Many Threads
                     │
                     ▼
              Code Node
          Combine Email Snippets
                     │
                     ▼
          Google Gemini AI Model
             Analyze and Summarize
                     │
                     ▼
             Gmail - Send Message
                     │
                     ▼
              Email Summary
