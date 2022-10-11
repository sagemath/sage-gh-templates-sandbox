name: Failure building from source
description: Use this template when reporting a build failure
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
