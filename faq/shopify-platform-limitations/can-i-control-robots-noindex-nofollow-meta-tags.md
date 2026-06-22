# Can I control robots / noindex / nofollow meta tags?

Some meta tags can be added only with a code edit.

This includes:

* `robots`
* `noindex` / `nofollow`
* verification tags such as Google site verification

{% hint style="warning" icon="triangle-exclamation" %}
**Important:** This is not available in the Theme Editor. It requires editing the theme code.
{% endhint %}

### Add a Google verification meta tag

If Google asks you to paste a tag into the home page `<head>`, add it to the main theme layout.

1. Go to Shopify **Admin → Online Store → Themes**.
2. Click **... → Edit code** on your published theme.
3. Open `layout/theme.liquid`.
4. Find the closing `</head>` tag.
5. Paste the verification tag on a new line right before `</head>`.
6. Save the file.

Example:

```html
<meta name="google-site-verification" content="-Aa4Ayy5UCZGHOjCvtks12sEfZMThnKvUx4yIp2TVZI" />
```

{% hint style="info" icon="circle-info" %}
Google verification tags confirm domain ownership. They do not enable analytics by themselves.
{% endhint %}

### For analytics

Use Shopify's native integrations when possible.

Preferred options:

* **Sales channels → Google & YouTube** for Google services
* **Settings → Customer events** for tracking pixels
* **Apps** if your analytics provider requires one

These methods are safer through theme updates and usually do not require manual code edits.

### Need help?

If you want us to add or review meta tags safely, [contact our support team](https://staylime.zendesk.com/hc/en-us/requests/new).
