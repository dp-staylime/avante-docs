# Fonts not displaying in Safari or Firefox

After updating to Avante v14, fonts may appear different in Safari and Firefox — headings and body text revert to system defaults — while appearing fine in Chrome.

***

### How to check if you're affected

Open your store in **Safari or Firefox** and compare with Chrome. If fonts look unstyled or generic — you're affected.

***

### Why this happens

Avante v14 introduced scalable fonts built on `rem` units. The initial release contains a CSS syntax error in `snippets/font-variables.liquid` — font size calculations divide by a px-unit value (e.g. `/ 24720px`), which is invalid CSS.

Chrome accepts this silently. Safari and Firefox follow the spec strictly and discard the entire rule — causing all font variables to stop applying.

***

### How to fix it

This requires a code-level patch — it cannot be resolved by changing theme settings or updating to a newer version at this time.

**Contact our support team** and we'll apply the fix to your store:

<a href="https://staylime.zendesk.com/hc/en-us/requests/new" class="button primary">Contact support →</a>

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** This bug exists in the initial v14.0.0 release. If you installed or updated after the patch was released, you may not be affected.
{% endhint %}
