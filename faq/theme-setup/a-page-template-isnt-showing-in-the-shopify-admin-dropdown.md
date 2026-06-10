# A page template isn't showing in the Shopify Admin dropdown

If you created a new page template in the Theme Editor (e.g., `FAQ` or `About Us`) but cannot find it in the Shopify Admin when trying to assign it to a page, this is due to how Shopify handles unpublished themes.

{% hint style="success" icon="sparkles" %}
The template dropdown in the Shopify Admin only displays templates that **exist in your currently published (Live) theme**.&#x20;
{% endhint %}

If you are customizing Avante as a draft (unpublished) theme, the new templates will be hidden.&#x20;

### How to fix this:

1. Go to your Live theme in Shopify Admin → Online Store → Themes.
2. Click Customize on the Live theme.
3. Use the top dropdown menu, go to Pages, and click Create template. Name it exactly as you need (e.g., `FAQ`). `[Вставить скриншот: Theme Editor Live-темы -> Создание пустого шаблона]`
4. Exit the Theme Editor and go to Shopify Admin → Pages.
5. Select your page and assign it to the newly created template. It will now appear in the dropdown. `[Вставить скриншот: Shopify Admin -> Настройки страницы -> Выбор шаблона]`
6. Finally, go to your working (Draft) Avante theme and create the exact same template there. It will now be properly linked!

Shopify only shows templates from your **published theme** in the Admin dropdown.

Templates created in a draft theme do not appear there.

### Fix

1. Open **Theme Editor** for your live theme.
2. Go to **Pages**.
3. Click **Create template**.
4. Return to **Shopify Admin → Online Store → Pages**.
5. Assign that template to the page.
