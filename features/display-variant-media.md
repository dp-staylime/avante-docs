# Display only media related to chosen variant

This feature filters the product gallery to show only images of the currently selected color variant. When a customer switches between colors, only the relevant photos are visible.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

***

### How it works

The feature uses image **Alt text** to group photos by color. When a customer selects a variant, the theme reads the color name from the Alt text and hides all images that don't match.

{% hint style="warning" icon="triangle-exclamation" %}
Simply assigning images to variants in Shopify Admin is not enough. You must add the correct Alt text to every image for filtering to work.
{% endhint %}

***

### Setup

#### Step 1 — Add Alt text to your images

1. Go to **Shopify Admin → Products → \[your product]**
2. Scroll to the **Media** section
3. Click on an image to open it
4. Click **Edit** → **Add alt text**
5. Add the color name in parentheses at the end of the alt text

```
Format:
Any descriptive text (Color name)

Examples:
Front view (Black), Model wearing the dress (Ocean Blue), Detail shot (Ivory White)
```

6. Save
7. Repeat for every image in that color group

<figure><img src="../.gitbook/assets/clean_up!.gif" alt=""><figcaption></figcaption></figure>

{% hint style="success" icon="lightbulb" %}
The color name inside the parentheses must match exactly across all images of the same color — including capitalization. `(Black)` and `(black)` are treated as different groups.
{% endhint %}

***

#### Step 2 — Link the variant to its image

Make sure the **first image of each color** is assigned directly to its variant in Shopify Admin:

1. Go to **Shopify Admin → Products → \[your product] → Variants**
2. Open a variant (e.g. Black / S)
3. Assign the main image for that color to this variant
4. Repeat for each color variant

The theme reads the Alt text from this assigned image to know which group to display when that variant is selected.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 15.59.56.png" alt=""><figcaption></figcaption></figure>

***

#### Step 3 — Enable the setting in Theme Editor

1. Open **Theme Editor → Products → Default product template** (or your custom product template)
2. Click on the **Product overview** section
3. Find **Show only media of selected variant** and enable it
4. Save

<figure><img src="../.gitbook/assets/Screenshot 2026-06-16 at 16.03.18.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/before-after.gif" alt=""><figcaption></figcaption></figure>

***

### Common issues

<details>

<summary>Images are not filtering when I switch variants</summary>

Check that:

* Every image has Alt text with the color name in **parentheses**
* The color name is spelled and capitalized consistently across all images of the same color
* The variant has an image assigned to it in **Variants** (not just in the Media section)

</details>

<details>

<summary>Only one image is showing in the gallery</summary>

If you see only one photo after enabling the feature, the other images likely have no Alt text or mismatched color names. The theme hides all images it cannot match to the selected variant.

Go back to **Media** and verify the Alt text on every image.

</details>

<details>

<summary>The gallery is not filtering on a specific product</summary>

Check if that product uses a **custom template**. The **Show only media of selected variant** setting needs to be enabled separately in each template it's used on.

Go to **Theme Editor → Products → \[your custom template] → Product overview** and enable the setting there.

</details>

{% hint style="warning" icon="lightbulb" %}
**Tip:** Images without any Alt text (or without parentheses in the Alt text) will be visible for **all color selections** — useful for lifestyle or packaging shots that apply to the whole product.
{% endhint %}
