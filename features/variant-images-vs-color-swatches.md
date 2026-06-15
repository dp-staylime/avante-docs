# Variant images vs Color Swatches

In Avante, color variants can be shown in two ways:

* **Variant images**
* **Color swatches**

Choose the option that fits how you want customers to shop.

{% columns %}
{% column %}
#### Variant images

Show a small product thumbnail for each color.

Best when each color has its own product photos.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.23.15.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
#### Color swatches

Show a small color circle for each color.

Best when you want a cleaner, simpler selector.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.43.56.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

{% hint style="info" %}
For both options, the value in **Variant label** should match your product option name, such as `Color`.
{% endhint %}

***

### Set up variant images

Variant images show a small thumbnail of the actual product photo for each color option.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.45.28.png" alt=""><figcaption></figcaption></figure>

{% stepper %}
{% step %}
#### Open the variant selector settings

Open **Theme Editor**. Go to **Theme settings → Variant selector**.
{% endstep %}

{% step %}
#### Enable variant images

Scroll to **Variant image**. Enter your option name in **Variant label**.
{% endstep %}

{% step %}
#### Adjust the appearance

Optionally adjust:

* shadow
* image ratio
* focal point
* corner radius
{% endstep %}
{% endstepper %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.40.09.png" alt=""><figcaption></figcaption></figure>

***

### Set up color swatches

Color swatches show a small color circle instead of a product photo. This keeps the selector compact and easy to scan.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.44.52.png" alt=""><figcaption></figcaption></figure>

{% stepper %}
{% step %}
#### Open the variant selector settings

Open **Theme Editor**. Go to **Theme settings → Variant selector**.
{% endstep %}

{% step %}
#### Enable color swatches

Scroll to **Color pills**. Enter your option name in **Variant label**.
{% endstep %}
{% endstepper %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.47.02.png" alt=""><figcaption></figcaption></figure>

***

### Set up custom color swatches

Avante uses standard HTML color names by default.

If a color name does not match, or the displayed shade looks wrong, you can upload custom color images.

{% stepper %}
{% step %}
#### Set Style to Image in Theme settings

1. Go to **Theme Editor → Theme settings → Variant selector → Color pills**
2. In the **Variant label** field enter your option name (e.g. `Color`)
3. Set **Style** to **Image**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.52.19.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Prepare the image files

Create **PNG** files for your color values. Name each file to **match the variant** value. Use lowercase letters and underscores for spaces.

* `Red` → `red.png`
* `Ocean blue` → `ocean_blue.png`

Recommended: **60×60px**, under **20KB**

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 14.50.54.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Upload the files in Shopify

In Shopify admin, go to **Content → Files**. Upload the prepared images.
{% endstep %}

{% step %}
#### Let Avante match the files automatically

After upload, Avante automatically links the images to matching color variants across your store.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Custom swatches only work when the file name matches the variant value format.
{% endhint %}

***

### Alternative: set custom colors directly in Theme settings

Instead of uploading PNG files, you can define custom colors directly in the Theme Editor.

This is faster when you only need solid colors.

{% stepper %}
{% step %}
#### Open the variant selector settings

Go to **Theme Editor → Theme settings → Variant selector**.
{% endstep %}

{% step %}
#### Open the custom color configuration

Scroll to **Custom colors for pills → Configuration**.
{% endstep %}

{% step %}
#### Add your color rules

Add one rule per line in this format:

```
VariantName:#hexcolor
```

Example:

```
Red:#ff0000
Ocean Blue:#4a90d9
Bubble Pink:#f5b8c4
```
{% endstep %}
{% endstepper %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-15 at 15.13.02.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Use the PNG method when you need textures, patterns, or photographic swatches.

For solid colors, the **Configuration** field is quicker.
{% endhint %}

***

Want the product gallery to show only media for the selected variant?

See [Display only media related to chosen variant](display-variant-media.md).
