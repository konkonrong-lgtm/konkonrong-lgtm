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

---

**Links**

- Repository: https://github.com/konkonrong-lgtm/shift-management-system-portfolio
- Staff Demo: https://demo-shift.vercel.app/s/demo
- Manager Demo: https://demo-shift.vercel.app/manager/demo/login  
  Password: `1111`

---

## Security Research

### Salesforce — Cross-Org Metadata Operation Integrity

Independently identified and responsibly disclosed a cross-org metadata operation integrity issue in Salesforce Extensions for VS Code.

Traced the issue to mutable target-org state across a single metadata operation lifecycle, reproduced the failure conditions, analyzed the affected execution and source-tracking paths, and developed a scoped remediation with regression tests.

Salesforce Product Security confirmed that the reported findings were successfully reproduced and that the Engineering team was working on remediation.

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

## Developer Tools

### mf-check — Salesforce Multi-Framework Preflight CLI

A CLI for detecting configuration, linkage, and GraphQL compatibility issues in Salesforce Multi-Framework projects before deployment.

Designed to catch deployment blockers and environment mismatches early, with a current focus on React-based Salesforce Multi-Framework applications.

**What it checks**
- UI Bundle configuration and build output
- CustomApplication → UI Bundle linkage
- Lightning application configuration
- Permission Set application visibility
- GraphQL operations against the target Salesforce org schema

Published as an npm package with automated tests and GitHub Actions CI.

**Tech Stack**

`TypeScript` `GraphQL` `Salesforce CLI` `Vitest` `GitHub Actions`

**Install**

```bash
npm install -g @konkonrong/mf-check
```

**Links**

- Repository: https://github.com/konkonrong-lgtm/mf-check
- npm: https://www.npmjs.com/package/@konkonrong/mf-check

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
