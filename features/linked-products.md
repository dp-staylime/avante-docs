---
description: Set up linked products for related variants or products.
---

# Linked Products

Linked Products let you connect separate products and display them as color swatches on the product page. This is useful when you want to:

* Show each color as a separate product on Collection pages
* Display only the images of the selected color in the product gallery

***

### Step 1 — Create the metafield

1. Go to **Shopify Admin → Settings → Metafields and metaobjects → Products**
2. Click **Add definition**
3. Fill in the fields exactly as shown:
   * **Name:** `Linked products`
   * **Namespace and key:** `custom.linked_products`
   * **Type:** Product — List of products
4. Save

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 12.10.52.png" alt=""><figcaption></figcaption></figure>

***

### Step 2 — Link products together

1. Go to **Shopify Admin → Products → \[your product]**
2. Scroll down to **Product metafields**
3. Find **Linked products** and select all the products in the same color group
4. **Include the current product itself** — this makes it appear first and look selected when a customer views that product
5. Save
6. Repeat for every product in the group

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 12.24.20.png" alt=""><figcaption></figcaption></figure>

***

### Step 3 — Add the block in Theme Editor

1. Go to **Theme Editor → Products → Default product template**
2. Inside the **Product overview** section click **Add block → Linked products**
3. Save

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 12.29.40.png" alt=""><figcaption></figcaption></figure>

***

### Step 4 — Adjust the design

1. In Theme Editor go to **Theme settings → Variant selector**
2. Scroll down to **Linked products**
3. Adjust **Image ratio**, **Focal point**, **Corner radius** and **Shadow** to match your store design

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 12.31.29.png" alt=""><figcaption></figcaption></figure>

***

{% hint style="warning" icon="triangle-exclamation" %}
Each product in the group must have the metafield filled in — including the current product itself. If any product is missing it, its swatch won't appear on the other products' pages.
{% endhint %}

{% hint style="danger" icon="octagon-exclamation" %}
Linked Products requires each color to be a **separate product** in your catalog. If your colors currently exist as variants within one product, you will need to create individual products for each color first. This is a significant catalog restructuring — consider this before getting started.
{% endhint %}
