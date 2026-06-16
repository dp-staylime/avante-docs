# How do I set up Linked Products?

Linked Products let you connect separate products and display them as color swatches on the product page — instead of using standard Shopify variants.

This is useful when you want to:

* Show each color as a separate product on Collection pages
* Display only the images of the selected color in the gallery

For the full setup guide see [Linked Products →](../../features-and-advanced-setup/linked-products.md)

***

### Common questions

<details open>

<summary><strong>How do I show color circles instead of product photos?</strong></summary>

By default, swatches display the first image of each linked product. To show solid color circles or custom images instead, create additional metafields:

1. Go to **Shopify Admin → Settings → Metafields and metaobjects → Products**
2. Click **Add definition** and create the metafields you need:

**For color circles:**

* Name: `Linked color`
* Namespace and key: `custom.linked_color`
* Type: **Color picker** — One value

**For a custom image:**

* Name: `Linked image`
* Namespace and key: `custom.linked_image`
* Type: **File** — One file

3. Open each product → scroll to **Product metafields**
4. Fill in the **Linked color** or **Linked image** field
5. Repeat for every product in the group

</details>

<details>

<summary><strong>How do I control the order of swatches?</strong></summary>

The swatch order is set by the order of products **inside the `custom.linked_products` metafield** — not in the Variants section.

1. Open a product → scroll to **Product metafields**
2. Find the **Linked products** field
3. Drag the products into the order you want

> ⚠️ You need to set the order separately on **each product** in the group. The order is not synced automatically.

</details>

<details>

<summary><strong>How do I make swatches circular?</strong></summary>

1. Go to **Theme Editor → Theme settings → Variant selector**
2. Scroll down to **Linked products**
3. Adjust the **Corner radius** to your preferred shape

</details>
