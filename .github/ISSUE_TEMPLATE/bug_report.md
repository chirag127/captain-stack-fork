---
name: Bug Report
description: Report a technical issue, crash, or unexpected behavior.
title: "[BUG] - "
labels: ["bug", "triage", "needs-investigation"]
assignees:
  - chirag127
body:
  - type: markdown
    attributes:
      value: |
        ### **CodePilot AI Bug Report**
        Thank you for helping improve CodePilot! To ensure a swift resolution, please complete this form with as much detail as possible.

  - type: checkboxes
    id: prerequisites
    attributes:
      label: Prerequisites
      description: Please confirm the following before submitting.
      options:
        - label: I have searched the [existing issues](https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/issues) to ensure this is not a duplicate.
          required: true
        - label: I am using the latest version of the **CodePilot** extension.
          required: true
        - label: I have confirmed this bug is reproducible with the provided steps.
          required: true

  - type: textarea
    id: bug-description
    attributes:
      label: Bug Description
      description: "Provide a clear and concise summary of the issue. What is the core problem?"
      placeholder: "e.g., Code suggestions are not appearing for Python files after the latest update."
    validations:
      required: true

  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to Reproduce
      description: "Detail the exact, step-by-step sequence to reproduce the behavior."
      placeholder: |
        1. Open a `.ts` file.
        2. Type `function example() {`
        3. ...
    validations:
      required: true

  - type: textarea
    id: expected-behavior
    attributes:
      label: Expected Behavior
      description: "What did you expect to happen?"
      placeholder: "I expected to see an inline code suggestion to complete the function body."
    validations:
      required: true

  - type: textarea
    id: actual-behavior
    attributes:
      label: Actual Behavior
      description: "What actually happened? Include any error messages from the VSCode Output panel or Developer Tools console."
      placeholder: "Nothing happened, and an error `[CodePilot] API request failed` appeared in the logs."
    validations:
      required: true

  - type: input
    id: vscode-version
    attributes:
      label: VSCode Version
      description: "Run `code --version` in your terminal."
      placeholder: "e.g., 1.95.0"
    validations:
      required: true

  - type: input
    id: extension-version
    attributes:
      label: CodePilot Extension Version
      description: "You can find this in the VSCode Extensions view."
      placeholder: "e.g., v1.2.3"
    validations:
      required: true

  - type: dropdown
    id: os
    attributes:
      label: Operating System
      description: "Which operating system are you using?"
      options:
        - Windows
        - macOS
        - Linux
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: Relevant Logs or Screenshots
      description: "Please paste any relevant logs inside the code block below. You can find logs in the VSCode Output panel (select 'CodePilot AI' from the dropdown)."
      render: shell

  - type: textarea
    id: additional-context
    attributes:
      label: Additional Context (Optional)
      description: "Is there anything else we should know? (e.g., specific project setup, other extensions that might be conflicting)."
