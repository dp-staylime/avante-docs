# On mobile, tapping a parent menu item navigates away instead of expanding the submenu

This is the default theme behavior.

* Tap the **arrow** to expand the submenu.
* Tap the **text** to open the parent link.

There is no built-in setting to change this behavior.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-12 at 10.42.44.png" alt=""><figcaption></figcaption></figure>

***

### Disable navigation on a specific parent item

If you want tapping the text to expand the submenu instead of opening the parent link, add this in **Theme Editor → Theme settings → Custom CSS**:

```css
.link-[item-name] {
  pointer-events: none;
}
```

Replace `[item-name]` with the menu item's CSS class.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-12 at 10.48.56.png" alt=""><figcaption></figcaption></figure>

### How to find the class

1. Open your store in the browser.
2. Right-click the menu item and select **Inspect**.
3. Find the `<a>` element and look for a class that starts with `link-`, such as `.link-brands-designers` or `.link-shop`.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-12 at 10.46.08.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" icon="lightbulb" %}
This only affects the menu item you target. All other menu items keep their default behavior.
{% endhint %}
