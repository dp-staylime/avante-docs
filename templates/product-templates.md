# Product templates

Use product templates to give different types of products a completely different page layout — different blocks, sections, and content structure — without affecting other products.

---

## When to use a separate template

One product template = one layout. Use multiple templates when products genuinely need different page structures:

| Example | Template |
|---------|----------|
| Standard products | `Default product` |
| Pre-order items | `pre-order` |
| Rings with size guide | `rings` |
| Clothing with fit guide video | `clothing` |
| Bundles | `bundle` |

If you only need **different content** (e.g. different size chart text per product), use metafields instead — see [How do I show different content per product?](../faq/different-content-per-product.md)

---

## How to create a product template

1. Open **Theme Editor**
2. At the top, click the template name (**Default product**)
3. Click **Create template**
4. Enter a name — e.g. `rings`, `clothing`, `bundle`
5. Click **Create**

The new template starts as a copy of Default product. Customize its blocks and sections independently.

> **Note:** Any changes you make to a template apply to all products assigned to that template.

---

## How to assign a template to a product

1. Go to **Shopify Admin → Products** → open a product
2. On the right side, find **Theme template**
3. Select your template from the dropdown
4. Save

> ⚠️ **Templates only appear here from your published live theme.** If you created a template in a [DEV] copy or draft theme, it won't show in this dropdown. Create templates in your live theme first.

---

## How to delete a product template

Deleting a template is not possible from the Theme Editor UI. It requires editing the theme code directly.

1. Go to **Shopify Admin → Online Store → Themes**
2. Next to your live theme, click **...** → **Edit code**
3. In the left panel, open the **Templates** folder
4. Find the template file — e.g. `product.rings.json`
5. Click the file → click **Delete file**

> ⚠️ **Make a backup before deleting.** Deleted code cannot be recovered. If you're not confident with code, contact Shopify Support or reach out to us.

> **Note:** Products assigned to a deleted template automatically revert to the Default product template.

---

## Related

- [How do I show different content per product?](../faq/different-content-per-product.md)
- [Pre-order template](pre-order-template.md)
- [Templates overview](README.md)
