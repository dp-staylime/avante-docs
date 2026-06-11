# Mega menu isn't working / dropdowns won't open

The Mega menu and Hover mega menu blocks both require a **Dropdown link** value that matches the exact name of a menu item in your navigation.

### How to fix this

1. Open **Theme Editor → Header → Mega menu** or **Hover mega menu** block
2. In the **Dropdown link** field, enter the exact name of the menu item you want to display as a mega menu (e.g. `Seasons` )

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-11 at 12.13.38.png" alt=""><figcaption></figcaption></figure>

3. Go to **Shopify Admin → Content → Menus**, open your menu and make sure that item has child links nested under it

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-11 at 12.24.20.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="triangle-exclamation" %}
Do not translate the **Dropdown link** field using Translate & Adapt or any other app. This is an internal reference — translating it breaks the connection to your navigation.
{% endhint %}

{% hint style="success" icon="lightbulb" %}
**Mega menu vs Hover mega menu**

Both blocks use the same Dropdown link logic.

_Mega menu_ displays links in columns. _Hover mega menu_ reveals a panel with banners on hover.

For full setup details see [Mega menu & Hover mega menu →](../../features/mega-menu.md)
{% endhint %}

