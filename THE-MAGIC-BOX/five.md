You don’t need a full app for this. You need one structured “wrap-up extractor” pass at the end of the chat. Here are your real options, from simplest to most automated:

Option 1: Zero-Code Built-In Wrap-Up (Fastest)

At the end of any long session, paste this directly into ChatGPT:

Review this entire conversation and extract:

- Discussion Name:
    
- Date:
    
- Initial Prompt:
    
- Final Deliverables Produced:
    
- Key Decisions:
    
- Open Threads / Dropped Ideas:
    
- Next Actions:
    

Return as a single CSV row formatted for Google Sheets.

Then paste directly into Sheets or Excel. This already solves 80 percent of the problem.

Option 2: Reusable “Wrap-Up Semantic Overlay” for Custom GPTs

Add this as a locked tool prompt inside your custom GPT:

When the user says "wrap up this session", scan the full conversation and return:

1. Discussion Name
    
2. Date
    
3. Initial Objective
    
4. Deliverables Created
    
5. Abandoned Threads
    
6. Key Decisions
    
7. Next Actions
    

Output strictly as a single CSV row with quoted cells.

Now your team just types:

> wrap up this session

Instant spreadsheet-ready output.

Option 3: Semi-Automated Script Pipeline (If You Want True Automation)

If you export chats as JSON or text, this pipeline works well:

1. Export chat
    
2. Send to LLM with this system prompt:
    

You are a conversation analyst. Extract session metadata and summarize into structured CSV fields.

3. Auto-append output to Google Sheets via:

Zapier

Make

Or Google Apps Script webhook

This gives you a real logging system without rebuilding ChatGPT