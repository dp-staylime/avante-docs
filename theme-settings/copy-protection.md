# Breadcrumbs

Show the navigation path on product and collection pages (e.g. Home → Collections → Product). Helps customers orient themselves and improves SEO.

<figure><img src="../.gitbook/assets/Group 18.jpg" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** Breadcrumbs create multiple URLs for the same product, which can affect SEO. In most cases the UX benefit outweighs the SEO impact.
{% endhint %}

***

### Settings

| Setting               | Description                                                                                                                                                                                     |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Enable**            | Activates breadcrumb navigation                                                                                                                                                                 |
| **Size**              | Typography size for breadcrumb text                                                                                                                                                             |
| **Dim path**          | Reduces visual weight of the path, making the current item stand out                                                                                                                            |
| **Path style**        | <p><strong>Disable:</strong> Hides the collection path, shows only the current item<br><strong>Show collections page:</strong> Includes the <code>/collections</code> root page in the path</p> |
| **Show current item** | Shows the current product or page name as the last crumb                                                                                                                                        |

***

### How to enable

Breadcrumbs require two steps:

{% stepper %}
{% step %}
#### **Step 1 — Configure in Theme settings**

Go to **Theme settings → Breadcrumbs** and enable the toggle.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-19 at 16.34.08.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### **Step 2 — Add the block to your template**

1. Open **Theme Editor → Default product** (or any product template)
2. Inside **Product overview** section, click **Add block → Breadcrumbs**
3. Save

<figure><img src="../.gitbook/assets/Screenshot 2026-06-19 at 16.34.57.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Note:** Adding the block without enabling **Theme settings → Breadcrumbs** will show nothing.
{% endhint %}
{% endstep %}
{% endstepper %}
