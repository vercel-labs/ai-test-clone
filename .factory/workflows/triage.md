---
description: Classify pull requests into bugs, features, others
on: { events: [issue.created] }
actions:
  github.read_issue: true
  github.add_label: { labels: ['feature', 'bug', 'other'] }
---

Check the issue content and decide if it is a 'feature', 'bug', 'other'.

Then label the issue with a matching label.