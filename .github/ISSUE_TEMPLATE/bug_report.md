---
name: Bug report
about: Create a report to help us improve
title: ''
labels: [bug]
assignees: ''
body:
  - type: dropdown
    id: crate
    attributes:
      label: Which crate is this issue about?
      multiple: true
      options:
        - `windows`
        - `windows-sys`
  - type: textarea
    attributes:
      label: Crate Version
      description: What is the version of the crate you're using?
      placeholder: You can find the exact crate version used in your `Cargo.lock` file.
    validations:
      required: false
  - type: textarea
    attributes:
      label: Code Example
      description: |
        Thank you for filing a bug report! 🐛 Please provide a short summary of the
        bug, along with any information you feel relevant to replicating the bug.
      placeholder: |
        ```rust
        <code>
        ```
    validations:
      required: false
  - type: textarea
    attributes:
      label: Expected Behavior
      description: I expected to see this happen:
      placeholder: *explanation*
    validations:
      required: false
  - type: textarea
    attributes:
      label: Actual Behavior
      description: Instead, this happened:
      placeholder: *explanation*
    validations:
      required: false
---