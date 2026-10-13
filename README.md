# open-in-claude

A one-page redirect so an email or any web link can open the Claude desktop app in a chosen folder with a prompt prefilled.
Gmail refuses to make `claude://` links clickable, so emails link here instead and this page forwards.

Published at: https://nathanielchanjack-dev.github.io/open-in-claude/

## Use

```
https://nathanielchanjack-dev.github.io/open-in-claude/?folder=/Users/nathaniel/Projects/dev-fundamentals&q=today%27s%20lesson
```

- `folder`: absolute path of the project on the Mac. Default: the dev-fundamentals course.
- `q`: text to prefill in the new session. Default: `today's lesson`.

Every scheduled agent that wants a "discuss this in Claude" link reuses this page with its own `folder` and `q`.
Nothing is stored or logged. The page builds a `claude://code/new?folder=…&q=…` link and navigates to it.
