name: Failure building from source
about: Use this template when reporting a build failure
title: ''
labels: ['build', 't:bug']
assignees: ''
body:
- type: checkboxes
  attributes:
    label: Is there an existing issue for this?
    description: Please search to see if an issue already exists for the bug you encountered.
    options:
    - label: I have searched the existing issues
      required: true
- type: checkboxes
  attributes:
    label: Did you read the documentation and troubleshoot guide?
    description: Please read [README.md](https://github.com/sagemath/sage/blob/develop/README.md) and [the Troubleshooting sectionin the Installation Guide](https://doc.sagemath.org/html/en/installation/troubles.html).
    options:
    - label: I have read the documentation and troubleshoot guide
      required: true
- type: textarea
  attributes:
    label: Environment
    description: |
      examples:
        - **OS**: Ubuntu 20.04
    value: |
        - OS:
    render: markdown
  validations:
    required: true
- type: textarea
  attributes:
    label: Steps To Reproduce
    description: Steps to reproduce the behavior.
    placeholder: |
      1. In this environment...
      2. With this config...
      3. Run '...'
      4. See error...
  validations:
    required: false
- type: textarea
  attributes:
    label: Config log
    description: |
      Please attach `config.log`.
  validations:
    required: true
- type: textarea
  attributes:
    label: Package logs
    description: |
      Please attach ̀`logs/pkgs/SPKG.log` for failing packages.
  validations:
    required: false
- type: textarea
  attributes:
    label: Anything else?
    description: |
      Links? References? Anything that will give us more context about the issue you are encountering!

      Tip: You can attach images or log files by clicking this area to highlight it and then dragging files in.
  validations:
    required: false
