# Gemini CLI Extension - Firestore

This Gemini CLI extension provides a set of tools to interact with [Firestore](https://cloud.google.com/firestore/docs) databases. It allows you to manage your databases, documents, and collections directly from the [Gemini CLI](https://google-gemini.github.io/gemini-cli/), using natural language prompts.

## Features

*   **Integrated with Gemini CLI:** As a Google-developed extension, it integrates seamlessly into the Gemini CLI environment, making security an accessible part of your workflow.
*   **Connect to Firestore:** Securely connect to your Firestore databases.
*   **Explore Database:** List collections and documents.
*   **Query your Database:** Execute queries against your database.

## Supported Tools

🟢 firestore-add-documents: Use this tool to add documents to a Firestore collection path.
🟢 firestore-get-documents: Use this tool to get multiple documents from Firestore by their paths.
🟢 firestore-list-collections: Use this tool to list Firestore collections for a given parent path.
🟢 firestore-delete-documents: Use this tool to delete multiple documents from Firestore.
🟢 firestore-query-collection: Use this tool to query documents from a collection with filtering, ordering, and limit options.
🟢 firestore-get-rules: Use this tool to retrieve the active Firestore security rules for the current project.
🟢 firestore-update-document: Use this tool to update an existing document in Firestore by its path.
🟢 firestore-validate-rules: Use this tool to validate Firestore security rules syntax and errors.

## Prerequisites

Before you begin, ensure you have the following:

*   [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed.
*   A Google Cloud project with the **Firestore API** enabled.
*   IAM Permissions

## Installation

To install the extension, use the `gemini extensions install` command:

```bash
gemini extensions install github.com/gemini-cli-extensions/firestore-native.git
```

## Configuration

*   `FIRESTORE_PROJECT`: The GCP project ID.
*   `FIRESTORE_DATABASE`: (Optional) The Firestore database ID.


## Usage

* Explore Schemas and Data
* Generate code


## Security

This extension executes commands against your Firestore database. Always review the generated queries before execution, especially for write operations.

## Disclaimer

This is not an officially supported Google product. This extension is under active development, and breaking changes may be introduced.
