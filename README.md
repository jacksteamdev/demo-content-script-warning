# Demo Content Script Warning

This repo demonstrates what happens when you add a content script to an extension that is published on the Chrome Web Store.

Warnings for new content scripts or content script match patterns are not documented in Google's Chrome extension docs.

## Hypothesis

Our supposition is:

- Given that an extension is published on the Chrome Web Store
  - and a user has installed that extension
- when you add a content script that matches a broader range of urls
- then Chrome will require the user to approve these changes

We will conduct an experiment to verify this, following these steps after each iteration:

## Method

1. Pack and install the extension using the Chrome extensions dashboard
2. Document the warnings

### Iterations

1. Create a simple extension with no content scripts
2. Add a content script with narrow host permissions
3. Broaden the content script host permissions
4. Add a second content script with host permissions for all urls

## Results



