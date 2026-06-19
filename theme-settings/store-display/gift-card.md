# Gift card

<figure><img src="../../.gitbook/assets/Group 18 (2).jpg" alt=""><figcaption></figcaption></figure>

The gift card page is shown to the recipient after a gift card is purchased. It automatically generates a unique code, a QR code for easy redemption, and supports adding the card to Apple Wallet.

<a href="https://help.shopify.com/en/manual/products/gift-card-products" class="button primary">Shopify gift cards guide</a>

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

**How to fix it:** You can easily resolve this by adding one line of code to the template.

1. Go to Shopify **Admin → Online Store → Themes**.
2. Click the **"..."** button next to your theme and select **Edit code**.
3. Open the `templates/gift_card.liquid` file.
4. Scroll to the very bottom and find the closing `</body>` tag.
5. Paste the following code exactly before the `</body>` tag: `{{ 'global.js' | asset_url | script_tag }}`
6. Click **Save**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-19 at 17.05.38.png" alt=""><figcaption></figcaption></figure>

_If you are not comfortable editing theme files, please_ [_contact our support team_](https://staylime.zendesk.com/hc/en-us/requests/new) _and we will resolve it for you!_

</details>
