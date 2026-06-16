# Mega menu & Hover mega menu

Avante includes two types of advanced navigation blocks for the Header — **Mega menu** and **Hover mega menu**. Both expand into a full-width panel when a visitor hovers over a menu item.

> 💡 Both blocks automatically transform into a regular dropdown menu when the header width is less than 1024px (mobile and tablet).

***

### Mega menu vs Hover mega menu

|          | Mega menu                           | Hover mega menu                         |
| -------- | ----------------------------------- | --------------------------------------- |
| Layout   | Links in columns                    | Links + banner panels                   |
| Banners  | One banner                          | Up to 2 banners + per-item banners      |
| Columns  | 1–4                                 | —                                       |
| Best for | Large catalogs with many categories | Visual storytelling, featured campaigns |

📸 \[Screenshot: Mega menu открыт — видны колонки с линками] 📸 \[Screenshot: Hover mega menu открыт — видны линки + баннер]

***

### Setup — Mega menu

#### Step 1 — Create nested menu items in Shopify Admin

The mega menu displays child links from your navigation menu.

1. Go to **Shopify Admin → Content → Menus**
2. Open your main menu
3. Make sure the parent item you want to use as a trigger has child links nested under it
4. Save

📸 \[Screenshot: Shopify Admin → Content → Menus → вложенные пункты]

#### Step 2 — Add the Mega menu block

1. Open **Theme Editor → Header**
2. Click **Add block → Mega menu**
3. In the **Dropdown link** field, enter the exact name of the menu item you want to trigger the mega menu (e.g. `Seasons`, `Shop`)

📸 \[Screenshot: Header → Mega menu block → Dropdown link поле]

> ⚠️ The Dropdown link value must match the menu item name exactly — including capitalization. Do not translate this field using Translate & Adapt or any other app.

#### Step 3 — Configure the block settings

| Setting                 | Description                                                   |
| ----------------------- | ------------------------------------------------------------- |
| **Highlight menu item** | Enter item names (comma-separated) to display in accent color |
| **Menu heading**        | Heading text above the menu links                             |
| **Width**               | Wide or Narrow panel                                          |
| **Columns**             | 1–4 columns for links                                         |
| **Show lines**          | Dividers between columns                                      |

📸 \[Screenshot: Mega menu block настройки — Columns, Width, Highlight]

#### Step 4 — Add a banner (optional)

1. Enable **Show banner** in the block settings
2. Upload an image
3. Add a **Banner link**, **Heading**, **Subheading**
4. Adjust overlay opacity and content alignment

📸 \[Screenshot: Mega menu → Banner настройки]

***

### Setup — Hover mega menu

#### Step 1 — Add the Hover mega menu block

1. Open **Theme Editor → Header**
2. Click **Add block → Hover mega menu**
3. In the **Dropdown link** field, enter the exact name of the menu item (e.g. `Shop`)

📸 \[Screenshot: Header → Hover mega menu block → Dropdown link]

#### Step 2 — Configure banners

The Hover mega menu supports up to **2 static banners** plus individual banners per menu item.

**Static banners (Banner 1 & Banner 2):** Enable **Show banner** for each → upload image → add link, heading, and subheading.

**Per-item banners:** Use the **Hover mega menu banners** block to set up individual banners for specific menu items.

1. Click **Add block → Hover mega menu banners**
2. In the **Dropdown link** field, enter the name of the specific menu item
3. Upload the banner image for that item

📸 \[Screenshot: Hover mega menu banners block → Dropdown link + изображение]

***

### Common issue: menu not opening

If the mega menu doesn't open when hovering, the most common cause is a mismatch between the **Dropdown link** field and the actual menu item name.

**Check:**

1. Open **Theme Editor → Header → Mega menu block**
2. Note the value in **Dropdown link**
3. Go to **Shopify Admin → Content → Menus** and confirm a menu item with that exact name exists and has child links under it

See also: Mega menu isn't working →
