name: Bug Report
description: Report a reproducible issue or malfunction.
title: "[Bug]: "
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Provide all details necessary to reproduce the issue.
  - type: input
    id: summary
    attributes:
      label: Summary
      description: Short description of the issue.
      placeholder: "The download page freezes when clicking 'Start'"
    validations:
      required: true
  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      description: Provide clear, step-by-step reproduction instructions.
      placeholder: |
        1. Go to...
        2. Click...
        3. Observe...
    validations:
      required: true
  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
    validations:
      required: true
  - type: textarea
    id: actual
    attributes:
      label: Actual Behavior
    validations:
      required: true
  - type: input
    id: env
    attributes:
      label: Environment
      placeholder: "Browser: Chrome 124, OS: Ubuntu 25.04"
  - type: textarea
    id: logs
    attributes:
      label: Logs / Console Output
      render: bash
