# Smart Triage Dashboard AI-Powered Engineering Task Prioritization UI
Frontend-first AI dashboard that turns vague engineering requests into prioritized, assignable tasks.

# Smart Triage Dashboard

A frontend-first AI workflow dashboard that turns vague engineering tasks into structured, prioritized, and assignable work items.

![Smart Triage Dashboard screenshot](public/screenshots/Dashboard.png)

## Overview

Smart Triage Dashboard is a product concept and frontend prototype for engineering teams that receive vague, incomplete, or poorly scoped requests.

The dashboard is designed to help teams:

* Capture unclear tasks quickly
* Expand vague requests into actionable engineering work
* Estimate priority and urgency
* Recommend the right engineer based on skills and workload
* Visualize the triage queue in a clean operational dashboard

This version focuses on the frontend experience first. The AI expansion, prioritization, and assignment logic currently run through mock data and client-side logic, with the architecture prepared for a future backend and LLM integration.

## Problem

Engineering teams often receive tasks like:

> “The dashboard feels slow.”
>
> “Can we fix the onboarding issue?”
>
> “Something is wrong with notifications.”

These requests usually lack context, severity, ownership, and technical scope. As a result, engineers spend time clarifying, prioritizing, and routing work before real implementation can begin.

Smart Triage Dashboard explores how AI can help convert vague input into structured engineering execution.

## Core Features

### Vague Task Intake

Users can enter a rough or incomplete task description, similar to how requests arrive in Slack, Jira, Linear, or email.

### AI Task Expansion

The system expands vague input into a clearer engineering task with:

* Summary
* Possible root cause
* Suggested next steps
* Acceptance criteria
* Risk level

### Priority Scoring

Tasks are categorized by urgency and impact so teams can identify what needs immediate attention.

### Engineer Assignment

The dashboard recommends an engineer based on:

* Skill match
* Current workload
* Availability
* Task category

### Triage Queue

All generated tasks appear in a queue so the team can review, compare, and act on them.

## Tech Stack

* Next.js
* React
* TypeScript
* Tailwind CSS
* Mock AI logic for frontend-first development

## Current Status

This is an early frontend-first prototype.

Implemented:

* Dashboard UI
* Task intake form
* Mock triage generation
* Mock priority assignment
* Mock engineer recommendation
* Responsive layout

Planned:

* LLM-powered task expansion
* Backend API
* Authentication
* Jira / Linear / GitHub Issues integration
* Engineer workload sync
* Analytics dashboard
* Task history and audit trail

## Product Vision

The long-term goal is to create an AI-powered triage layer for engineering teams.

Instead of manually interpreting vague requests, the system would help teams move from:

> unclear request → structured task → priority → owner → next action

This could be useful for engineering managers, startup teams, platform teams, support engineering teams, and AI operations teams.

## Getting Started

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm run dev
```

Open the app locally:

```bash
http://localhost:3000
```

## Example Use Case

Input:

```text
Users are saying the dashboard is slow after uploading large CSV files.
```

Generated triage output:

```text
Priority: High
Category: Performance
Suggested Owner: Frontend / Platform Engineer
Expanded Task: Investigate dashboard performance degradation after large CSV uploads. Review client-side rendering, upload handling, and data processing bottlenecks.
```

## Why I Built This

I built this project to explore how AI can improve engineering operations by helping teams move faster from ambiguous requests to clear execution.

The first version focuses on the user experience and product workflow before adding the production AI/backend layer.

