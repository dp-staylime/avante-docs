# Filters & search

### Setting up filters

In Shopify OS 2.0 themes like Avante, adding variants or tags to your products doesn't make filters appear automatically on collection pages. Filtering is managed centrally through Shopify's native **Search & Discovery** app — you need to explicitly add each filter there.

{% stepper %}
{% step %}
Install [**Search & Discovery**](https://apps.shopify.com/search-and-discovery) from the App Store — it's free.
{% endstep %}

{% step %}
Go to the app → **Filters** → Add filters (availability, price, vendor, product type, or metafields)

<figure><img src="../.gitbook/assets/Screenshot 2026-06-30 at 14.54.11.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Filters automatically appear on your collection pages

{% hint style="warning" icon="question" %}
For more details, see [Shopify's official guide on search and discovery filters](https://help.shopify.com/en/manual/online-store/storefront-search/search-and-discovery-filters).
{% endhint %}
{% endstep %}
{% endstepper %}

***

### Filter swatches

To show color filters as visual swatches instead of checkboxes:

1. Go to **Theme settings → Filter swatches → Color swatches**
2. Enter the exact name of your filter option (e.g. `Color`)
3. Avante will render that filter as color pills

### Quick search

Enable in **Theme settings → Quick search**. The search drawer supports:

* Product results with images
* Collection results
* Blog post results
* Suggested queries

### Search page

The `/search` page uses the same product grid as collection pages. Configure it in **Theme Editor → Search template**.

