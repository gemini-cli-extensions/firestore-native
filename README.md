# Gemini CLI Extension - Firestore Native

> [!NOTE]
> This extension is currently in beta, and may see breaking changes until the first stable release (v1.0).

This Gemini CLI extension provides a set of tools to interact with [Firestore](https://cloud.google.com/firestore/docs) databases. It allows you to manage your databases, documents, and collections directly from the [Gemini CLI](https://google-gemini.github.io/gemini-cli/), using natural language prompts.

Learn more about [Gemini CLI Extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extension.md).

## Why Use the Firestore Native Extension?

* **Natural Language Management:** Stop wrestling with complex commands. Explore schemas and query data by describing what you want in plain English.
* **Seamless Workflow:** As a Google-developed extension, it integrates seamlessly into the Gemini CLI environment. No need to constantly switch contexts for common database tasks.
* **Code Generation:** Accelerate development by asking Gemini to generate data classes and other code snippets based on your table schemas.

## Prerequisites

Before you begin, ensure you have the following:

*   [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed with version +v0.6.0.
*   A Google Cloud project with the **Firestore API** enabled.
*   IAM Permissions
    *   Cloud Datastore User (`roles/datastore.user`)
    *   Firebase Rules Viewer (`roles/firebaserules.viewer`) 

## Installation

To install the extension, use the `gemini extensions install` command:

```bash
gemini extensions install github.com/gemini-cli-extensions/firestore-native
```

## Configuration

Set the following environment variables before starting the Gemini CLI:

*   `FIRESTORE_PROJECT`: The GCP project ID.
*   `FIRESTORE_DATABASE`: (Optional) The Firestore database ID.

Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment. 

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

* "cannot execute binary file": Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://googleapis.github.io/genai-toolbox/getting-started/introduction/#installing-the-server) for more information.
