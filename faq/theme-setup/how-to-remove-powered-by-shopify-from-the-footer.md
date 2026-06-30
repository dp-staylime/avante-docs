# How to remove "Powered by Shopify" from the footer

By default, Shopify adds a **"Powered by Shopify"** link to the bottom of your store's footer.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 09.54.18.png" alt=""><figcaption></figcaption></figure>

Many merchants prefer to remove it to keep their storefront completely white-labeled and focused solely on their own brand. There are two ways merchants usually try to do this, but we highly recommend the CSS method as the only way to truly remove the link.

***

### The Reliable Way: Custom CSS (Recommended)

Hiding the link via the theme's global Custom CSS is the fastest, safest, and most permanent method. Why is this the best way?

* **Targeted and Safe:** The code specifically targets the `.copyright__content` class. This means it only hides the Shopify link in your footer. If you manually add a link to Shopify in your blog posts or About Us page, those links will remain perfectly visible.
* **Works for all languages at once:** If your store is multilingual (Shopify Markets), this single CSS snippet hides the link across all languages instantly.
* **Update-safe:** It won't be overwritten during minor theme updates.

#### How to do it:

{% stepper %}
{% step %}
Open your Theme Editor (Customize).
{% endstep %}

{% step %}
Go to **Theme settings** (the gear icon on the left) → **Custom CSS**.
{% endstep %}

{% step %}
Paste the following snippet:

```css
.copyright__content a[href*="shopify.com"] { 
  display: none !important; 
}
```
{% endstep %}

{% step %}
Click **Save**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 09.59.01.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
_**Note:** Your store's copyright name and year will remain fully visible. Only the Shopify link is hidden._
{% endhint %}
{% endstep %}
{% endstepper %}

***

### Why the Native Method (Edit Default Theme Content) Fails

You might see tutorials suggesting you remove this text using Shopify's language editor (**Edit default theme content**) by entering a single space.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.18.58.png" alt=""><figcaption></figcaption></figure>

In our testing, this doesn't reliably remove the link — Shopify often forces the default text back, or the link remains visible even after saving.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.13.38.png" alt=""><figcaption></figcaption></figure>

**Other limitations of this method, even when it does work:**

* **Manual repetition:** If you use Shopify Markets, the change must be repeated manually for every single language your store uses.
* **It only works on this specific field:** there's a separate "Powered by Shopify HTML" field for your store's password-protected "Opening soon" page, which needs the same edit repeated separately.

Because of these limitations, we recommend skipping this method entirely and using the Custom CSS snippet above.

***

### Edit the theme code

If you'd rather remove the link at the code level instead of using CSS:

{% stepper %}
{% step %}
Go to **Online Store → Themes**.
{% endstep %}

{% step %}
Click the three dots (...) next to your theme → **Edit code**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.16.56.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
In the sidebar, open **Sections → footer.liquid**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.20.47.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Press `Ctrl+F` (Windows) or `Cmd+F` (Mac) and search for `powered_by_link`.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.21.49.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Delete the entire line containing that tag — it will look like `{{ powered_by_link }}`.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-30 at 10.23.56.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Click **Save**.
{% endstep %}
{% endstepper %}

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** This directly edits a core theme file. It will be overwritten on the next theme update, and you'll need to re-apply it manually. The CSS method above doesn't have this problem — use it whenever possible.
{% endhint %}

***

### Related

[Shopify: Remove "Powered by Shopify" message](https://help.shopify.com/en/manual/online-store/themes/customizing-themes/common-customizations/remove-powered-by-shopify-message) — official guide
