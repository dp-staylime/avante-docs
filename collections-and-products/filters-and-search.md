# Filters & search

### Setting up filters

In Shopify OS 2.0 themes like Avante, adding variants or tags to your products doesn't make filters appear automatically on collection pages. Filtering is managed centrally through Shopify's native Search & Discovery app.

{% stepper %}
{% step %}
Install the free [**Search & Discovery**](https://apps.shopify.com/search-and-discovery) app from the Shopify App Store.
{% endstep %}

{% step %}
Go to the app → **Filters** → click **Add filter** (you can choose availability, price, vendor, product type, or specific metafields).

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 14.54.11.png" alt=""><figcaption></figcaption></figure>

Once added, filters will automatically appear on your collection and search pages. For more details, see [Shopify's official guide on search and discovery filters](https://www.google.com/url?sa=E\&q=https%3A%2F%2Fhelp.shopify.com%2Fen%2Fmanual%2Fonline-store%2Fstorefront-search%2Fsearch-and-discovery-filters).

{% hint style="warning" icon="lightbulb" %}
**Good to know:** Shopify natively hides a filter if your products lack variation. For example, if all products in a collection only come in size "M", the Size filter won't display because selecting it wouldn't filter anything out.
{% endhint %}
{% endstep %}
{% endstepper %}

***

### Changing the filter layout

You can choose how filters are presented on the page (as a sidebar, a top bar, or a slide-out drawer). To change this:

1. Open Theme Editor and navigate to the **Default collection** template.
2. Click on the **Collection page** (or Product grid) section.
3. Find the **Desktop filter style** setting and choose between **Horizontal**, **Vertical**, or **Drawer**.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 16.10.52.png" alt=""><figcaption></figcaption></figure>

***

### Filter swatches

To make your filters more visual, you can display color or material options as visual swatches or image thumbnails instead of standard checkboxes.

1. Go to **Theme settings** → **Filter swatches**.
2. Under **Color swatches** or **Thumbnail swatches**, enter the exact name of your filter option (e.g., `Color`, `Size`, or `Material`). You can add up to 3 different labels.
3. Avante will automatically render these filters as visual pills or images.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 16.17.46.png" alt=""><figcaption></figcaption></figure>

***

### Quick search

Avante features a predictive search drawer that suggests products, collections, and blog posts as the customer types.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 16.27.19.png" alt=""><figcaption></figcaption></figure>

To enable and configure it, go to **Theme settings** → [**Quick search**](../theme-settings/quick-search.md). Here you can adjust the result display (grid or list) and enable key features like:

* **Popular searches:** You can connect a specific navigation menu to show curated promotional links (like "New Arrivals" or "Summer Sale") inside the search drawer. These links appear before the customer even starts typing, acting as a great conversion tool.
* **'All results' button:** Customize the text for the button that links to the full search results page.

***

### Search page

The main `/search` page uses a flexible product grid that is very similar to your collection pages, supporting the same filter layouts and product card features.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 16.33.02.png" alt=""><figcaption></figcaption></figure>

For full instructions on how to configure its layout, adjust the grid, and manage blog post results, check out our detailed guide on the [**Search template**](../templates/search-template.md).

