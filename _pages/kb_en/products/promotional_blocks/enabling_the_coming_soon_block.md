---
lang: en
layout: article_with_sidebar
updated_at: '2016-09-28 18:05 +0400'
identifier: ref_hQnN8cAT
title: Enabling the &quot;Coming soon&quot; block
categories:
  - User manual
published: true
order: 200
redirect_from:
  - /kb_en/products/enabling_the_coming_soon_block.html
---


The "Coming soon" feature in X-Cart 5 is available through the use of **Product Advisor** module by X-Cart team. With this feature your store can showcase products with an arrival date in the future:

*   in a separate block titled "Coming soon";
*   on a separate page (`http://<your-domain>/<x-cart-5-directory>/?target=coming_soon`) available by default through the "Coming soon" item in your store's Primary menu.

In addition to that, products with an arrival date in the future can be marked with "Coming soon" labels in all product lists in the Customer front end.

To use the "Coming soon" feature, make sure that the module **Product Advisor** is installed and enabled at your store:

![]({{site.baseurl}}/attachments/6389778/8717811.png)To configure how the products that are about to appear in your store's catalog should be displayed to your store's visitors, you will need to adjust some module settings:

1.  Click the **Settings** link near the "Product Advisor" module icon in the list of your store's installed modules to go to the module's settings page.
2.  On the "Product Advisor" module settings page, adjust the settings in the **"Coming soon" block settings** section:
    ![]({{site.baseurl}}/attachments/6389776/8717923.png)
    The settings are as follows:
    *   **Enable "Coming soon" feature in catalog**: Enable this option to enable the "Coming soon" feature.
    *   **Mark upcoming products in catalog**: Enable this option to mark all the products that are about to appear in your store with the "Coming soon" label. The "Coming soon"  labels on products will appear in all product lists except for the "Coming soon" lists. 
        ![]({{site.baseurl}}/attachments/6389776/8717926.png)

    *   **Show arrival date on product details pages**: This setting defines whether the arrival date for products that are "coming soon" should be displayed on the product details pages of the respective products. Enable the option to show the arrival date; disable to hide the arrival date.
        ![]({{site.baseurl}}/attachments/6389776/8717927.png)
    *   **Show "coming soon" products only from category being viewed by customer**: This setting defines whether you want to show "coming soon" products from the entire store or just from the category the customer is currently viewing. Drupal block settings can override this option (when the DrupalConnector module is enabled).
    *   **Display "Coming soon" block on sidebar (otherwise in center area)**: This setting defines the location of the "Coming soon" block. Enable if you want the "Coming soon" block to appear in the sidebar:
        ![]({{site.baseurl}}/attachments/6389776/8717924.png)
        Disable if you want this block to be displayed in the central area of your store site:
        ![]({{site.baseurl}}/attachments/6389776/8717925.png)
        Drupal block settings can override this option (when the DrupalConnector module is enabled).
    *   **Maximum number of products to display in "Coming soon" block**: Specify the maximum number of products to be shown in the "Coming soon" block. Specify a non-zero value; otherwise, 3 products will be displayed by default. If the number of "coming soon" products is more than the number specified by this setting, any products above the specified number will be available for viewing via the "All upcoming products" link. Drupal block settings can override this option (when the DrupalConnector module is enabled).

3.  Once you are done configuring the settings, click the **Submit **button at the bottom of the page to save the changes.
