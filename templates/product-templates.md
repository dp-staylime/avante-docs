---
description: How to create a new product template
---

# Product templates

Use product templates to give different types of products a completely different page layout — different blocks, sections, and content structure — without affecting other products.

***

### When to use a separate template

One product template = one layout. Use multiple templates when products genuinely need different page structures:

| Example                       | Template          |
| ----------------------------- | ----------------- |
| Standard products             | `Default product` |
| Pre-order items               | `pre-order`       |
| Rings with size guide         | `rings`           |
| Clothing with fit guide video | `clothing`        |
| Bundles                       | `bundle`          |

If you only need **different content** (e.g. different size chart text per product), use metafields instead — see [How do I show different content per product?](../faq/products-and-variants/how-do-i-show-different-content-per-product.md)

***

### How to create a product template

1. In the theme editor (**Customize**), use the page selector to open **Products** > **Create template**.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-18 at 14.42.20.png" alt=""><figcaption></figcaption></figure>

2. Add **Name** in the provided field for the new template.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-18 at 14.43.43.png" alt=""><figcaption></figcaption></figure>

3. Select an existing product template to base on, then click **Create template**.

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** Any changes you make to a template apply to all products assigned to that template.
{% endhint %}

***

### How to assign a template to a product

1. Go to **Shopify Admin → Products** → open a product
2. On the right side, find **Theme template**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-18 at 14.48.58.png" alt=""><figcaption></figcaption></figure>

3. Select your template from the dropdown
4. Save

{% hint style="warning" icon="octagon-exclamation" %}
**Templates only appear here from your published live theme.** If you created a template in a \[DEV] copy or draft theme, it won't show in this dropdown. Create templates in your live theme first.
{% endhint %}

***

### Managing your templates <a href="#managing-your-templates" id="managing-your-templates"></a>

To rename or delete your template, you need to use the code editor. Editing your template file might cause issues with your online store.

#### **Rename a template**

1. From your Shopify admin, go to **Online Store** > [**Themes**](https://www.shopify.com/admin/themes)
2. Find the theme with the template that you want to rename, and then click the **...** button > **Edit code**.
3. In the code editor, find the templates folder. Click the name of the template that you want to rename, and then click **Rename file**.
4. Enter the new template name, and click **Rename file** to save.

#### **Delete a template**

1. From your Shopify admin, go to **Online Store** > [**Themes**](https://www.shopify.com/admin/themes)
2. Find the theme you want to delete a template from, and then click the **...** button > **Edit code**.
3. In the code editor, find the templates folder. Click the name of the template that you want to delete, and then click **Delete file**.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-18 at 14.55.24.png" alt=""><figcaption></figcaption></figure>

If you have any resources assigned to that template, then they are displayed with the default template until you assign a different one.
