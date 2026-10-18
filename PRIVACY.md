# Privacy Policy — AI Text Explainer

Last updated: 2026 (initial 1.0.0 release)

This privacy policy explains how the **AI Text Explainer** browser extension
("the extension") handles information. It applies only to this extension.

## Summary

AI Text Explainer is a "bring your own key" (BYOK) tool. You supply your own
OpenRouter API key, and the extension uses it to send the text you want
explained directly to OpenRouter. The developer of this extension does not
operate a server for these requests and does not receive your API key or your
text.

## Information the extension handles

### 1. Your OpenRouter API key
- You enter your own API key on the extension's Settings page.
- The key is stored locally on your device using the Chrome extension storage
  API (`chrome.storage.local`).
- Access to this stored value is restricted to the extension's own trusted
  contexts (the background service worker and extension pages). Content scripts
  and web pages cannot read it.
- The key is used only by the extension's background service worker to
  authenticate requests to OpenRouter.
- The developer never receives your API key. It is not sent anywhere except to
  OpenRouter as the authentication credential for your own requests.
- You can remove the saved key at any time from the Settings page.

### 2. The text you choose to explain
- When you use the extension, the text you paste into the popup or highlight on
  a page before choosing "Explain with AI" is sent to OpenRouter to generate an
  explanation.
- This text is sent directly from your browser to OpenRouter. It is not routed
  through, stored on, or collected by any developer-operated server, because
  this extension does not use one.

## Third-party processing

Requests are sent to **OpenRouter** (openrouter.ai), which forwards them to the
model provider you are using (currently a DeepSeek model). Your API key and the
text you submit are handled by OpenRouter and its upstream providers according
to their own privacy policies and terms. You should review OpenRouter's
documentation and policies to understand how they process data. The developer
of this extension does not control and is not responsible for how OpenRouter or
its upstream providers handle your data.

## What the extension does NOT do

- It does not include or use a developer-owned API key.
- It does not send your data to the developer.
- It does not use analytics, tracking, or advertising.
- It does not sell or share your information.
- It does not access web page content except the specific text you choose to
  explain, and only when you explicitly trigger the feature.

## Data storage and retention

- The only information the extension stores on your device is your OpenRouter
  API key (and only if you choose to save it).
- The extension does not build a history of your explanations.
- Removing the key in Settings deletes it from local extension storage.
- Uninstalling the extension removes its local storage.

## Clipboard

The optional "Copy" buttons copy the generated explanation to your system
clipboard. This happens locally and is controlled by your operating system.

## Notable limitations

Because your text is transmitted to OpenRouter to produce an explanation, this
extension does transmit data off your device when you use it. Treat the
highlighted or pasted text as data that leaves your browser and reaches a
third party. Do not use the extension on text you are not permitted to send to
a third-party service.

## Children's privacy

This extension is not directed at children and is not intended for use by
children.

## Changes to this policy

This policy may be updated if the extension's behavior changes. The "Last
updated" date above will change accordingly.

## Contact

For questions about this extension, please use the support contact information
listed on the extension's Chrome Web Store listing.
