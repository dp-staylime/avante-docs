# Mega menu & Hover mega menu

Avante includes two types of advanced navigation blocks for the Header — **Mega menu** and **Hover mega menu**. Both expand into a full-width panel when a visitor hovers over a menu item.

{% hint style="success" icon="lightbulb" %}
Both blocks automatically transform into a regular dropdown menu when the header width is less than 1024px (mobile and tablet).
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.41.11.png" alt=""><figcaption></figcaption></figure>

***

### Mega menu vs Hover mega menu

|                  | Mega menu                           | Hover mega menu                         |
| ---------------- | ----------------------------------- | --------------------------------------- |
| Layout           | Links in columns                    | Links + up to 2 banners                 |
| Per-item banners | —                                   | ✓ via Hover mega menu banners block     |
| Columns          | 1–4                                 | —                                       |
| Best for         | Large catalogs with many categories | Visual storytelling, featured campaigns |

{% columns %}
{% column %}
#### Mega menu

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.49.49.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
#### Hover mega menu

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.50.12.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

### Setup — Mega menu

#### Step 1 — Create nested menu items

The mega menu displays child links from your navigation.

1. Go to **Shopify Admin → Content → Menus**
2. Open your main menu
3. Drag child links underneath the parent item you want to use as a trigger
4. Save

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.53.36.png" alt=""><figcaption></figcaption></figure>

#### Step 2 — Add the Mega menu block

1. Open **Theme Editor → Header**
2. Click **Add block → Mega menu**
3. In the **Dropdown link** field, enter the exact name of the parent menu item (e.g. `Seasons`, `Shop`)
4. Configure the block settings (see below)

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.54.44.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
The **Dropdown link** value must match the menu item name exactly — including capitalization. Do not translate this field using Translate & Adapt or any other app.
{% endhint %}

<details>

<summary>Block settings</summary>

**Dropdown link** \
Enter the title of the dropdown parent link to show its nested menu as the mega menu.

**Highlight menu item** \
Enter item names separated by commas to display them in accent color (e.g. `Sale, New`).

**Menu heading** \
Optional text heading above the menu links. Wrap a word in `{curly brackets}` to apply the Secondary heading style from Theme settings → Typography.

**Heading size** \
Choose the size of the heading text.

**Width**

* **Wide** — spans the full width of the page
* **Narrow** — leaves spacing on both sides

**Columns** \
Select 1–4 columns. Links are automatically divided into equal-sized columns.

**Show lines** \
Enable to display divider lines between columns.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 14.58.28.png" alt=""><figcaption></figcaption></figure>

</details>

#### Step 3 — Add a banner (optional)

1. Enable **Show banner**
2. Upload an **Image** (landscape 3:2 or wide 16:9 works best)
3. Add a **Banner link** URL
4. Adjust **Image overlay**, **Image overlay gradient**, and **Image overlay opacity**
5. Set **Content color** for heading and subheading text
6. Add **Subheading** and **Heading** text
7. Set **Subheading size** and **Heading size**
8. Use **Swap banner position** to move it from right to left
9. Set **Vertical** and **Horizontal text alignment**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.00.21.png" alt=""><figcaption></figcaption></figure>

***

### Setup — Hover mega menu

#### Step 1 — Add the Hover mega menu block

1. Open **Theme Editor → Header**
2. Click **Add block → Hover mega menu**
3. In the **Dropdown link** field, enter the exact name of the parent menu item (e.g. `Shop`)

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.01.18.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="triangle-exclamation" %}
The **Dropdown link** value must match the menu item name exactly — including capitalization. Do not translate this field using Translate & Adapt or any other app.
{% endhint %}

<details>

<summary>Block settings</summary>

**Dropdown link** \
Enter the menu item name to be displayed as hover mega menu.

**Highlight menu item** \
Enter item names separated by commas to display them in accent color.

**Color** \
Sets the color for highlighted menu items.

**Link size** \
Choose the typography size for menu links.

**Menu heading** \
Optional heading above the menu links. Wrap a word in `{curly brackets}` to apply the Secondary heading style from Theme settings → Typography.

**Heading size** \
Choose the size of the heading text.

**Width**

* **Wide** — spans the full width of the page
* **Narrow** — leaves spacing on both sides

**Show lines** \
Enable to display divider lines between menu items.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.04.59.png" alt=""><figcaption></figcaption></figure>

</details>

#### Step 2 — Configure banners

The Hover mega menu supports **Banner 1** and **Banner 2** — two static banners displayed alongside the menu links.

For each banner:

1. Enable **Show banner**
2. Upload an **Image** (landscape 3:2 or wide 16:9 works best)
3. Add a **Banner link** URL
4. Adjust **Image overlay**, **Image overlay gradient**, and **Image overlay opacity**
5. Set **Content color** for text
6. Add **Subheading** and **Heading** text
7. Set **Subheading size** and **Heading size**
8. Set **Vertical** and **Horizontal text alignment**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.07.12.png" alt=""><figcaption></figcaption></figure>

#### Step 3 — Add per-item banners (optional)

This block lets you show a different banner when hovering over a specific child item within the Hover mega menu.

1. Click **Add block → Hover mega menu banners**
2. In the **Hover menu item link** field, enter the name of the **child menu item** (e.g. `Shop by type`) — not the parent trigger
3. _(Optional)_ Fill in the **Dropdown link** field to specify which Hover mega menu block these banners belong to — only needed if the same child item appears in more than one Hover mega menu block
4. Enable **Show banner**, upload an image and configure the banner settings

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.18.16.png" alt=""><figcaption></figcaption></figure>

***

### Common issue: menu not opening

The most common cause is a mismatch between the **Dropdown link** field and the actual menu item name.

**Check:**

1. Open **Theme Editor → Header → Mega menu** or **Hover mega menu** block
2. Note the value in **Dropdown link**
3. Go to **Shopify Admin → Content → Menus** and confirm a menu item with that exact name exists and has child links under it

{% hint style="danger" %}
Never translate the **Dropdown link** field using **Translate & Adapt** — this breaks the connection to your navigation tree.
{% endhint %}
