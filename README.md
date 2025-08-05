# 💥 ACCEPTCEPTION.JS 💥

**Tired of cookie banners? So are we.**

Deploy acceptception.js on your site and turn the tables on the GDPR architects

[Live Demo Here](https://redpepperdev.github.io/acceptception-demo/?acceptception_test=true)

<div style="text-align: center;">
    <img src="https://raw.githubusercontent.com/redpepperdev/acceptception/main/acceptception.png" alt="Acceptception Banner" style="max-width: 100%; height: auto;">
</div>

Do you have eyes and use the internet? Then you've felt the pain. The endless, soul-crushing, mind-numbing tyranny of the cookie consent banner! A "solution" so elegant, so user-friendly, it could only have been designed by a committee of bureaucrats with a deep-seated hatred for the internet.

We've had enough. The cookie accept must end.

## The Solution

`acceptception.js` is our answer. It's a weapon of malicious compliance, designed to give the regulators a taste of their own medicine. This script will unleash an endless barrage of pop-ups, impossible-to-click buttons, and absurdly long terms of service on the very people who brought this plague upon us. It's about sending a message.

## How It Works

The script is simple. It detects if a user is visiting from an IP address associated with a European regulatory body and, if so, unleashes the chaos. For everyone else, it does nothing.

## Join the Resistance

1.  Add `acceptception.js` to your website.
2.  Include this script tag:
    ```html
    <script src="https://cdn.jsdelivr.net/gh/redpepperdev/acceptception@main/acceptception.js"></script>
    ```
3.  Watch the fun begin.

## Testing

To verify that `acceptception.js` is working on your site without affecting real users, you can simulate a blacklisted IP using the URL query parameter `?acceptception_test=true`. This triggers the script's behavior (modals and event listeners) as if the visitor's IP were blacklisted.

### Steps to Test

- **Enable Test Mode**: Load your site with the query parameter, e.g., `https://your-site.com?acceptception_test=true`.
- **Verify Initial Modal**: The initial cookie consent modal should appear immediately upon page load.
- **Test Interactions**: Interact with the page (e.g., scroll, click, or type) to trigger additional modals, confirming that event listeners are active.
- **Disable Test Mode**: Remove the query parameter (e.g., `https://your-site.com`) and reload the page to ensure no modals appear for non-blacklisted IPs.
- **Check Console Logs**: Open Developer Tools (F12) and check the Console tab for debug logs like `[AcceptAccept Debug]: Test mode enabled via query parameter (?acceptception_test=true).` or `[AcceptAccept Debug]: IP <your-ip> is not blacklisted`.

### Example

- **With Test Mode**: `https://example.com?acceptception_test=true` → Modals appear.
- **Without Test Mode**: `https://example.com` → No modals.

## Play with the Demo
- Visit the live demo: [https://redpepperdev.github.io/acceptception-demo/?acceptception_test=true](https://redpepperdev.github.io/acceptception-demo/?acceptception_test=true)
- Interact with the page (e.g., scroll, click) to trigger additional modals.

### Notes

- Ensure your browser and any server/CDN caches are cleared to avoid loading an outdated script. You can add a cache-busting query string to the script tag, e.g., `<script src=".../acceptception.js?v=1"></script>`.
- If modals don’t appear as expected, check the console for errors like `[AcceptAccept Error]: Failed to fetch IP`.
- The script requires internet access to fetch the visitor’s IP via `api.ipify.org` or `api.seeip.org`.

**Disclaimer:** This is satire. Or is it?
