# Copy of Frequently asked questions

### Theme setup

<details>

<summary><strong>What's the difference between Adelle, Bloop, Fairmont, Vortex, and Avante?</strong></summary>

Fairmont, Vortex, Adelle, Bloop, and Avante are not separate themes that you need to purchase individually. They are simply built-in style presets (theme styles) included within the Avante theme.You can easily switch between these presets to instantly change the overall look and feel of your store.

How to switch between presets:

1. Open your **Theme Editor** (Edit theme).
2. Click on the Theme settings icon (**gear icon**) on the left sidebar.
3. Scroll down and click on **Theme style**.
4. Select the preset you want to apply (e.g., Adelle, Bloop, etc.).

<figure><img src="../.gitbook/assets/Screenshot 2026-06-08 at 17.17.49.png" alt=""><figcaption></figcaption></figure>

_**Note**: Switching presets updates the visual settings (colors, fonts, etc.), but Shopify does not automatically apply the full demo content structure._&#x20;

_If you want to start with the exact setup shown in one of our demos, it is best to install that specific preset fresh directly from the Shopify Theme Store._

</details>

<details>

<summary><strong>My theme settings reset after an update — what happened?</strong></summary>

When updating your theme, you might notice that your visual settings (colors, fonts, section layouts) have disappeared. This is standard Shopify platform behavior that depends on the type of update you are installing.&#x20;

**Major vs. Minor Updates:**

* **Minor/Patch updates** (e.g., from v13.0.0 to v13.0.1): Shopify’s automated update process will smoothly transfer all your visual settings and layouts without any data loss.
* **Major updates** (e.g., from v13.0.x to v14.0.0): These updates contain significant architectural changes to the theme's core files. Because the internal structure changes, Shopify cannot automatically transfer your Theme Editor settings, and they are reset to defaults.

**What transfers automatically during a Major Update?**

* All content managed in your Shopify Admin remains perfectly safe (Products, Collections, Pages, Blog posts, Navigation menus).

**How to fix this:** After a major update, you will need to manually reconfigure your settings (colors, fonts, and section blocks) in the Theme Editor to match your previous design.

</details>

***

### A page template isn't showing in the Shopify Admin dropdown

Shopify only shows templates from your **currently published (live) theme** in the Admin dropdown. Templates created in a draft theme don't appear there.

**Fix:** Create the template in your live theme first (**Theme Editor → Pages → Create template**), then assign it to your page in Shopify Admin.

***

### How do I create a FAQ page with expandable questions?

1. Go to **Shopify Admin → Online Store → Pages** → Create a new page
2. Assign it to the **FAQ template** (create it first in Theme Editor if needed)
3. In **Theme Editor → Pages → FAQ template**, add a **Collapsible tabs** section
4. Fill in your questions and answers as tab items

***

### Can I use custom fonts?

Shopify's native font picker only supports fonts from the Shopify/Google font library.

To use your own WOFF/WOFF2 files, it requires uploading font files to your Assets folder and writing `@font-face` rules in `custom-styles.css`. This is a code task — contact us if you'd like us to handle it ($80/hour, approx. 1 hour).

***

## Navigation

### Mega menu isn't working / dropdowns won't open

The **Dropdown link** field in the Mega menu block must exactly match the menu item name in **Shopify Admin → Online Store → Navigation** (e.g. `Collections`).

> ⚠️ Do not translate this field using Translate & Adapt — it's an internal reference, not visible text.

***

### How do I create nested / dropdown menus?

Menu nesting is set in **Shopify Admin**, not the Theme Editor:

1. Go to **Shopify Admin → Online Store → Navigation**
2. Open the menu you want to edit
3. Drag items slightly to the right under a parent item to create submenus (up to 3 levels)
4. Save

The theme will automatically render the nesting as dropdowns or a Mega menu depending on your Header settings.

***

### Transparent header isn't working

Two settings must be active at the same time:

1. **Theme settings → Navigation** → enable **Allow transparent navigation**
2. Open the first section on your page (Slideshow or Image banner) → set **Section width → Overlap by navigation**

If only one is enabled, the effect won't appear. See [Transparent header](../features/transparent-header.md) for the full guide.

