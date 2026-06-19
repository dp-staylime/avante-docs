---
description: >-
  A guide to customize the typography for your store to match your brand and
  improve readability.
---

# Typography

Select fonts and typography presets to match your brand identity.

<figure><img src="../.gitbook/assets/Group 9.jpg" alt=""><figcaption></figcaption></figure>

***

### Typography preset

Avante ships with 9 built-in presets. Each preset defines a combination of Base and Accent fonts with pre-configured sizes.

| Preset                | Description                                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **Minimal uppercase** | Uses Base font only, uppercase styling.                                                                                                     |
| **Minimal basic**     | Uses Base font only, clean minimal style.                                                                                                   |
| **Minimal heavy**     | Uses Base font only, heavier weight.                                                                                                        |
| **Classic**           | Combination of Base and Accent fonts, traditional look.                                                                                     |
| **Avant-garde**       | Combination of Base and Accent fonts, contemporary styling.                                                                                 |
| **Contrast**          | Combination of Base and Accent fonts, high contrast between body and headings.                                                              |
| **Brutalist**         | Combination of Base and Accent fonts, bold editorial style.                                                                                 |
| **Duet**              | Combination of Base and Accent fonts, balanced pairing.                                                                                     |
| **Custom**            | Full granular control over every individual text style. See [Custom typography preset](custom-typography-preset.md) for all settings (v11). |

**Swap base and accent fonts** — toggle to invert which font is used for body text and headings.

{% hint style="success" icon="lightbulb" %}
**Tip:** Start with a preset close to your brand, then switch to Custom if you need fine-tuned control over individual text styles.
{% endhint %}

***

### Base

Used for body text throughout the store.

| Setting              | Description                                              |
| -------------------- | -------------------------------------------------------- |
| **Font**             | Select the base font from Shopify's font library.        |
| **Base icon weight** | Weight for icons displayed alongside base font elements. |

***

### Accent

Used for headings and titles.

| Setting                | Description                                                |
| ---------------------- | ---------------------------------------------------------- |
| **Font**               | Select the accent font from Shopify's font library.        |
| **Accent icon weight** | Weight for icons displayed alongside accent font elements. |

***

### Secondary

Used for supporting text elements where a third font variation is needed.

| Setting  | Description                                            |
| -------- | ------------------------------------------------------ |
| **Font** | Select the secondary font from Shopify's font library. |

{% hint style="success" icon="sparkles" %}
**Tip:** To apply the Secondary heading style to a specific word anywhere in a text block, wrap it in {curly brackets} — e.g. `AVANTE—{BEYOND} THE ORDINARY`. The bracketed word will use the Secondary font defined here.
{% endhint %}

<figure><img src="../.gitbook/assets/Group 10 (2).jpg" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**Adding fonts affects store performance.** Each additional font loads extra files. Stick to 1–2 fonts where possible. See [Shopify's font speed guide](https://help.shopify.com/en/manual/online-store/store-speed/improving-speed#fonts).
{% endhint %}

***

### Custom fonts

Upload your own brand fonts in WOFF or WOFF2 format.

**Enable custom fonts** — toggle to activate custom font upload.

Once enabled, follow the [Shopify custom fonts guide](https://shopify.dev/docs/themes/architecture/settings/fonts#custom-fonts) to upload your font files to the theme assets.

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** Only WOFF and WOFF2 formats are supported.
{% endhint %}

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** Adding custom fonts requires uploading font files to the theme code and adding `@font-face` declarations — it's a code-level task. If you need help, [contact our support team](https://staylime.zendesk.com/hc/en-us/requests/new).
{% endhint %}

See also: [Can I use custom fonts?](../faq/theme-setup/can-i-use-custom-fonts.md)
