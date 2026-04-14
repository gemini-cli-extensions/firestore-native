# DEVELOPER.md

This document provides instructions for setting up your development environment and contributing to the Firestore Native Gemini CLI Extension project.

## Prerequisites

Before you begin, ensure you have the following:

1.  **Gemini CLI:** Install the Gemini CLI version v0.6.0 or above. Installation instructions can be found on the [official Gemini CLI documentation](https://google-gemini.github.io/gemini-cli/). You can verify your version by running `gemini --version`.
2.  **Firestore database:** For testing skills, you will need access to an active Firestore database.

## Developing the Extension

### Running from Local Source

This extension uses **Agent Skills** to interact with Firestore. The development process involves generating these skills locally and linking the extension to the Gemini CLI.

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/gemini-cli-extensions/firestore-native.git
    cd firestore-native
    ```

2.  **Generate Skills:** Use the `toolbox` binary to generate the skills.

    ```bash
    # Set the required env vars for configuration.
    export FIRESTORE_PROJECT="<your-gcp-project-id>"
    export FIRESTORE_DATABASE="(default)" # Optional

    # Download the toolbox binary
    export VERSION=1.1.0
    curl -L -o toolbox https://storage.googleapis.com/mcp-toolbox-for-databases/v$VERSION/darwin/arm64/toolbox
    chmod +x toolbox

    # Generate skills for firestore-data
    ./toolbox --prebuilt firestore skills-generate --name "firestore-data" --description "Handles NoSQL document operations and collection hierarchy exploration. Use for CRUD tasks and data retrieval. Provides flexible document manipulation and structured querying." --toolset=data --license-header "// Copyright 2026 Google LLC
    //
    // Licensed under the Apache License, Version 2.0 (the \"License\");
    // you may not use this file except in compliance with the License.
    // You may obtain a copy of the License at
    //
    //      http://www.apache.org/licenses/LICENSE-2.0
    //
    // Unless required by applicable law or agreed to in writing, software
    // distributed under the License is distributed on an \"AS IS\" BASIS,
    // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    // See the License for the specific language governing permissions and
    // limitations under the License."

    # Generate skills for firestore-security
    ./toolbox --prebuilt firestore skills-generate --name "firestore-security" --description "Manages access control and security compliance. Use when auditing permissions or deploying new security logic. Provides rule retrieval and syntax validation." --toolset=security --license-header "// Copyright 2026 Google LLC
    //
    // Licensed under the Apache License, Version 2.0 (the \"License\");
    // you may not use this file except in compliance with the License.
    // You may obtain a copy of the License at
    //
    //      http://www.apache.org/licenses/LICENSE-2.0
    //
    // Unless required by applicable law or agreed to in writing, software
    // distributed under the License is distributed on an \"AS IS\" BASIS,
    // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    // See the License for the specific language governing permissions and
    // limitations under the License."
    ```

3.  **Link the Extension Locally:** Use the Gemini CLI to install the extension from your local directory.

    ```bash
    gemini extensions link .
    ```
    The CLI will prompt you to confirm the linking. Accept it to proceed.

4.  **Testing Changes:** After linking, start the Gemini CLI (`gemini`). You can now interact with the Firestore skills to manually test your changes.

## Testing

### Automated Skills Validation

A GitHub Actions workflow (`.github/workflows/skills-validate.yml`) is triggered for every pull request. This workflow validates the structure and content of the generated skills.

### Other GitHub Checks

*   **License Header Check:** A workflow ensures all necessary files contain the proper license header.
*   **Conventional Commits:** This repository uses [Release Please](https://github.com/googleapis/release-please) to manage releases. Your commit messages must adhere to the [Conventional Commits](https://www.conventionalcommits.org/) specification.

## Maintainer Information

### Team

The primary maintainers for this repository are defined in the [`.github/CODEOWNERS`](.github/CODEOWNERS) file:

*   `@gemini-cli-extensions/senseai-eco`
*   `@gemini-cli-extensions/firestore-native-maintainers`

### Releasing

The release process is automated using `release-please`. It consists of an automated changelog preparation step followed by the manual merging of a Release PR. When the Release PR is merged, `release-please` creates a new GitHub tag and a corresponding GitHub Release.
