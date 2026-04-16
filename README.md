# Firestore Native Agent Skills

> [!NOTE]
> Currently in beta (pre-v1.0), and may see breaking changes until the first stable release (v1.0).

This repository provides a set of agent skills to interact with [Firestore](https://cloud.google.com/firestore/docs) databases. These skills can be used with various AI agents, including [Gemini CLI](https://google-gemini.github.io/gemini-cli/), Claude Code, and Codex, to manage your databases, collections, and documents using natural language prompts.

> [!IMPORTANT]
> **We Want Your Feedback!**
> Please share your thoughts with us by filling out our feedback [form][form].
> Your input is invaluable and helps us improve the project for everyone.

[form]: https://docs.google.com/forms/d/e/1FAIpQLSfEGmLR46iipyNTgwTmIDJqzkAwDPXxbocpXpUbHXydiN1RTw/viewform?usp=pp_url&entry.157487=firestore-native

## Table of Contents

- [Why Use Firestore Native Agent Skills?](#why-use-firestore-native-agent-skills)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Configuration](#configuration)
  - [Installation & Usage](#installation--usage)
    - [Gemini CLI](#gemini-cli)
    - [Claude Code](#claude-code)
    - [Codex](#codex)
    - [Antigravity](#antigravity)
- [Usage Examples](#usage-examples)
- [Supported Skills](#supported-skills)
- [Additional Agent Skills](#additional-agent-skills)
- [Troubleshooting](#troubleshooting)

## Why Use Firestore Native Agent Skills?

- **Seamless Workflow:** Integrates seamlessly into your AI agent's environment. No need to constantly switch contexts for common database tasks.
- **Natural Language Queries:** Stop wrestling with complex commands. Explore schemas and query data by describing what you want in plain English.
- **Data Management:** Manage your Firestore data directly from your agent.
- **Code Generation:** Accelerate development by asking your agent to generate data classes and other code snippets based on your document structures.

## 📺 Video Walkthrough
Follow this step-by-step video walkthrough to setup and use the Firestore Native Extension.
<p align="center">
<a href="https://youtu.be/mQGIANnQnCI"><img src="https://github.com/user-attachments/assets/feb798ad-8963-47c0-abf2-f34b4b847bca" alt="Video Tutorial" width="50%" /></a>
</p>

## Prerequisites

Before you begin, ensure you have the following:

- One of these AI agents installed
  - [Gemini CLI](https://github.com/google-gemini/gemini-cli) version **v0.6.0** or higher
  - [Claude Code](https://claude.com/product/claude-code) version **v2.1.94** or higher
  - [Codex](https://developers.openai.com/codex) **v0.117.0** or higher
  - [Antigravity](https://antigravity.google) **v1.14.2** or higher
- A Google Cloud project with the **Firestore API** enabled.
- Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.
- IAM Permissions:
    * Cloud Datastore User (`roles/datastore.user`)
    * Firebase Rules Viewer (`roles/firebaserules.viewer`)

## Getting Started

### Configuration

Please keep these env vars handy during the installation process:

- `FIRESTORE_PROJECT`: The GCP project ID.
- `FIRESTORE_DATABASE`: (Optional) The Firestore database ID. Defaults to `(default)`.

> [!NOTE]
>
> - Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.

### Installation & Usage

To start interacting with your database, install the skills for your preferred AI agent, then launch the agent and use natural language to ask questions or perform tasks.

For the latest version, check the [releases page][releases].

[releases]: https://github.com/gemini-cli-extensions/firestore-native/releases

<!-- {x-release-please-start-version} -->

<details open>
<summary id="gemini-cli">Gemini CLI</summary>

**1. Install the extension:**

```bash
gemini extensions install https://github.com/gemini-cli-extensions/firestore-native
```

During the installation, enter your environment vars as described in the [configuration section](#configuration).

**2. (Optional) Manage Configuration:**
To view or update your configuration in Gemini CLI:

- Terminal: `gemini extensions config firestore-native [setting name] [--scope <scope>]`
- Gemini CLI: `/extensions list`

**3. Start the agent:**

```bash
gemini
```

_(Tip: Run `/extensions list` to verify your configuration and active extensions.)_

> [!WARNING]
> **Changing Database Connections**
> Currently, the database connection must be configured before starting the agent and can not be changed during a session.
> To save and resume conversation history in Gemini CLI use command: `/chat save <tag>` and `/chat resume <tag>`.

</details>

<details>
<summary id="claude-code">Claude Code</summary>

**1. Set env vars:**
In your terminal, set your environment vars as described in the [configuration section](#configuration).

**2. Start the agent:**

```bash
claude
```

**3. Add the marketplace:**

```bash
/plugin marketplace add https://github.com/gemini-cli-extensions/firestore-native.git#0.3.0
```

**4. Install the plugin:**

```bash
/plugin install firestore-native@firestore-native-marketplace
```

_(Tip: Run `/plugin list` inside Claude Code to verify the plugin is active, or `/reload-plugins` if you just installed it.)_

</details>

<details>
<summary id="codex">Codex</summary>

**1. Clone the Repo:**

```bash
git clone --branch 0.3.0 git@github.com:gemini-cli-extensions/firestore-native.git
```

**2. Install the plugin:**

```bash
mkdir -p ~/.codex/plugins
cp -R /absolute/path/to/firestore-native ~/.codex/plugins/firestore-native
```

**3. Set env vars:**
Enter your environment vars as described in the [configuration section](#configuration).

**4. Create or update marketplace.json:**
`~/.agents/plugins/marketplace.json`

```json
{
  "name": "my-data-cloud-google-marketplace",
  "interface": {
    "displayName": "Google Data Cloud Skills"
  },
  "plugins": [
    {
      "name": "firestore-native",
      "source": {
        "source": "local",
        "path": "./plugins/firestore-native"
      },
      "policy": {
        "installation": "AVAILABLE",
        "authentication": "ON_INSTALL"
      },
      "category": "Database"
    }
  ]
}
```

_(Tip: Run `codex plugin list` or use the `/plugins` interactive menu to verify your installed plugins.)_

</details>

<details>
<summary id="antigravity">Antigravity</summary>

**1. Clone the Repo:**

```bash
git clone --branch 0.3.0 https://github.com/gemini-cli-extensions/firestore-native.git
```

**2. Install the skills:**

Choose a location for the skills:
- **Global (all workspaces):** `~/.gemini/antigravity/skills/`
- **Workspace-specific:** `<workspace-root>/.agents/skills/`

Copy the skill folders from the cloned repository's `skills/` directory to your chosen location:

```bash
cp -R firestore-native/skills/* ~/.gemini/antigravity/skills/
```

**3. Set env vars:**
Set your environment vars as described in the [configuration section](#configuration).

_(Tip: Antigravity automatically discovers skills in these directories at the start of a session.)_

</details>

<!-- {x-release-please-end} -->

## Usage Examples

Interact with Firestore using natural language:

- **Document and Data Retrieval**:
  - "Show me the Firestore data for the test users qa_user_123 and qa_user_456 from the users-staging collection."
  - "Find all users in the users-staging collection whose wishlist contains product-glasses."
- **Document Updates and Cleanup**:
  - "For all 20 test users you just found, please remove product-glasses(inactive) from their wishlist."
  - "Update the document with ID order-987 in the orders collection to set the status to 'Shipped'."

## Supported Skills

The following skills are available in this repository:

- [Firestore Data](./skills/firestore-data/SKILL.md) - Handles NoSQL document operations and collection hierarchy exploration. Use for CRUD tasks and data retrieval. Provides flexible document manipulation and structured querying.

## Additional Agent Skills

Find additional skills to support your entire software development lifecycle at [github.com/gemini-cli-extensions](https://github.com/gemini-cli-extensions).

## Troubleshooting

Use the debug mode of your agent (e.g., `gemini --debug`) to enable debugging.

Common issues:

- "failed to find default credentials: google: could not find default credentials.": Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment. See [Set up Application Default Credentials](https://cloud.google.com/docs/authentication/external/set-up-adc) for more information.
- "✖ Error during discovery for server: MCP error -32000: Connection closed": The database connection has not been established. Ensure your configuration is set via environment variables.
- "✖ MCP ERROR: Error: spawn .../toolbox ENOENT": The Toolbox binary did not download correctly. Ensure you are using the latest version of your agent.
- "cannot execute binary file": The Toolbox binary did not download correctly. Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://mcp-toolbox.dev/documentation/introduction/#install-toolbox) for more information.
