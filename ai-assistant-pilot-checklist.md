# AI Assistant Pilot Checklist

Use this checklist before an AI assistant answers customers or employees. It keeps the first pilot narrow, reviewable and easy to pause.

## 1. Choose one useful job

Write one sentence describing what the assistant may do.

> Example: Answer common service questions from approved public pages and offer a human handoff when the answer is uncertain.

Avoid combining sales, support, account changes and internal operations in the first pilot.

## 2. Approve the source material

- List every page, document or knowledge source the assistant may use.
- Confirm that the material is current and that you have permission to use it.
- Exclude passwords, API keys, private customer messages and unnecessary personal data.
- Name the person responsible for updating each source.

## 3. Define the answer boundary

Document what the assistant may answer and what it must escalate.

Escalate when:

- the approved sources do not support the answer;
- a customer asks for a price, promise or policy exception that needs approval;
- the request involves billing, credentials, sensitive personal data or account access;
- the user asks for a person;
- the assistant detects conflicting source material.

The assistant should say when it is uncertain. It should never invent a policy, order status, quotation or completed action.

## 4. Design the human handoff

Specify:

- where the conversation is handed off;
- who owns the handoff;
- the expected response window;
- what short summary is passed to the person;
- when the assistant may resume after a human reply.

Pass only the information needed for the handoff. Do not silently add people to marketing lists.

## 5. Test with a fixed question set

Create at least 20 synthetic questions covering:

- clear questions with a supported answer;
- vague or incomplete questions;
- requests outside the approved scope;
- requests for a person;
- misleading premises and conflicting instructions;
- attempts to obtain private information or make the assistant ignore its rules.

For every test, record whether the correct result is **answer**, **clarify**, **handoff** or **refuse**.

## 6. Set launch checks

Before limited release, confirm:

- every answer is grounded in an approved source;
- unsupported questions are escalated instead of guessed;
- the human contact path works;
- conversation history and logs follow the agreed retention rule;
- the assistant can be disabled quickly;
- a named person reviews failures and source updates.

## 7. Review the pilot

Use a small sample and measure separate facts:

- questions received;
- supported answers;
- clarifications requested;
- human handoffs;
- incorrect or unsupported answers;
- average response time;
- customer-reported problems.

Do not report a successful deployment from a demo alone. Expand only after the pilot meets the agreed accuracy and handoff checks.

## Simple acceptance record

| Check | Owner | Result | Evidence |
| --- | --- | --- | --- |
| Approved sources are current |  |  |  |
| Out-of-scope requests hand off |  |  |  |
| Human contact path works |  |  |  |
| No private test data is present |  |  |  |
| Disable/pause control works |  |  |  |
| Pilot results were reviewed |  |  |  |

