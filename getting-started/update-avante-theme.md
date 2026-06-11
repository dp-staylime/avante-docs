---
description: A guide to update the theme to the latest version
---

# Update Avante theme

Keeping your Avante theme up to date ensures your store benefits from the latest features, bug fixes, and compatibility improvements.

The most up-to-date version is always available on the Shopify Theme Store.

### Minor vs. major updates

Before updating, it's important to understand how Shopify handles different types of updates:

**Minor updates** (e.g. v13.0.0 → v13.0.1) Shopify automatically transfers your visual settings and safe code customizations.

**Major updates** (e.g. v13.0.0 → v14.0.0) The theme's core architecture changes significantly. Visual settings (colors, fonts) and custom code are not transferred automatically — you will need to reconfigure them manually.

***

### Update automatically ⚙️

{% stepper %}
{% step %}
#### Check notifications on Shopify

In your Shopify admin, go to **Online Store > Themes**. If a new version of Avante is available, you'll see a notification in your theme library.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 13.05.55.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Review update details

* Click the notification to view more details about the update.
* Select **View release notes** to read what's new in the release.
{% endstep %}

{% step %}
#### Add to theme library

Click **Add to theme** **library** to download and add the updated version to your Shopify store.

The updated version will now appear in your theme library, ready to customize and publish.
{% endstep %}
{% endstepper %}

### No update notification? 🔍

This usually happens if the theme was previously uploaded as a ZIP file (which breaks the connection to the Theme Store) or if there are code customizations conflicting with Shopify's update system.&#x20;

In this case, reinstall the theme manually:

{% stepper %}
{% step %}
#### Create a backup

Always duplicate your current theme before updating.

{% hint style="success" %}
**Steps:**

1. Go to **Online Store > Themes.**
2. Open the Actions dropdown for your current theme, select **Duplicate.**
3. Rename the duplicated file.
{% endhint %}
{% endstep %}

{% step %}
#### Install the latest theme version

{% hint style="success" %}
**Steps:**

1. Visit the Shopify Theme Store and choose **Avante** them&#x65;**.**
2. Click **Add a new copy** to add the latest version.
{% endhint %}
{% endstep %}

{% step %}
#### Transfer your settings

{% hint style="warning" icon="octagon-exclamation" %}
**Major update (e.g. v13 → v14)**&#x20;

Do NOT copy the `settings_data.json` file. The architecture has changed — pasting old code will break the new theme and cause errors in Theme Editor.&#x20;

**Reconfigure your Theme Settings (Colors, Typography) manually in the Theme Editor.**
{% endhint %}

{% hint style="success" %}
**Minor update (e.g. v13.0.0 → v13.0.1)**&#x20;

You can safely copy `settings_data.json` from the `Config` folder of your old theme into the new one via **Edit code**.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 13.13.56.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-06-11 at 13.14.55.png" alt=""><figcaption></figcaption></figure>

**For custom page templates:** Re-create your custom templates in the new theme — they won't exist there by default. Create a template with the exact same name, then copy the contents of the JSON file from the `Templates` folder of your old theme.
{% endstep %}

{% step %}
#### Re-install apps

Apps that add code to your theme files will need to be reinstalled or re-enabled in the new version.

{% hint style="info" %}
Find the app documentation in the [App Store](https://apps.shopify.com/) to follow the installation instructions.

If you're unfamiliar with this process, you can go to **Apps >** click **View details** to find the support email for that Shopify app.
{% endhint %}
{% endstep %}
{% endstepper %}
