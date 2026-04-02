# CLAUDE.md — InsureMyBiz123 (daven-insurance)

## Project Overview
Commercial insurance agency website operating as an affiliate of Daven Insurance Agency.
- **Live URL:** insuremybiz123.com
- **GitHub repo:** bb313x/daven-insurance
- **Owner:** Bryan Boutins
- **Licensed in:** NY, NJ, and FL

## Tech Stack
- Single-file HTML/CSS/JS — no frameworks, no build tools
- **Deployment:** GitHub → Hostinger manual deploy via hPanel
- **CRM:** Monday.com (workspace: bryanboutins-team)

## Business Context
- Affiliate model under Daven Insurance Agency
- Target audience: Small business owners needing commercial insurance
- Sister businesses: Lets Grow Digital (LGD), MaxLifeMD (vitamd)
- Recently completed a full visual rebrand
- Previous deployment issue: Hostinger Git deploy misconfiguration was serving stale version — resolved

## Deployment Workflow
1. Edit HTML file locally
2. Commit and push to GitHub
3. Deploy manually via Hostinger hPanel (file upload or Git deploy)
4. Verify live site is serving latest version after each deploy

## Coding Conventions
- Single-file architecture is intentional — do not split into separate CSS/JS files
- Mobile-responsive by default
- No npm, no node_modules, no build step
- CSS variables for all colors and design tokens

## What Claude Should NOT Do
- Do not suggest multi-file architecture
- Do not add npm dependencies or build tools
- Do not expose any API tokens in client-side code
- Do not redesign the brand without explicit instruction
- Do not use placeholder copy — ask if real copy is needed
