---
hidden: true
---

# Fonts not displaying in Safari or Firefox

After updating to Avante v14, fonts may stop applying correctly in Safari and Firefox — while appearing fine in Chrome. This is a known bug in the v14 release.

***

## Why this happens

Avante v14 introduced scalable fonts built on `rem` units. The initial release contained a CSS syntax error in `snippets/font-variables.liquid` — font size calculations used division by a px-unit value (e.g. `/ 24720px`), which is invalid CSS.

Chrome accepts this non-standard syntax silently. Safari and Firefox follow the spec strictly and discard the entire CSS rule, causing all font variables to go unset.

***

## How to fix it

This requires a code-level patch to the theme. Contact our support team and we'll apply the fix to your store.

> **Note:** This bug exists in the initial v14.0.0 release. If you installed or updated after the patch was released, you may not be affected.

[Contact support →](https://staylime.zendesk.com/hc/en-us/requests/new)
