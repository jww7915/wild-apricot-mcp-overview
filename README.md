# Wild Apricot MCP

**Connect your AI assistant to Wild Apricot for member administration, events, financial records, and website work.**

Created and owned by **Justin Williams**. Built for Wild Apricot organizations and service providers working with authorized client accounts.

**117 supported API operations · 35 native gadget guides · 3 skill categories**

[Discuss a demonstration or license](mailto:justin@justw.me?subject=Wild%20Apricot%20MCP%20inquiry)

## What it does

Describe a task in ordinary language. Your AI assistant uses the MCP's tools to read or update Wild Apricot and return the result.

Use it to:

- Find and update contacts and members, review membership information, and handle pending membership approvals.
- Create and update events, work with registrations and waitlists, and check in attendees.
- Review or update invoices, payment records, refunds, and donations.
- Work with supported email operations, store products and orders, and continuing-education records.
- Update page content through the Wild Apricot website editor and check the saved result.

The package supports both reading and writing. Each installation connects to its own Wild Apricot account and uses that account's authorized access.

## How it works

**MCP** stands for **Model Context Protocol**. It is a standard way for an AI application to discover tools and request actions. Your chosen application supplies the AI; Wild Apricot MCP supplies the connection to Wild Apricot.

**Your request → AI assistant → Wild Apricot MCP → Wild Apricot**

Two connections handle different kinds of work:

| Connection | What it handles |
| --- | --- |
| **Wild Apricot API** | Business records such as contacts, memberships, events, registrations, and invoices, using your API key. |
| **Signed-in Google Chrome** | Website-editor work using your administrator session and configured page and gadget targets. |

The server runs locally as a Node.js program. Your AI application starts it and exchanges messages through a local MCP connection, known as **stdio**. Website workflows use the browser connection when needed.

## Three skill categories

Skills are reusable instructions that help the assistant follow a consistent process.

| Category | What it helps you do |
| --- | --- |
| **Wild Apricot Operations** | Find the right records, perform member, event, registration, and financial tasks, and confirm saved changes. |
| **Wild Apricot Website Editor** | Edit existing, configured **Content** and **Custom HTML** gadgets through Chrome. Use the **35 native gadget guides** with a companion browser connection for directories, forms, menus, calendars, photos, and other gadget settings. |
| **Wild Apricot Website QA** | Reopen saved content and check links, audience access, preserved gadgets, and desktop, tablet, and mobile layouts using the appropriate browser sessions. |

The instructions can be installed as skills where your AI application supports them, or used as workflow references.

## Applications you can use

Wild Apricot MCP uses the local MCP connection supported by applications such as:

- **[Codex](https://developers.openai.com/codex/mcp)**
- **[Claude Desktop](https://modelcontextprotocol.io/docs/2026-07-28/develop/connect-local-servers)** with local MCP configuration
- **[Cursor](https://cursor.com/docs/mcp)**
- **[VS Code with GitHub Copilot](https://code.visualstudio.com/docs/agent-customization/mcp-servers)**
- **[Google Antigravity](https://antigravity.google/docs/mcp)**

Each application has its own MCP configuration and permission controls. Website work also uses Google Chrome.

## Getting started

1. **Arrange your license.** Contact Justin to agree on the team, organization or client accounts, and any onboarding or support needed.
2. **Install the package.** Authorized users receive the installation package, documentation, and configuration examples. Install Node.js **22.12 or newer** and the package on the computer running your AI application.
3. **Connect your account.** Create a Wild Apricot server-application API key, keep it in a private local configuration file, and register the local MCP server in your AI application.
4. **Confirm the connection.** Restart the application and ask the assistant to identify the connected organization. Add the skill instructions where supported.
5. **Add website work.** Configure the intended pages and gadgets, sign in to Chrome as a Wild Apricot administrator, and add the companion browser connection for native gadget settings.

## Example requests

> Summarize all active members by membership level.

> Find the contact with this email address, update only their phone number, and confirm the saved value.

> List everyone registered for this event, including their registration type and payment status.

> List all unpaid invoices, group them by contact, and total the balances.

> Update the introduction on my configured page. Preserve the native gadgets and check the saved result on desktop, tablet, and mobile.

For useful results, identify the exact person, event, or page; specify the date range or requested change; and ask the assistant to confirm what was saved.

## Licensing and contact

Wild Apricot MCP is **proprietary software owned by Justin Williams**. Use is licensed by written agreement, including the scope of any work on client accounts. Pricing, account coverage, updates, and support are agreed before purchase.

**Contact:** [justin@justw.me](mailto:justin@justw.me?subject=Wild%20Apricot%20MCP%20inquiry)

This repository contains the public product overview only. The MCP implementation, reusable skill files, and installation packages are distributed privately to authorized users. Access to this overview does not grant a software license.

Product scope described here: **version 0.2.6**.

Copyright © 2026 Justin Williams. All rights reserved. See [COPYRIGHT](COPYRIGHT).
