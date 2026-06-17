# Store Selector

The Store Selector lets customers switch between your retail or warehouse locations and see real-time product pickup availability — directly on collection pages and product pages.

***

### Step 1: Set up Shopify Locations

Before configuring the Store Selector in the theme, set up your locations in Shopify Admin.

Go to **Shopify Admin → Settings → Locations** and make sure all your locations are active.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 10.46.01.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Note:** The location names shown here (e.g. "TBB Store Boston", "Warehouse Brussels") are exactly what you need to enter in the **Store name** field in the theme. Copy them character-for-character.
{% endhint %}

Then open each location and make sure **Pickup in store** is set to **On** under the Fulfillment section. Without this, the availability widget won't display for that location.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.19.42.png" alt=""><figcaption></figcaption></figure>

For full setup instructions, follow Shopify's official guide: [Setting up pickup in store for online orders](https://help.shopify.com/en/manual/fulfillment/setup/delivery-methods/pickup-in-store)

***

### Step 2: Add the Store Selector drawer

1. Open **Theme Editor**
2. In the left panel, find **More header sections** group
3. Click **Add section → Store selector drawer**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.00.56.png" alt=""><figcaption></figcaption></figure>

4. Inside the section, click **Add block → Store**
5. Fill in the block settings:
   * **Store name** — must exactly match the name in Shopify Admin → Settings → Locations
   * **Address** — shown inside the drawer
   * **Image** — optional logo or location photo
   * **Details** — opening hours, pickup info, or any other text

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.21.39.png" alt=""><figcaption></figcaption></figure>

Repeat for each location.

***

### Step 3: Show Store Selector in navigation

**In the header**

1. In Theme Editor, open **Header section → Miscellaneous block**
2. Find **Store selector** in the right panel
3. Enable the **Enable** toggle
4. Optionally enable **Show icon**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.22.38.png" alt=""><figcaption></figcaption></figure>

**In the menu drawer**

1. In Theme Editor, open **Menu drawer section**
2. Click **Add block → Store selector**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.24.06.png" alt=""><figcaption></figcaption></figure>

***

### Step 4: Show pickup availability on product cards

To display availability badges on product cards in collection pages:

1. In Theme Editor, open your collection template
2. Click on a section that shows product cards (e.g. **Collection page**)
3. In the right panel, scroll to **Product card content**
4. Enable **Show pickup availability**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.29.05.png" alt=""><figcaption></figcaption></figure>

***

### Step 5: Show pickup availability on the product page

1. In Theme Editor, open **Default product** template
2. Inside **Product overview** section, click **Add block → Pickup availability**
3. The block shows the currently selected store and availability for the active variant

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.44.26.png" alt=""><figcaption></figcaption></figure>

***

### Customize colors

To change the colors of the availability indicators:

Go to **Theme settings → Colors** and scroll to the **Pickup availability** group:

| Setting           | What it controls                |
| ----------------- | ------------------------------- |
| Available text    | Color of "Available at..." text |
| Available icon    | Color of the green dot          |
| Out of stock text | Color of unavailable text       |
| Out of stock icon | Color of the unavailable dot    |

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.52.03.png" alt=""><figcaption></figcaption></figure>

***

### Live example

<figure><img src="../.gitbook/assets/Screenshot 2026-06-17 at 11.26.51.png" alt=""><figcaption></figcaption></figure>
