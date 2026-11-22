---
title: "What Is BusinessKit"
subtitle: "All your business tools in one workspace"
seo_title: "Get Started: What Is BusinessKit Unified Workspace for Small Teams"
slug: what-is-businesskit
description: "BusinessKit brings billing, inventory, accounting, CRM, and AI agents into a single workspace with a dedicated database for each profile in your organization."
app: get-started
collection: Get Started
type: concept
order: 1
created: 2026-10-23
updated: 2026-11-20
status: published
verified_from:
  - README.md
  - docs/ARCHITECTURE.md
  - src/routes/apps/index.tsx
related:
  - apps/browse-apps
  - get-started/create-first-profile
  - agents/what-are-agents
  - settings-account/how-data-is-stored
faq:
  - q: "Must you install every app at once?"
    a: "No. You select and install only the apps needed for your workflow. Free apps such as Link in Bio are available immediately, while others require a paid plan."
  - q: "Can one organization manage multiple businesses?"
    a: "Yes. An organization holds separate profiles, and each profile keeps its own isolated database. Plan limits determine how many profiles you can add."
  - q: "Is the full interface available on mobile devices?"
    a: "Most workspace features work on mobile, but the built-in terminal runs only on desktop computers."
---

BusinessKit is a unified desktop and mobile workspace for small businesses, combining billing, inventory, bookkeeping, CRM, web publishing, and autonomous AI agents. Each business profile connects to an isolated, dedicated database hosted on Turso Cloud.

> **Note:** BusinessKit uses dedicated remote Turso databases for every profile (BYODB). Business data from one client or enterprise is never commingled with another, and queries are executed over HTTPS via the lightweight `TursoConn` pipeline shim with zero local database files.

## Modular Apps

You customize your workspace by installing apps tailored to your daily tasks. An independent retailer might rely on Shop and Accounts, while a consultancy might focus on CRM, Forms, and Content.

| Workspace | Included tools | Best suited for |
| --- | --- | --- |
| Shop | Point of sale, item variants, inventory tracking, dining tables, and stay folios | Retailers, cafes, and hotels |
| Finance | Chart of accounts, bank statement reconciliation, expense logs, and tax returns | Bookkeepers and business owners |
| CRM | Contact records, lead stages, and deal pipelines | B2B sales and consulting |
| Content | Personal notes, public documentation, blog posts, and scheduled social updates | Writers, founders, and marketers |
| Operations | Form builders, applicant tracking for job listings, and member spaces | Hiring teams and communities |
| Agents | Interactive AI assistants with tools to query and update your records | Teams automating routine entries |

Additional tools appear on the Apps page. [Browse Apps](/docs/apps/browse-apps) details which workspaces come free and which require a subscription.

## Profiles and Databases

Your account belongs to an organization. Inside that organization, you create distinct profiles for each venture or client project.

Each profile connects to its own remote database. Invoices, contacts, and inventory from one business do not mingle with another. You switch between profiles using the profile selector, or open extra workspaces in separate desktop windows using `Cmd+Shift+N` (macOS) or `Ctrl+Shift+N` (Windows/Linux).

## Built-in Agents

Agents provide conversational assistants capable of taking actions inside your current profile. An agent can record incoming supplier stock, prepare an invoice draft, or log a newly acquired contact.

Agent tools only interact with the active profile. They cannot read information from other businesses in your organization or inspect your account sign-in details. Desktop versions also include a terminal for running local command-line tools, though that terminal is omitted on mobile devices.

## Next

- [Create Your First Profile](/docs/get-started/create-first-profile): Set up a dedicated workspace.
- [Browse Apps](/docs/apps/browse-apps): Review available workspaces and plan tiers.
- [What Are Agents](/docs/agents/what-are-agents): Compare conversational, CLI, and terminal workflows.
- [How Your Data Is Stored](/docs/settings-account/how-data-is-stored): Learn how profile databases remain isolated.

## Content / CMS HTML Export

