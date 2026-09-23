# Azure Cloud Portfolio

My personal portfolio site, hosted on **Microsoft Azure** and deployed automatically from GitHub.

**Live site:** _(add your Azure URL here once it's deployed)_

## What this project does

- Hosts a static portfolio website on **Azure Static Web Apps**
- Every time I push a change to GitHub, **GitHub Actions** automatically redeploys the site (CI/CD)

## AZ-900 concepts applied

| AZ-900 area | What I used it for in this project |
|---|---|
| Cloud concepts: PaaS | Azure Static Web Apps is a platform service: Azure manages the servers, and I only manage my code |
| Cloud concepts: consumption pricing | Runs on the Free tier; I explain why it costs $0 below |
| Azure architecture: resource groups | All project resources live in one resource group (`rg-cloud-portfolio`) so I can manage or delete them together |
| Azure architecture: regions | Chose a US East region, close to my target users in NJ/NY |
| Management & governance: Cost Management | Set a budget alert so I'm notified before any unexpected charges |
| Management & governance: tags | Tagged resources with `project` and `environment` for cost tracking |

## Architecture

```
Me (VS Code) --> GitHub repo --> GitHub Actions --> Azure Static Web Apps --> Visitors
```

## Cost

_(Explain the tier you picked and what your budget alert is set to.)_

## What I learned

_(Write 3–4 bullets after you finish: what was confusing, what clicked, what you'd do differently.)_

## Next steps

- [ ] Add a visitor counter using **Azure Functions** + **Cosmos DB** (serverless)
- [ ] Add monitoring with **Application Insights**
