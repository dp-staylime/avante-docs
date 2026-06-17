# Store Selector

The Store Selector lets customers switch between your retail or warehouse locations and see real-time product pickup availability — directly on collection pages and product pages.

***

#### Step 1: Set up Shopify Locations

Before configuring the Store Selector in the theme, make sure your locations are set up in Shopify Admin.

Go to **Shopify Admin → Settings → Locations** and add each location with its full name and address. These are the locations the theme will link to.

> **Important:** The store name you enter in the theme must exactly match the location name in Shopify Admin → Settings → Locations. Any mismatch will break the availability display.

***

#### Step 2: Add the Store Selector drawer

The Store Selector drawer is a section that lives in the header area. Each store inside it corresponds to one Shopify Location.

1. Open **Theme Editor**
2. In the left panel, find **More header sections** group
3. Click **Add section → Store selector drawer**
4. Inside the section, click **Add block → Store**
5. Fill in the block settings:
   * **Store name** — must exactly match the name in Shopify Admin → Settings → Locations
   * **Address** — shown inside the drawer
   * **Image** — optional logo or photo
   * **Details** — opening hours, pickup info, or any other text

Repeat for each location.

`[SCREENSHOT: Theme Editor showing Store selector drawer section with two Store blocks, and the right panel showing Store name, Address, Image, Details fields — Image 2]`

***

#### Step 3: Show Store Selector in navigation

**In the header**

1. In Theme Editor, open **Header section → Miscellaneous block**
2. Find **Store selector** in the right panel
3. Enable the **Enable** toggle
4. Optionally enable **Show icon**

`[SCREENSHOT: Header Miscellaneous block selected, right panel showing Store selector toggle enabled, "Select your store" visible in the header — Image 3]`

**In the menu drawer**

1. In Theme Editor, open **Menu drawer section**
2. Click **Add block → Store selector**

The drawer will now show the store switcher when customers open the mobile menu.

***

#### Step 4: Show pickup availability on product cards

To display availability badges on product cards in collection pages:

1. In Theme Editor, open your collection template
2. Click on a section that shows product cards (e.g. **Collection page**)
3. In the right panel, scroll to **Product card content**
4. Enable **Show pickup availability**

`[SCREENSHOT: Collection page section selected in Theme Editor, right panel showing "Show pickup availability" toggle enabled, product cards showing "Available to pickup at SpecHaus" — Image 4]`

***

#### Step 5: Show pickup availability on the product page

1. In Theme Editor, open **Default product** template
2. Inside **Product overview** section, click **Add block → Pickup availability**
3. The block shows the currently selected store and availability for the active variant

`[SCREENSHOT: Product overview section with Pickup availability block selected, right panel showing block settings, product page showing "Available to pickup at Focus and Frame" — Image 5]`

***

#### Customize colors

To change the colors of the availability indicators:

Go to **Theme settings → Colors** and scroll to the **Pickup availability** group:

| Setting           | What it controls                |
| ----------------- | ------------------------------- |
| Available text    | Color of "Available at..." text |
| Available icon    | Color of the green dot          |
| Out of stock text | Color of unavailable text       |
| Out of stock icon | Color of the unavailable dot    |

`[SCREENSHOT: Theme settings → Colors open, Pickup availability section highlighted with color pickers — Image 6]`

***

#### Live example

`[SCREENSHOT: Store selector drawer open on storefront, showing two locations with addresses and checkboxes — Image 1]`
