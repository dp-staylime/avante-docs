---
description: A guide to update the theme to the latest version
---

# Update Avante theme

Keeping your **Avante theme** up to date ensures your store benefits from the latest features, bug fixes, and compatibility improvements.&#x20;

> The most up-to-date version of the theme is always available on the Shopify Theme Store.

{% hint style="danger" %}
Any **code customizations** in your current theme are **not transferred automatically** to a new theme version.&#x20;

You'll need to manually duplicate and move custom code to the updated theme.
{% endhint %}

***

### Update the theme automatically ⚙️

{% stepper %}
{% step %}
#### Check notifications on Shopify

In your Shopify admin, go to **Online Store > Themes**. If a new version of Avante is available, you'll see a notification in your theme library.

<figure><img src="../.gitbook/assets/Screenshot 2026-06-03 at 14.31.39.png" alt=""><figcaption></figcaption></figure>
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

### Troubleshooting: no update notification? 🔍

If you don't see an update notification, it could be due to code customizations conflicting with Shopify's update system, or the theme was previously uploaded as a ZIP file. In this case, you can manually reinstall the theme and transfer your customizations.

{% stepper %}
{% step %}
#### Create a backup

Before updating, always **duplicate** your current theme so you can restore your store if something goes wrong.&#x20;

{% hint style="success" %}
**Steps:**

1. Go to **Online Store > Themes.**
2. Open the Actions dropdown for your current theme, select **Duplicate.**
3. Rename the duplicated file.
{% endhint %}
{% endstep %}

{% step %}
#### Install the latest theme version

Install the theme from the Shopify Theme Store.

{% hint style="success" %}
**Steps:**

1. Visit the Shopify Theme Store and choose **Avante** them&#x65;**.**
2. Click **Add a new copy** to add the latest theme version to your online store.
{% endhint %}
{% endstep %}

{% step %}
#### Move the theme settings and pages

After uploading the new theme, transfer your settings, custom templates, and modifications to the new version.

{% hint style="success" %}
**Steps:**

1. Go to your current theme, click **Actions > Edit code**.\\
2. Copy the following files from the **old theme** and paste them into the same folders in the **new version**:
   * All edited **JSON files** in the `Templates` folder.
   * The `settings_data.json` file in the `Config` folder.
3. Re-create custom templates (if any).
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-06-03 at 14.31.39.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
For custom templates, you'll need to create the JSON template in the new theme files since they won't exist there by default. More details [here](https://help.shopify.com/manual/online-store/themes/theme-structure/templates#create-a-new-template) from Shopify on creating new templates in the theme.
{% endhint %}
{% endstep %}

{% step %}
#### Re-install apps

Any apps that add code to your theme's files will need to be reinstalled. This can be an automatic or manual process depending on the app, so **confirm with the app's developer whether removing and adding the app is enough to connect with the new version.**

{% hint style="info" %}
Find the app documentation in the [App Store](https://apps.shopify.com/) to follow the installation instructions.

If you're unfamiliar with this process, you can go to **Apps >** click **View details** to find the support email for that Shopify app.
{% endhint %}
{% endstep %}
{% endstepper %}
