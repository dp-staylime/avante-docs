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


{% endcolumn %}

{% column %}
#### Color swatches

Show a small color circle for each color.

Best when you want a cleaner, simpler selector.
{% endcolumn %}
{% endcolumns %}

{% hint style="info" %}
For both options, the value in **Variant label** should match your product option name, such as `Color`.
{% endhint %}

***

### Set up variant images

Variant images show a small thumbnail of the actual product photo for each color option.

_Screenshot: Variant images on the product page._

{% stepper %}
{% step %}
#### Open the variant selector settings

Open **Theme Editor**.

Go to **Theme settings → Variant selector**.
{% endstep %}

{% step %}
#### Enable variant images

Scroll to **Variant image**.

Enter your option name in **Variant label**.
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

_Screenshot: Theme settings → Variant selector → Variant image → Variant label._

***

### Set up color swatches

Color swatches show a small color circle instead of a product photo.

This keeps the selector compact and easy to scan.

_Screenshot: Color swatches on the product page._

{% stepper %}
{% step %}
#### Open the variant selector settings

Open **Theme Editor**.

Go to **Theme settings → Variant selector**.
{% endstep %}

{% step %}
#### Enable color swatches

Scroll to **Color pills**.

Enter your option name in **Variant label**.
{% endstep %}
{% endstepper %}

_Screenshot: Theme settings → Variant selector → Color pills → Variant label._

***

### Set up custom color swatches

Avante uses standard HTML color names by default.

If a color name does not match, or the displayed shade looks wrong, you can upload custom color images.

{% stepper %}
{% step %}
#### Prepare the image files

Create PNG files for your color values.

Name each file to match the variant value.

Use lowercase letters and underscores for spaces.

Examples:

* `Red` → `red.png`
* `Ocean blue` → `ocean_blue.png`

Recommended image size:

* `60 × 60 px`
* under `20 KB`
{% endstep %}

{% step %}
#### Upload the files in Shopify

In Shopify admin, go to **Content → Files**.

Upload the prepared images.
{% endstep %}

{% step %}
#### Let Avante match the files automatically

After upload, Avante automatically links the images to matching color variants across your store.
{% endstep %}
{% endstepper %}

_Screenshot: Shopify Admin → Content → Files._

{% hint style="info" %}
Custom swatches only work when the file name matches the variant value format.
{% endhint %}

***

Want the product gallery to show only media for the selected variant?

See [Display only media related to chosen variant](display-variant-media.md).
