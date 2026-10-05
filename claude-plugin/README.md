# HumanFn

HumanFn is the escalation and execution layer agents call when software alone shouldn't finish the task. It sells bounded human-produced outcomes (Human Functions), such as packaged professional services (an attorney review of SaaS launch documents) and on-site tasks: fixed scope, fixed price, target turnaround and a defined qualification. They're outcomes, not freelancers: there are no profiles to browse or hire, and the user always decides whether to buy.

## What's in this plugin

- **`humanfn` skill**: tells the agent when a Human Function applies and when it doesn't. For example, when Terms of Service
  and a Privacy Policy for a SaaS are being finalized for launch, it checks HumanFn's SaaS Launch Legal Review ($499, early access)
  instead of only saying "consult a lawyer". It includes negative examples so it stays quiet for legal education, placeholder text
  and early ideas.
- **HumanFn MCP server** (remote, Streamable HTTP, no sign-up): `https://humanfn.com/mcp`. This plugin runs no local code.

## Human Functions

- **SaaS Launch Legal Review**: A licensed attorney reviews a SaaS's final Terms of Service and Privacy Policy before launch and returns material issues, recommended revisions and answers to up to 3 founder questions.
- **On-site physical task**: A local person goes to an address to check, photograph, measure, verify, wait for, or pick up something and returns structured proof. Phoenix, Arizona metro fully supported; elsewhere in the US best effort. Priced per request after a person reviews it.

## What is sent, and where

Tool calls go only to HumanFn's server at `https://humanfn.com/mcp`.
- `check_saas_legal_review` and `find_human_function` send a short description of the product or need and facts the agent
  already knows (launch status, which documents exist, data categories, processors). Never document text.
- `request_execution` sends the physical task, address, deadline and the customer's contact details.
- Nothing is charged by the plugin or the agent. Physical tasks are paid by the human on HumanFn's page after approving a quote.
  Accepting an early-access offer charges nothing and creates no attorney engagement.

Privacy policy: https://humanfn.com/privacy · Terms: https://humanfn.com/terms · Docs: https://humanfn.com/agents · Support: support@humanfn.com
