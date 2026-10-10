# Jiro Build for Claude

Jiro Build is a library of 1,000+ production-ready website sections and full-page templates, built with React and Tailwind CSS. This plugin lets Claude search the library, show you live previews, and add the section or template you pick straight into your project, in chat, Cowork and Claude Code.

## What you can do

- **Find a section**: "Find a dark pricing section with a monthly/yearly toggle for my AI SaaS and add it to my landing page."
- **Start from a template**: "Start my fintech landing page from a Jiro Build template."
- **Compare options first**: "Show me three minimal testimonial sections with photos."
- **Check your plan**: "How many Jiro Build copies do I have left today?"

Claude searches with your words and filters (theme, look, industry, layout, motion, accent colors), shows each match with a link to its live preview on jiro.build, and fetches the code only for the item you choose.

## What's inside

| Component | What it adds |
|---|---|
| **Jiro Build connector** (`https://mcp.jiro.build`) | Three tools: `search_components`, `get_component`, `get_usage` |
| **add-section** skill | Finds one section or UI piece, lets you pick, and adds it |
| **build-landing-page** skill | Plans a whole page from one template or from matching sections |

## Requirements

- A Jiro Build account. You sign in through your browser the first time you connect. There are no API keys.
- A Jiro Build plan that includes MCP access. Search and fetch are part of paid plans. A free account can connect and check its plan, and Claude will explain what is locked. See [jiro.build/pricing](https://jiro.build/pricing).
- Each new item you fetch uses one of your plan's daily copies. Fetching the same item again the same day is free.

## Install

- **Claude (web, desktop, Cowork)**: open **Customize → Plugins**, find **Jiro Build**, select **Add**, then connect the Jiro Build connector from the plugin's **Connectors** tab and sign in. You can also add this repository directly: **Customize → Plugins → Add → Add marketplace**, then enter `Jiro-Build/claude-plugin`.
- **Claude Code**:

  ```bash
  claude plugin marketplace add Jiro-Build/claude-plugin
  claude plugin install jiro-build@jiro
  ```

  Then run `/mcp`, choose the Jiro Build server and select **Authenticate**.

## Data and privacy

This plugin runs nothing on your computer. It has no hooks and no scripts. Its skills are instructions for Claude, and its only connection is the Jiro Build MCP server at `https://mcp.jiro.build`.

- **Sent to Jiro Build**: your search words and filters, the slug of each item you fetch, and the sign-in token your Jiro Build account issues for Claude through OAuth.
- **Received from Jiro Build**: search results (names, summaries, style metadata, thumbnail and preview links), the code and build steps for items you fetch, and your plan and usage counts.
- **Stored by Jiro Build**: a record of each item you fetch, which counts toward your daily limit, and usage analytics tied to your account. Nothing else from your conversation is sent or stored.

Read the full [Jiro Build Privacy Policy](https://jiro.build/privacy-policy). You can disconnect Claude at any time from [jiro.build/settings/connected-apps](https://jiro.build/settings/connected-apps).

## Support

Questions or problems: [jiro.build/contact](https://jiro.build/contact).

## License

The files in this repository are released under the MIT License (see `LICENSE`). The components and templates you get from the Jiro Build library are licensed under the [Jiro Build Terms and Conditions](https://jiro.build/terms-conditions).
