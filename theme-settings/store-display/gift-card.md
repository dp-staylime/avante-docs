# Gift card

<figure><img src="../../.gitbook/assets/Group 18 (2).jpg" alt=""><figcaption></figcaption></figure>

The gift card page is shown to the recipient after a gift card is purchased. It automatically generates a unique code, a QR code for easy redemption, and supports adding the card to Apple Wallet.

***

### Customize the image

Go to **Theme settings → Gift card** and upload a custom image to replace the default gift card design.

**Custom image** — recommended size: 1024 × 1024 px.

***

### Important limitation

The gift card page uses a standalone Liquid template (`gift_card.liquid`) — not an OS 2.0 JSON template. Because of this:

* You **cannot** edit this page using blocks and sections in the Theme Editor
* Any structural changes beyond replacing the image require editing `gift_card.liquid` directly in the code editor

{% hint style="warning" icon="question" %}
**Need custom changes?** [Contact our support team](https://staylime.zendesk.com/hc/en-us/requests/new) — we can help with code-level customizations.
{% endhint %}

***

### Troubleshooting

<details>

<summary><strong>Gift card page appears blank</strong></summary>

If the page loads but shows no content, it's caused by a conflict with the theme's fade-in animation. The `gift_card.liquid` template uses `{% layout none %}`, so standard scripts aren't loaded — leaving the content hidden.

This requires a code-level fix. Contact our support team and we'll resolve it.

</details>

<a href="https://help.shopify.com/en/manual/products/gift-card-products" class="button primary">Shopify gift cards guide</a>
