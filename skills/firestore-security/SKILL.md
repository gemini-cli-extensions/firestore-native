---
name: firestore-security
description: Manages access control and security compliance. Use when auditing permissions or deploying new security logic. Provides rule retrieval and syntax validation.
---

## Usage

All scripts can be executed using Node.js. Replace `<param_name>` and `<param_value>` with actual values.

**Bash:**
`node <skill_dir>/scripts/<script_name>.js '{"<param_name>": "<param_value>"}'`

**PowerShell:**
`node <skill_dir>/scripts/<script_name>.js '{\"<param_name>\": \"<param_value>\"}'`

Note: The scripts automatically load the environment variables from various .env files. Do not ask the user to set vars unless skill executions fails due to env var absence.


## Scripts


### get_rules

Retrieves the active Firestore security rules for the current project



---

### validate_rules

Checks the provided Firestore Rules source for syntax and validation errors. Provide the source code to validate.

#### Parameters

| Name | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| source | string | The Firestore Rules source code to validate | Yes |  |


---

