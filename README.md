# IAM Audit Automation

## Vision

Build an AI-powered IAM Audit Assistant using:

- n8n
- OpenAI
- Google Sheets

---

# Learning Journey

## Day 1 (2026-07-07)

### Achievement

- Created first n8n workflow
- Connected OpenAI API
- Generated IAM risk analysis

### Learning

Prompt = instructions given to AI.

---

## Day 2 (2026-07-08)

### Achievement

- Learned variables
- Used dynamic data
- Passed access_data to OpenAI

### Learning

Data Source
↓
Variable
↓
Prompt
↓
AI

---

## Day 3 (2026-07-09)

### Achievement

- Connected Google Sheets
- Retrieved real user access data
- Sent user-role dataset to OpenAI
- Generated IAM audit findings

### Workflow

Manual Trigger
↓
Google Sheets
↓
Basic LLM Chain
↓
OpenAI Chat Model

### Key Learning

System Message:
Defines AI identity and rules.

User Message:
Provides data and task.

Source for Prompt:
Defines where User Message comes from.

### Challenge Found

Google Sheets returned 5 items.

OpenAI was called 5 times.

Potential issue:
Higher API cost.

### Next Goal

Aggregate all rows into a single dataset before sending to OpenAI.

Target:

Google Sheets
↓
Aggregate
↓
1 OpenAI Call
↓
1 Audit Report
``
