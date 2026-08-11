# Hi, I'm Sunghun

Engineering student in Japan interested in software engineering, product development, and developer tools.

I enjoy identifying real operational problems, building solutions, and improving them through actual user feedback.

## Featured Project

### Restaurant Shift Management System

A web-based shift submission and management system built for real restaurant operations.

Built for an operation spanning **9 stores and approximately 130 staff members**.

**What I worked on**
- Employee shift submission workflow
- Manager-side scheduling and staffing management
- Required staffing configuration by weekday / holiday
- Automatic shortage detection
- Shift assignment assistance based on role and availability
- Role-based access control and Row Level Security
- Excel export for existing operational workflows
- Continuous improvements based on real user feedback

**Tech Stack**

`Next.js` `TypeScript` `Supabase` `PostgreSQL` `Vercel`

**Links**

- Repository: [add repository URL]
- Demo: [add demo URL]

---

## Open Source Contributions

### Salesforce — salesforcedx-vscode

Contributed to Salesforce's official VS Code extensions repository.

I investigated an issue where opening a `.cls` file in a non-Salesforce workspace could unintentionally activate the Salesforce Apex extension, start the Apex Language Server, and create `.sfdx/tools` artifacts.

**What I did**
- Reproduced the issue in a non-SFDX workspace
- Isolated `.cls` file opening as the trigger
- Traced the behavior from VS Code language association to Apex extension activation
- Identified Apex Language Server startup as the unwanted side effect
- Added a Salesforce-project guard using `ProjectService.isSalesforceProject()`
- Added regression tests for both Salesforce and non-Salesforce workspaces
- Verified the fix with 12 test suites / 115 tests, linting, and manual validation

My external **PR #7973** was adopted by Salesforce as internal **PR #7976** for their internal CI/review process and merged with my author credit preserved.

- Issue #7886  
  https://github.com/forcedotcom/salesforcedx-vscode/issues/7886

- My PR #7973  
  https://github.com/forcedotcom/salesforcedx-vscode/pull/7973

- Salesforce adoption / merged PR #7976  
  https://github.com/forcedotcom/salesforcedx-vscode/pull/7976

---

## Currently Building

### Restaurant Cost & Recipe Management System

Building a system for managing restaurant ingredients, recipes, and food costs.

Current focus:
- Ingredient management
- Recipe composition
- Automatic recipe cost calculation
- Food cost ratio analysis
- Architecture designed for future inventory, POS, and sales-analysis features

**Tech Stack**

`Next.js` `TypeScript` `Supabase` `PostgreSQL`

---

## Tech

**Languages**  
`TypeScript` `JavaScript` `Python`

**Web / Backend**  
`Next.js` `React` `Supabase` `PostgreSQL`

**Tools / Platforms**  
`Git` `GitHub` `VS Code` `Salesforce CLI`

---

## Interests

- Software Engineering
- Product Development
- Developer Tools
- Open Source
- Automation
