# Project & Task Management BI Dashboard

A multi-view Power BI dashboard built to give different stakeholders — executives, managers, and employees — a role-specific window into project status, task progress, and approval workflows, all from a single connected data model.

## Overview

The report is organized into five report pages, each designed around what a specific stakeholder needs to see and act on:

| Page | Audience | Purpose |
|---|---|---|
| **CEO View** | Leadership | High-level KPIs and project-level rollups for quick decision-making |
| **Manager View** | Team managers | Task-level tracking, ownership, and progress monitoring |
| **Approval Workflow** | Approvers | Pending decisions and approval history by project |
| **Alerts Panel** | All users | Priority-flagged issues and upcoming deadlines |
| **Employee Proposal** | Employees | Project proposals, objectives, and resource requests |

## Key Features

- **Executive summary cards** — Total Tasks, Overdue Tasks, Completion %, and Pending Approvals surfaced as at-a-glance KPIs on the CEO View
- **Project performance chart** — clustered column chart comparing total tasks across projects
- **Interactive drill-down tables** — project status, task ownership, and due-date hierarchies, filterable via slicers
- **Approval workflow tracking** — approval level, decision status, and reviewer comments per project
- **Priority alerting system** — flags overdue and upcoming-due tasks by priority and assignee, with read/unread status
- **Proposal intake view** — lets employees submit and track new project proposals with objectives and resource needs, alongside approval decisions

## Data Model

The report connects four core tables into a relational model:

- **Projects** — project name, status, initiator, objective, resource needs, deadlines
- **Tasks** — task name, assignee, status, progress %, due dates, milestone flags
- **Approvals** — project linkage, decision, approval level, reviewer comments
- **Alerts** — alert message, priority, assignee, read status, due dates

Custom DAX measures power the KPI cards, including:
- `Total Tasks`
- `Overdue Tasks`
- `Completion %`
- `Upcoming Due`
- `Pending Approvals`

## Tools Used

- **Power BI Desktop** — data modeling, DAX measures, report design
- **DAX** — custom calculated measures for KPI tracking
- Interactive slicers, tables, and cards for cross-filtered, role-based reporting

## File

- `dashboard_powerBI.pbix` — open in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free) to explore the full report, data model, and DAX measures.

---

*Built as a personal project to demonstrate BI dashboard design, data modeling, and stakeholder-focused reporting.*
