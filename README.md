# forms.app for Claude

Create any online form from a conversation with Claude, collect unlimited responses, and turn the results into insight. The plugin connects Claude to your [forms.app](https://forms.app) account and adds a skill that teaches Claude how to build, edit, and analyze forms well.

## What you can do

- **Create forms from a description.** "Create an onboarding survey for a branding agency with contact details, brand personality questions, and must-haves."
- **Edit existing forms.** Add or rewrite questions, set up conditional logic, scoring, thank-you pages, design, and publishing schedules.
- **Preview forms in the chat.** Claude can show an interactive preview of a published form, or open your form library to pick one.
- **Evaluate performance.** "Look at my job application form's content, drop-off rates, and statistics, and tell me how to improve conversions."
- **Analyze submissions.** "Based on our employee survey responses, what should we prioritize to improve morale and collaboration?"
- **Visualize results.** "Get the statistics and drop-off rates of my feedback form and create visuals I can use in a presentation."

## Getting started

1. Install the plugin.
2. Open the plugin's **Connectors** tab and connect **forms.app**. You'll sign in to your forms.app account through forms.app's own OAuth page. If you don't have an account yet, you can create one there for free.
3. Ask Claude to create or analyze a form.

In Claude Code, install the plugin and then run `/mcp` to sign in:

```
/plugin marketplace add forms-app/forms.app-claude-plugin
/plugin install forms-app@forms-app-plugins
```

## What's included

| Component | Purpose |
| --- | --- |
| `forms-app` connector (`.mcp.json`) | The remote forms.app MCP server at `https://api.forms.app/mcp` |
| `forms-app` skill | Instructions for creating, editing, previewing, and analyzing forms with the connector's tools |

## Data and privacy

- The plugin contains no code that runs on your device. It holds only Markdown, JSON, and an icon.
- All actions go through the forms.app MCP server at `https://api.forms.app/mcp`, which acts on your forms.app account after you sign in. Form content, settings, and the submissions and statistics you ask about are exchanged between Claude and forms.app.
- The plugin sends no data to any other service and stores nothing itself. forms.app stores your forms and responses under its [Privacy Policy](https://forms.app/en/privacy-policy) and [Terms of Service](https://forms.app/en/terms).

## Support

Contact the forms.app team at [forms.app/en/contact-us](https://forms.app/en/contact-us).
