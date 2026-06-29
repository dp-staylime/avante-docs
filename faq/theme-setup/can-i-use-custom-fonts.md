# Can I use custom fonts?

### Option 1 — Use the built-in font picker (Google Fonts)

If your font is available in the Google Fonts library, no code is needed.

Go to **Theme settings → Typography** and use the font picker to select your font directly.

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-29 at 17.44.34.png" alt=""><figcaption></figcaption></figure>

***

### Option 2 — Use a custom font file (WOFF/WOFF2)

Shopify's built-in font picker only supports fonts from the Shopify and Google font library. Using a custom font file requires a code edit.

{% hint style="warning" icon="triangle-exclamation" %}
**Important:** This is not a Theme Editor setting. It requires direct access to your theme files.
{% endhint %}

{% stepper %}
{% step %}
#### Step 1 — Prepare your font files

You'll need the font in `.woff2` format (recommended) or `.woff`. Make sure you have the weights you need — typically Regular (400) and Bold (700).
{% endstep %}

{% step %}
#### Step 2 — Upload font files to your theme

1. Go to **Shopify Admin → Online Store → Themes**
2. Next to your theme click **Edit code**
3. In the left panel find **Assets** → click **Add a new asset → Upload file**
4. Upload your `.woff2` files one by one

The file name you upload is exactly what you use in the CSS — no full URL needed.
{% endstep %}

{% step %}
#### Step 3 — Enable custom styles

Open the Theme Editor → **Edit code** → `snippets/custom-assets.liquid` and change:

```liquid
{% assign useCustomStyles = false %}
```

to:

```liquid
{% assign useCustomStyles = true %}
```
{% endstep %}

{% step %}
#### Step 4 — Add the font to custom-styles.css

Open `assets/custom-styles.css` and add your `@font-face` declarations:

```css
@font-face {
  font-family: 'Your Font Name';
  src: url('your-font-regular.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Your Font Name';
  src: url('your-font-bold.woff2') format('woff2');
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}

:root {
  --base-font-family: 'Your Font Name', sans-serif;
}
```

Replace `your-font-regular.woff2` with the actual file names from Step 2. For monospace fonts, use `monospace` instead of `sans-serif` as the fallback.

{% hint style="warning" icon="triangle-exclamation" %}
**Note:** `--base-font-family` applies the font globally. To apply it only to buttons, add this instead:
{% endhint %}

```css
.button,
.shopify-challenge__button,
.shopify-payment-button__button,
button[type="submit"],
a.button,
.product-form__submit,
.cart__checkout-button {
  font-family: 'Your Font Name', sans-serif;
}
```
{% endstep %}
{% endstepper %}

***

### Need help?

If you'd prefer us to handle this for you, submit a request and our team will take care of it.

{% embed url="https://staylime.zendesk.com/hc/en-us/requests/new" %}
