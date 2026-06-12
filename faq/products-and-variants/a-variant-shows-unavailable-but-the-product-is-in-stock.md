# A variant shows "Unavailable" but the product is in stock

"Unavailable" does not mean sold out. It means that exact combination of options does not exist in your product setup.

### How to fix this

1. Go to **Shopify Admin → Products → \[your product] → Variants**.
2. Check that every option combination you want to sell is listed.
3. Make sure each variant has inventory assigned and is active.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-12 at 11.47.53.png" alt=""><figcaption></figcaption></figure>

***

### Still showing "Unavailable"?

If your variants are set up correctly but the product still shows as unavailable, check which market you are viewing the store from.

**Example:** The same product can show differently depending on the visitor's location.

<figure><img src="../../.gitbook/assets/preview.webp" alt=""><figcaption><p><em>Hong Kong SAR → "Machine Only — Unavailable", Sold out button</em></p></figcaption></figure>

<figure><img src="../../.gitbook/assets/preview (1).webp" alt=""><figcaption><p><em>United States → "Machine Only", Add to bag button</em></p></figcaption></figure>

This happens because **Shopify** automatically **hides** or restricts products for markets **outside your configured shipping zones**, even when the product is in stock.

**To check:**

* Use the **View as** selector at the bottom of the Theme Editor to preview a different market.
* Go to **Shopify Admin → Settings → Shipping and delivery** and confirm your shipping zones cover the markets you want to sell to.
