# Content Script Warning Demonstration

This repo demonstrates what happens when you add a content script to an extension that is published on the Chrome Web Store.

Warnings for new content scripts or content script match patterns are not documented in Google's Chrome extension docs.

## Hypothesis

Our supposition is:

- Given that an extension is published on the Chrome Web Store
  - and a user has installed that extension
- When you add a content script that matches a broader range of urls
- Then Chrome will require the user to approve these changes

We will conduct an experiment to verify this, following this method after each iteration:

## Method

1. Pack and install the extension using the Chrome extensions dashboard
2. Document the warnings

## Iterations

1. Create a simple extension with a content script with narrow host permissions
2. Broaden the content script host permissions
3. Add a second content script with host permissions for all urls

## Results

Our supposition was correct. After each update, the extension was disabled and Chrome displayed a warning with the new permissions, requiring user consent before re-enabling the extension.

### Step 1 Warning Image

![Step 1 Warning Image](https://raw.githubusercontent.com/jacksteamdev/demo-content-script-warning/blob/master/pngs/step1.png)

### Step 2 Warning Image

![Step 2 Warning Image](https://raw.githubusercontent.com/jacksteamdev/demo-content-script-warning/blob/master/pngs/step2.png)

### Step 3 Warning Image

![Step 3 Warning Image](https://raw.githubusercontent.com/jacksteamdev/demo-content-script-warning/blob/master/pngs/step3.png)
