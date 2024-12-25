# Tailwind CSS: Styles Not Applied Due to Incorrect `content` Array Configuration

This repository demonstrates a common yet often overlooked issue in Tailwind CSS: the improper configuration of the `content` array within the `tailwind.config.js` file.  When the `content` array is missing or incorrectly specifies the files where Tailwind should look for class names, styles may fail to apply, leading to frustrating debugging sessions.

The `bug.js` file showcases the problematic configuration. The `bugSolution.js` file presents the corrected configuration.

## Steps to Reproduce

1. Clone this repository.
2. Observe that in `bug.js` styles are not applied because of incorrect `content` configuration.
3. Compare with the corrected configuration in `bugSolution.js` and verify that the issue is fixed.

## Resolution

Ensure that the `content` array in your `tailwind.config.js` file accurately reflects the locations of your template files (e.g., HTML, Vue, React, etc.).  Tailwind uses this information to scan your project for class names and generate the appropriate CSS rules.