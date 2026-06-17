---
description: Set up transparent navigation and control the sidebar hover background.
---

# Transparent header

Use transparent navigation to let the header or sidebar sit on top of the first section.

This works best with hero-style layouts and full-width media banners.

### Basic setup

Transparent navigation requires two settings to be active at the same time.

{% stepper %}
{% step %}
### Enable the global setting

1. Go to **Theme Editor → Theme settings → Appearance**
2. Scroll down to **Transparent header and sidebars**
3. Enable **Allow transparent navigation**
4. Enable **Enable on mobile** if you want the effect on small screens

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 15.01.13.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set the first section to overlap

1. Make sure the first section on the page is one of these:
   * **Slideshow with media**
   * **Image banner**
   * **Video banner**
2. Open that section's settings
3. Set **Section width → Overlap by navigation**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 15.03.24.png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Both settings must be active at the same time.
{% endhint %}

***

### Sidebar navigation hover background

If you use **Sidebar-based navigation**, the sidebar is designed to be transparent over the first section — and turn white when **hovered**.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 16.03.31.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 16.03.47.png" alt=""><figcaption></figcaption></figure>

If this animation is not working, check two things:

#### 1. Set the menu style to Overlap slide out

Open **Theme Editor → Main sidebar → Main menu block** → set **Menu style** to **Overlap slide out**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 15.16.19.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
This style is required for the hover background transition.
{% endhint %}

#### 2. Make sure the menu has nested child links

Go to **Shopify Admin → Content → Menus** → open your menu and make sure at least one item has child links nested underneath it.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 14.44.02.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="question" %}
If you need help building nested links, see [**How do I create nested / dropdown menus?**](../faq/navigation/how-do-i-create-nested-dropdown-menus.md).
{% endhint %}

{% hint style="success" icon="lightbulb" %}
#### No nested items in your menu?

Add a **Nested menu** block in **Main sidebar** as a workaround.

Go to **Main sidebar → Add block → Nested menu**.

In **Dropdown link**, enter the exact name of any existing menu item.

This activates the hover animation without changing your actual menu structure.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 16.09.38.png" alt=""><figcaption></figcaption></figure>

***

### Changing the sidebar hover background color

By default, the sidebar hover background uses the color from **Theme settings → Colors → Layout → Background**.

{% hint style="warning" %}
Make sure **Main sidebar → Colors → Color scheme** is **not** set to **Set**.

If it is set to **Set**, the background stays visible all the time.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 16.11.47.png" alt=""><figcaption></figcaption></figure>

To change the background color across the entire site:

Go to **Theme Editor → Theme settings → Colors → Layout** and update **Background**.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 16.14.12.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
This affects all sections and blocks across your store.
{% endhint %}

***

### Change the sidebar hover color only

Add this in **Main sidebar → Custom CSS**:

{% code title="Main sidebar → Custom CSS" %}
```css
.main-sidebar:hover {
  background-color: #00ffee;
}
```
{% endcode %}

Replace `#00ffee` with your own color value.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 15.33.46.png" alt=""><figcaption></figcaption></figure>
