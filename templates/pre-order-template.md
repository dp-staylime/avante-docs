# Pre-order template

Switch a product to pre-order mode — the Add to Cart button automatically changes to "Pre-order" and customers can place orders before the product is in stock.

---

## How it works

Avante includes a built-in `pre-order` product template. When a product is assigned to this template, the buy button label changes from "Add to cart" to "Pre-order". No app or code changes required.

---

## Step 1: Assign the pre-order template to a product

1. Go to **Shopify Admin → Products** → open the product
2. On the right side, find **Theme template**
3. Select **pre-order** from the dropdown
4. Save

`[SCREENSHOT: Product page in Shopify Admin, правая панель з Theme template dropdown → pre-order вибрано]`

> ⚠️ The pre-order template only appears in the dropdown from your **published live theme**. If you don't see it, make sure you're editing the live theme — not a [DEV] copy.

---

## Step 2: Add delivery information (recommended)

Let customers know when to expect their order. Add a Collapsible tab block with estimated shipping dates:

1. Open **Theme Editor → Default pre-order template**
2. Inside **Product overview** section, click **Add block → Collapsible tab**
3. Set the tab name — e.g. `Expected delivery`
4. Enter your delivery estimate in the Content field — e.g. `Ships in 4–6 weeks. You will receive a confirmation email when your order ships.`

`[SCREENSHOT: Theme Editor з pre-order template, Collapsible tab блок з delivery info]`

---

## Step 3: Add a countdown timer (optional)

Create urgency by showing a countdown to the pre-order end date:

1. Inside **Product overview** section, click **Add block → Countdown timer**
2. Set the end date and time
3. Choose what happens when the timer ends: hide the block or show a custom message

---

## How to revert a product back to normal

When the product is in stock and ready to ship:

1. Go to **Shopify Admin → Products** → open the product
2. Change **Theme template** back to **Default product**
3. Save

The buy button will return to "Add to cart" immediately.

---

## Customizing the pre-order template layout

The pre-order template is independent from the Default product template. You can customize its sections and blocks without affecting regular product pages:

1. Open **Theme Editor**
2. At the top, switch to **pre-order** template
3. Add, remove, or reorder blocks as needed

> **Tip:** Consider adding a prominent notice about pre-order terms near the top of the page — use a **Text** block or **Callout** block in the Product overview section.

---

## Related

- [Product templates](product-templates.md)
- [How do I show different content per product?](../faq/different-content-per-product.md)
