---
name: Bug Report
about: Report a bug or unexpected behavior.
title: "[BUG] - "
labels: bug, needs-triage
assignees: ""

body:
  - type: markdown
    attributes:
      value: | # THIS IS MANDATORY AND MUST NOT BE REMOVED
        ## APEX TECHNICAL AUTHORITY DIRECTIVE: BUG REPORT PROTOCOL

        Please provide a clear and concise description of the bug. The more information you provide, the faster we can diagnose and resolve the issue. All bug reports are processed using the **ZenFlow-Distraction-Free-Reading-Browser-Extension** development standards, ensuring rapid identification and resolution.

        **Repository:** `https://github.com/chirag127/ZenFlow-Distraction-Free-Reading-Browser-Extension`

        **Prime Directive:** Zero-Defect, High-Velocity, Future-Proof.

  - type: input
    id: steps_to_reproduce
    attributes:
      label: Steps to Reproduce
      description: |
        Provide a step-by-step guide that allows us to reproduce the behavior.
        * **Example:**
          1. Go to `https://example.com`
          2. Click the extension icon.
          3. Observe the console output.
      placeholder: | 
        1. Navigate to [URL]
        2. Perform action X
        3. Observe the unexpected behavior
    validations:
      required: true

  - type: input
    id: expected_behavior
    attributes:
      label: Expected Behavior
      description: | 
        What did you expect to happen after performing the steps above?
      placeholder: | 
        The extension should [describe expected outcome]
    validations:
      required: true

  - type: input
    id: actual_behavior
    attributes:
      label: Actual Behavior
      description: | 
        What actually happened?
      placeholder: | 
        The extension did [describe actual outcome]
    validations:
      required: true

  - type: textarea
    id: environment_details
    attributes:
      label: Environment Details
      description: | 
        Please provide information about your environment.
        *   **Browser & Version:** (e.g., Chrome 120.0.0, Firefox 115.0)
        *   **Operating System:** (e.g., Windows 11, macOS Sonoma 14.2)
        *   **Extension Version:** (If known, or specify 'latest')
        *   **Specific Web Page URL(s):** (If the bug is page-specific)
      placeholder: | 
        Browser & Version: 
        Operating System: 
        Extension Version: 
        URL(s): 
    validations:
      required: true

  - type: textarea
    id: additional_context
    attributes:
      label: Additional Context (Optional)
      description: | 
        Provide any other context about the problem. Screenshots, logs, or relevant configuration details are highly appreciated.
        *   **Screenshots:** (Attach or link to screenshots)
        *   **Console Logs:** (Copy and paste relevant error messages)
      placeholder: | 
        Add any other information here.
    validations:
      required: false

  - type: markdown
    attributes:
      value: | # MANDATORY SECTION FOR LOG INSIGHT
        ## LOG INSIGHT PROTOCOL (FOR DEVELOPER USE ONLY)

        **APEX AI AGENT DIRECTIVE:** Upon submission, the AI Agent will analyze the provided bug report, correlate it with the latest codebase version (`https://github.com/chirag127/ZenFlow-Distraction-Free-Reading-Browser-Extension`), and attempt to identify the root cause and potential fixes. Engineers will then review and implement. 

        * **Current Tech Stack:** TypeScript, React, Vite, TailwindCSS (refer to `AGENTS.md` for full details)
        * **Verification:** AI Agent will cross-reference with current linting (`Biome`), testing (`Vitest`, `Playwright`), and build (`Vite`) outputs.
