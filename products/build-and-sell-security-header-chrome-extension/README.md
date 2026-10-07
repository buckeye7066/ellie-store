# Build and sell security-header Chrome extension

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/cNidRa1aK8bH5h19wPawo1s) · delivered as a Markdown file you can import or edit.

Security Header Scanner Chrome Extension - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# Security Header Scanner Chrome Extension

## Files
- manifest.json
- background.js
- popup.html
- popup.js
- styles.css
- LICENSE
- README.md
- icons/icon16.svg
- icons/icon32.svg
- icons/icon48.svg
- icons/icon128.svg

---

manifest.json
```json
{
  "manifest_version": 3,
  "name": "Security Header Scanner",
  "description": "Scan the current page for missing security headers and generate a report.",
  "version": "1.0.0",
  "action": {
    "default_title": "Security Header Scanner",
    "default_popup": "popup.html",
    "default_icon": {
      "16": "icons/icon16.svg",
      "32": "icons/icon32.svg",
      "48": "icons/icon48.svg",
      "128": "icons/icon128.svg"
    }
  },
  "permissions": [
    "webRequest",
    "webRequestBlocking",
    "<all_urls>",
    "storage"
  ],
  "host_permissions": [
    "<all_urls>"
  ],
  "background": {
    "service_worker": "background.js",
    "type": "module"
  },
  "icons": {
    "16": "icons/icon16.svg",
    "32": "icons/icon32.svg",
    "48": "icons/icon48.svg",
    "128": "icons/icon128.svg"
  }
}
```

---

background.js
```javascript
// Security Header Scanner - background script
// Captures response headers for main-frame requests and stores them per tab.

const REQUIRED_HEADERS = [
  "content-security-policy",
  "x-content-type-options",
  "x-frame-options",
  "strict-transport-security",
  "referrer-policy",
  "permissions-policy",
  "x-xss-protection"
];

function parseHeaders(headerArray) {
  const headers = {};
  for (const { name, value } of headerArray) {
    headers[name.toLowerCase()] = value.trim();
  }
  return headers;
}

chrome.webRequest.onHeadersReceived.addListener(
  (details) => {
    // Only care about main frame
    if (details.type !== "main_frame") return;
    const headers = parseHeaders(details.responseHeaders);
    // Store under a key unique to the tab
    chrome.storage.local.set({ [`headers-${details.tabId}`]: headers });
  },
  { urls: ["<all_urls>"], types: ["main_frame"] },
  ["responseHeaders"]
);
```

---

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/cNidRa1aK8bH5h19wPawo1s)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
