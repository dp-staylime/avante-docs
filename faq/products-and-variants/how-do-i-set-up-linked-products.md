# How do I set up Linked Products?

Linked Products let you connect separate products and display them as color swatches on the product page — instead of using standard Shopify variants.

This is useful when you want to:

* Show each color as a separate product on Collection pages
* Display only the images of the selected color in the gallery

***

### Common questions

<details open>

<summary><strong>How do I show color circles instead of product photos?</strong></summary>

By default, Linked Products shows product thumbnails. To show solid color circles, create an additional metafield on your products:

* Namespace and key: `custom.linked_color`
* Type: **Color picker**

Then assign a color to each product in that metafield.

</details>

<details>

<summary><strong>How do I control the order of swatches?</strong></summary>

The order is set by dragging items within the `custom.linked_products` metafield itself — not in the Variants section. You need to set the order separately on each product in the group.

</details>

<details>

<summary><strong>How do I make swatches circular?</strong></summary>

Go to **Theme settings → Variant selector → Linked products** and adjust the **Corner radius** setting.

</details>

***

For the full setup guide see:

{% content-ref url="../../features-and-advanced-setup/linked-products.md" %}
[linked-products.md](../../features-and-advanced-setup/linked-products.md)
{% endcontent-ref %}