***

### On mobile, tapping a parent menu item navigates away instead of expanding the submenu

This is the default behavior — tap the arrow to expand, tap the text to navigate.

To disable navigation on the parent item, add one line of CSS to **Theme settings → Custom CSS**:

```css
.link-[your-item-name] {
  pointer-events: none;
}
```

Find the exact class name via browser DevTools → Elements → find the `<a>` tag of the menu item → look for `link-[name]` in its class attribute.

***

## Products & variants

### Variant images aren't switching when I select a color

1. In **Theme Editor → Products → Product overview section**, make sure **"Show the first image instead of the variant's"** is **unchecked**
2. If using **"Show only media of selected variant"**, add the variant name in brackets to each image's Alt text in Shopify Admin — e.g. `(Red)`, `(Blue)`

***

### How do I add a Pre-order button?

1. Go to **Shopify Admin → Products** → select the product
2. Scroll to **Theme template** on the right
3. Change from `Default product` to `pre-order`
4. Save — the button automatically changes to "Pre-order"

***

### How do I show color swatches and a short description on collection cards?

**Color swatches:** Theme Editor → Collection template → Product grid section → enable **"Enable color pills"**

**Short description:** Requires setting up the Product subtitle metafield — see [Product subtitle](../features/product-subtitle.md) for the full guide.

***

### A variant shows "Unavailable" but the product is in stock

"Unavailable" means that specific combination of options hasn't been created in your product setup — it's different from "Sold out."

Go to **Shopify Admin → Products → \[product] → Variants** and check that all combinations you want to offer are listed with inventory assigned.

Also check: if you're testing from a country outside your store's shipping zones, Shopify shows products as unavailable. Test with a VPN set to your target market.

***

### Quick View / Quick Add buttons aren't visible on mobile

These buttons appear on hover by default. Since mobile devices don't have a hover state, they're hidden to keep the grid clean.

To make them permanently visible on mobile, add a CSS snippet to **Theme settings → Custom CSS**. Contact us if you need help with this.

***

## Performance

### My store is loading slowly

The theme itself is rarely the cause. Most common culprits:

* **Large images or videos** — compress images to under 500 KB, videos to 2–5 MB
* **Third-party app scripts** — loyalty programs, chat widgets, tracking pixels each add JavaScript that loads on every page
* **Too many active apps** — disable apps you don't actively use

Always test your live store in incognito mode at [PageSpeed Insights](https://pagespeed.web.dev/). Preview links bypass Shopify's CDN cache and always show lower scores.

***

### The Checkout button is slow or unresponsive

Almost always caused by third-party scripts blocking the browser's main thread — not the theme.

Check: **Settings → Customer Events** and remove any unused tracking pixels. Common culprits: Klarna, Omnisend, loyalty app pixels. Note that disabling an app doesn't automatically remove its Web Pixel — you must delete it manually from Customer Events.

***

## Shopify platform limitations

### Can I customize the checkout page?

The checkout page is managed entirely by Shopify. Customization beyond basic branding (logo, colors) is only available on **Shopify Plus** via Checkout Extensibility.

For standard plans: **Shopify Admin → Settings → Checkout → Branding**.

***

### Can I add a wishlist?

Wishlist functionality requires saving data to a user account, which needs database access. This is not permitted in Shopify themes per the Shopify Theme Store requirements.

Recommended apps:

* [Wishlist Plus](https://apps.shopify.com/swym-relay) by Swym
* [Growave](https://apps.shopify.com/growave) (wishlist + reviews + loyalty)

Both integrate with Avante.

***

## Licensing

### Can I use Avante on a staging store?

Per Shopify's licensing policy, one purchase covers one store. Using the theme on a second store (including staging) creates an unlicensed installation.

Acceptable staging approach: use a **password-protected** duplicate of your store. Keep it private (password enabled at all times).

***

### How do I transfer Avante to a new store?

1. Purchase a fresh license on the new store from the Shopify Theme Store
2. Contact **Shopify Support** and ask for a refund on the original store's purchase (Shopify handles all licensing and billing)

You cannot transfer a license directly — Shopify manages this process.
