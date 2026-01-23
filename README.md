# Gemini CLI Extension - Firestore Native

> [!NOTE]
> This extension is currently in beta (pre-v1.0), and may see breaking changes until the first stable release (v1.0).

This Gemini CLI extension provides a set of tools to interact with [Firestore](https://cloud.google.com/firestore/docs) databases. It allows you to manage your databases, documents, and collections directly from the [Gemini CLI](https://google-gemini.github.io/gemini-cli/), using natural language prompts.

Learn more about [Gemini CLI Extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/index.md).
> [!IMPORTANT]
> **We Want Your Feedback!**
> Please share your thoughts with us by filling out our feedback [form][form]. 
> Your input is invaluable and helps us improve the project for everyone.

[form]: https://docs.google.com/forms/d/e/1FAIpQLSfEGmLR46iipyNTgwTmIDJqzkAwDPXxbocpXpUbHXydiN1RTw/viewform?usp=pp_url&entry.157487=firestore-native

## Why Use the Firestore Native Extension?

* **Natural Language Management:** Stop wrestling with complex commands. Explore schemas and query data by describing what you want in plain English.
* **Seamless Workflow:** As a Google-developed extension, it integrates seamlessly into the Gemini CLI environment. No need to constantly switch contexts for common database tasks.
* **Code Generation:** Accelerate development by asking Gemini to generate data classes and other code snippets based on your table schemas.

## 📺 Video Walkthrough
Follow this step-by-step video walkthrough to setup and use the Firestore Native Extension.
<p align="center">
<a href="https://youtu.be/mQGIANnQnCI"><img src="https://github.com/user-attachments/assets/feb798ad-8963-47c0-abf2-f34b4b847bca" alt="Video Tutorial" width="50%" /></a>
</p>

## Prerequisites

Before you begin, ensure you have the following:

* [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed with version **+v0.6.0**.
* Setup Gemini CLI [Authentication](https://github.com/google-gemini/gemini-cli/tree/main?tab=readme-ov-file#-authentication-options).
* A Google Cloud project with the **Firestore API** enabled.
* Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.
* IAM Permissions
    * Cloud Datastore User (`roles/datastore.user`)
    * Firebase Rules Viewer (`roles/firebaserules.viewer`)

## Getting Started

### Installation

To install the extension, use the `gemini extensions install` command:

```bash
gemini extensions install https://github.com/gemini-cli-extensions/firestore-native
```

### Configuration

Set the following environment variables before starting the Gemini CLI. These variables can be loaded from a `.env` file.

```bash
export FIRESTORE_PROJECT="<your-gcp-project-id>"
export FIRESTORE_DATABASE="(default)" # Optional
```

Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.

### Start Gemini CLI

To start the Gemini CLI, use the following command:

```bash
gemini
```

> [!WARNING]
> **Changing Database Connections**
> Currently, the database connection must be configured before starting the Gemini CLI and can not be changed during a session.
> To save and resume conversation history use command: `/chat save <tag>` and `/chat resume <tag>`.

## Usage Examples

Interact with Firestore using natural language right from your IDE:

* **Document and Data Retrieval**:

  * "Show me the Firestore data for the test users qa_user_123 and qa_user_456 from the users-staging collection."
  * "Find all users in the users-staging collection whose wishlist contains product-glasses."

* **Document Updates and Cleanup**:
  * "For all 20 test users you just found, please remove product-glasses(inactive) from their wishlist."
  * "Update the document with ID order-987 in the orders collection to set the status to 'Shipped'."

* **Security Rules Management**:
  * "new_rules.txt is a new Firestore Security Rule I'm working on for staging. Can you validate it for me?"
  * "Show me the active Firestore security rules for this project."

## Supported Tools

This extension provides a comprehensive set of tools:

* `add_documents`: Use this tool to add documents to a Firestore collection path.
* `get_documents`: Use this tool to get multiple documents from Firestore by their paths.
* `list_collections`: Use this tool to list Firestore collections for a given parent path.
* `delete_documents`: Use this tool to delete multiple documents from Firestore.
* `query_collection`: Use this tool to query documents from a collection with filtering, ordering, and limit options.
* `get_rules`: Use this tool to retrieve the active Firestore security rules for the current project.
* `update_document`: Use this tool to update an existing document in Firestore by its path.
* `validate_rules`: Use this tool to validate Firestore security rules syntax and errors.

## Additional Extensions

Find additional extensions to support your entire software development lifecycle at [github.com/gemini-cli-extensions](https://github.com/gemini-cli-extensions).

## Troubleshooting

Use `gemini --debug` to enable debugging.

Common issues:

* "failed to find default credentials: google: could not find default credentials.": Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment. See [Set up Application Default Credentials](https://cloud.google.com/docs/authentication/external/set-up-adc) for more information.
* "✖ Error during discovery for server: MCP error -32000: Connection closed": The database connection has not been established. Ensure your configuration is set via environment variables.
* "✖ MCP ERROR: Error: spawn /Users/USER/.gemini/extensions/firestore-native/toolbox ENOENT": The Toolbox binary did not download correctly. Ensure you are using Gemini CLI v0.6.0+.
* "cannot execute binary file": The Toolbox binary did not download correctly. Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://googleapis.github.io/genai-toolbox/getting-started/introduction/#installing-the-server) for more information.
