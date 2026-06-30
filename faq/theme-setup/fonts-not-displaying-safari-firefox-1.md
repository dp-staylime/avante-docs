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

***

### How to do it:

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

You might see outdated tutorials suggesting you remove this text using Shopify's language editor (Edit default theme content).&#x20;

However, this method does not actually let you delete the link.Nuances to keep in mind:

* It only renames the link: If you try to delete the text in the language editor, Shopify will not let you leave it completely blank or will force the default text back. The most you can do is rename the link to something else.
* Manual repetition: If you use Shopify Markets, any text changes must be repeated manually for every single language your store uses.

Because of these limitations, using the Custom CSS snippet above is the only reliable way to achieve a clean, white-labeled footer.
