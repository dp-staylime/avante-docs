# A page template isn't showing in the Shopify Admin dropdown

If you created a new page template in the Theme Editor but can't find it when assigning it to a page in Shopify Admin, this is standard Shopify behavior.

{% hint style="success" icon="sparkles" %}
The template dropdown in Shopify Admin only shows templates that exist in your currently **published (Live) theme**. Templates created in a draft theme are not visible there.
{% endhint %}

### How to fix this:

1. Go to **Shopify Admin → Online Store → Themes**
2. Click **Edit theme** on your **Live theme**
3. Open the top dropdown → go to **Pages** → click **Create template**
4. Name it exactly as needed (e.g. `FAQ`)

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-10 at 17.37.18.png" alt=""><figcaption></figcaption></figure>

5. Exit the Theme Editor and go to **Shopify Admin → Online Store → Pages**
6. Open your page and assign it to the new template in the **Template** dropdown on the right

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-10 at 17.39.39.png" alt=""><figcaption></figcaption></figure>

7. Go back to your **draft Avante theme** and create the same template there — it will now be properly linked

{% hint style="warning" icon="triangle-exclamation" %}
**Important:** Always create new templates in your Live theme first.

That's the only way they appear in the Shopify Admin dropdown.
{% endhint %}