```html
<p>BusinessKit is a unified desktop and mobile workspace for small businesses, combining billing, inventory, bookkeeping, CRM, web publishing, and autonomous AI agents. Each business profile connects to an isolated, dedicated database hosted on Turso Cloud.</p>

<div data-type="info-card" class="tech-callout tech-callout--info" role="note">
  <div class="tech-callout__content">
    <p><strong>Database Isolation (BYODB):</strong> BusinessKit uses dedicated remote Turso databases for every profile. Business data from one client or enterprise is never commingled with another, and queries are executed over HTTPS via the lightweight <code>TursoConn</code> pipeline shim without local database files.</p>
  </div>
</div>

<h2>Modular Business Workspaces</h2>
<p>Tailor your daily operations by installing only the applications your team needs. Every app communicates seamlessly within the active profile workspace.</p>

<table>
  <thead>
    <tr>
      <th>Workspace App</th>
      <th>Core Capabilities</th>
      <th>Target Workflows</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Shop &amp; Inventory</strong></td>
      <td>Point of sale, batch tracking, stock receipts, and barcodes</td>
      <td>Retail stores, pharmacies, restaurants, and wholesalers</td>
    </tr>
    <tr>
      <td><strong>Accounts &amp; Finance</strong></td>
      <td>Double-entry ledger, bank reconciliation, GST &amp; tax returns</td>
      <td>Accountants, bookkeepers, and finance controllers</td>
    </tr>
    <tr>
      <td><strong>CRM &amp; Sales</strong></td>
      <td>Contact directory, sales deals, lead pipelines, and notes</td>
      <td>Agencies, consultancies, and B2B sales teams</td>
    </tr>
    <tr>
      <td><strong>Content &amp; Publishing</strong></td>
      <td>Blogs, documentation, newsletters, and social scheduling</td>
      <td>Marketing teams, technical writers, and creators</td>
    </tr>
    <tr>
      <td><strong>Operations &amp; HR</strong></td>
      <td>Form builders, hiring pipelines, and member portals</td>
      <td>HR departments, operations managers, and recruiters</td>
    </tr>
    <tr>
      <td><strong>Autonomous AI Agents</strong></td>
      <td>Conversational assistants, MCP server tools, and background CLI</td>
      <td>Automating catalog entry, triage, and data entry</td>
    </tr>
  </tbody>
</table>

<h2>Multi-Profile Organization Architecture</h2>
<p>Your account belongs to an organization that houses separate profiles for each business, client, or regional brand.</p>

<div data-type="steps" class="tech-steps">
  <div data-type="step-item" class="tech-step">
    <div data-type="step-title" class="tech-step__title">1. Organization Management</div>
    <div data-type="step-content" class="tech-step__content">
      <p>Single sign-on via WorkOS provides central authentication and team membership across all enterprise ventures.</p>
    </div>
  </div>
  <div data-type="step-item" class="tech-step">
    <div data-type="step-title" class="tech-step__title">2. Isolated Profile Databases</div>
    <div data-type="step-content" class="tech-step__content">
      <p>Each profile uses an encrypted AES-256-GCM connection string pointing to its dedicated remote Turso database instance.</p>
    </div>
  </div>
  <div data-type="step-item" class="tech-step">
    <div data-type="step-title" class="tech-step__title">3. Multi-Window Multitasking</div>
    <div data-type="step-content" class="tech-step__content">
      <p>Open separate desktop windows (<kbd class="tech-kbd">⌘</kbd> + <kbd class="tech-kbd">Shift</kbd> + <kbd class="tech-kbd">N</kbd> on macOS or <kbd class="tech-kbd">Ctrl</kbd> + <kbd class="tech-kbd">Shift</kbd> + <kbd class="tech-kbd">N</kbd> on Windows) to operate multiple client profiles concurrently.</p>
    </div>
  </div>
</div>

<h2>What Built-in Agents Can Do</h2>
<p>BusinessKit includes autonomous AI agents equipped with native MCP tools to execute operations directly on your behalf.</p>

<ul data-type="taskList">
  <li data-type="taskItem" data-checked="true"><label><input type="checkbox" checked="checked" /></label><div><p>Receive vendor invoices and automatically restock inventory items</p></div></li>
  <li data-type="taskItem" data-checked="true"><label><input type="checkbox" checked="checked" /></label><div><p>Create customer sales bills and issue GST-compliant invoices</p></div></li>
  <li data-type="taskItem" data-checked="true"><label><input type="checkbox" checked="checked" /></label><div><p>Capture inbound CRM leads and update deal status stages</p></div></li>
  <li data-type="taskItem" data-checked="true"><label><input type="checkbox" checked="checked" /></label><div><p>Author and publish rich semantic documentation articles and newsletters</p></div></li>
</ul>

<h2>Frequently Asked Questions</h2>
<div data-type="accordion-group" class="tech-accordion">
  <div data-type="accordion-item" class="tech-accordion__item" data-open="true">
    <div data-type="accordion-title" class="tech-accordion__summary">Must you install every app at once?</div>
    <div data-type="accordion-content" class="tech-accordion__content">
      <p>No. You select and install only the apps needed for your workflow. Free apps such as Link in Bio are available immediately, while others require a paid plan.</p>
    </div>
  </div>
  <div data-type="accordion-item" class="tech-accordion__item" data-open="false">
    <div data-type="accordion-title" class="tech-accordion__summary">Can one organization manage multiple businesses?</div>
    <div data-type="accordion-content" class="tech-accordion__content">
      <p>Yes. An organization holds separate profiles, and each profile keeps its own isolated database. Plan limits determine how many profiles you can add.</p>
    </div>
  </div>
  <div data-type="accordion-item" class="tech-accordion__item" data-open="false">
    <div data-type="accordion-title" class="tech-accordion__summary">Is the full interface available on mobile devices?</div>
    <div data-type="accordion-content" class="tech-accordion__content">
      <p>Most workspace features work on mobile, but the built-in terminal runs only on desktop computers.</p>
    </div>
  </div>
</div>
```
