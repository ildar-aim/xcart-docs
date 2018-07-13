---
lang: en
layout: article_with_sidebar
updated_at: '2017-11-25 22:43 +0400'
identifier: ref_fhzzxDTy
title: Adding products
categories:
  - User manual
published: true
order: 120
---
_This section is currently a draft.
Material may not yet be complete, information may presently be omitted, and certain parts of the content may be subject to radical, rapid alteration._


## Video guide

This video captures the process of adding a new product in X-Cart 5.3.x. 

<iframe class="youtube-player" type="text/html" style="width: 800px; height: 450px" src="https://www.youtube.com/embed/yJAaZIXOWLo" frameborder="0"></iframe>

## Adding a new product

This section provides information on how to add products to your store manually one by one. Please note that you can also add products via {% link "import" ref_TANvG2De %}. 

To add a new product:

1.  In your store's Admin area, go to the Products section (**Catalog** > **Products**).
    ![xc5_products.png]({{site.baseurl}}/attachments/ref_fhzzxDTy/xc5_products.png)

2.  Click the **Add product** button.
    ![xc5_products_add_product_button.png]({{site.baseurl}}/attachments/ref_fhzzxDTy/xc5_products_add_product_button.png)
    
    The Add product page opens.
    ![xc5_products_add_product_page.png]({{site.baseurl}}/attachments/ref_fhzzxDTy/xc5_products_add_product_page.png)

3.  Use the fields on the Add product page to provide information about the product. The page contains quite a number of fields, but you do not have to set all of them right now: the only required field is **Product name**, which means you only have to provide that value, whereas the rest of the product fields may be configured at any time later. See the section "[Basic product setup](#basic-product-setup)" below for a detailed explanation of all the product page fields. 

4.  To save the product information you have provided, click **Add product** at the bottom of the page. The new product will be saved. If necessary, you will be able to find it in the Products section (**Catalog** > **Products**) to do further editing or to specify some advanced product settings (See the section "[Advanced product setup](#advanced-product-setup)" section of this manual for more info).

## Basic product setup

When creating a new product, you need to specify product information via the form fields of the Add product page. Note that the actual set of fields available to you on this page depends on the X-Cart edition you are using and the set of addons (modules) enabled. The following list of fields corresponds to the set of product fields available for configuration on a fresh install of X-Cart Ultimate edition. If you do not see any of the fields described below in your X-Cart store back end, it means that the addon that enables this field is not installed or not active. To see what addons are active in your store and, if necessary, to install/activate more addons, check the **My addons** section in your X-Cart store Admin area. More info on the management of X-Cart addons can be found in the {% link "Managing addons" ref_gTOegEua %} section of this manual.

So, here is the product information that can be specified when adding a new product:

*   **Vendor**: Company name and email of the vendor who owns the product. This field is only available if X-Cart's {% link "Multi-vendor" ref_cvwmAuRi %} addon is active. Since an administrator can create products not only for themselves, but also for other users (vendors), this field needs to be adjusted to specify the owner of the product.

*   **Product name**: The name by which you and your customers will identify this product.

*   **SKU**: The product SKU (A code that will serve as a unique identifier for this product). If you leave this field blank, a SKU will be generated automatically when the product is saved.

*   **Images**: Use this section to add images of the product.

*   **Category**: The category (or categories) to which this product belongs. 

*   **Description**: A short product description that will be displayed on product list pages.

*   **Full description**: A longer product description that will be displayed on the product details page.

*   **Allow buyers to attach files to this product**: This field is only available if X-Cart's "[Customer Files Uploads & Product Attachments](https://market.x-cart.com/addons/files-uploads-product-attachments.html?sl=en&utm_source=XC5admin&utm_medium=addons_list_installed&utm_campaign=XC5admin "Adding products")" addon is active.

*   **Tags**: This field is only available if X-Cart's {% link "Product Tags" ref_6nFoxYf1 %} addon is active; it enables you to assign tags defined via the Product tags section (**Catalog** > **Tags**) to the current product.

*   **Available for sale**: Whether the product should be displayed on the storefront. Uncheck this option to temporarily remove the product from the storefront (Store visitors will not be able to see it).

    <a id="available-for-sale"></a>
    
    {% note info %}    
    If you disable the **Available for sale** option, the product will become inactive, and store visitors who will attempt to access the page of this product via a direct link will see the 404 "Page not found" error. If necessary, you can set redirects for the pages of disabled products using .htacces or the [Redirects Module](https://market.x-cart.com/addons/redirects-by-Nova-Horizons.html "Adding products"). 
  
    If you don't want to sell a product any longer but want a product page be still accessible on the storefront, set the product's stock to zero and add "Not available for sale" to the product name, rather than making it inactive. Make sure the _How to show out of stock products_ option is set to "Show in all the sections" in the **Store setup** -> **Cart & checkout** section of the admin area. 
    {% endnote %}
    
*   **Call for price**: This field is only available if X-Cart's {% link "Call For Price" ref_3K1pJExV %} addon is active; it enables you to specify that the price and Add to cart button must not be provided for the current product; instead, a message inviting store visitors to call for price should be displayed.

_Prices & Inventory_

*   **Memberships**: Membership levels to which this product should be available. Non-members and users belonging to other membership levels will not be able to see the product on the storefront. For more info on memberships in X-Cart, see the section {% link "User membership levels" ref_RXsgxNSm %} of this manual.

*   **Tax class**: The tax class to which the product belongs (Defines what taxes should be applied to the product). For more info on tax classes, see: {% link "Setting up tax classes" ref_pAWOdG8N %}.

*   **Price**: The product price.

*   **Market price**: This field is enabled by the [Market Price](https://market.x-cart.com/addons/market-price.html "Adding products") addon. It can be used to set a market product price showing the difference between the product price offered in your store and the average price of this product on the market. The market price is meant to show a customer how advantageous it is to order the product from your store. The market price is displayed next to the regular one on the product details page and in the product listing within a category. A sign showing the discount produced by the price difference is shown next to it to draw the attention of your site visitors.

*   **Sale**: Use this to put the product on sale.

*   **Arrival date**: This field allows you to record the date since when the product is or will be available in your store. On its own, the information entered in this field serves purely informational purposes, but may be employed by X-Cart modules (For example, a module that allows you to add a new product to your catalog in advance and let it be published on the storefront automatically when its arrival date is reached).

*   **Automatic reward points**: This field is only available if X-Cart's [Loyalty Program](https://market.x-cart.com/addons/loyalty-program.html?sl=en&utm_source=XC5admin&utm_medium=addons_list_installed&utm_campaign=XC5admin "Adding products") addon is active; it enables you to specify whether reward points for buying the current product should be calculated from the product price automatically or adjusted manually. With the "Automatic reward points" option disabled you will be able to set the number of points that a customer will earn by buying the current product via the **Reward points** field (appears when the "Automatic reward points" option is enabled).

*   **Inventory tracking**: Whether you wish to use the inventory tracking feature for this product. The inventory tracking feature enables you to specify the number of product units you have on hand initially (using the "Quantity in stock" field; see below); your X-Cart store will then track all the purchases of the product. Every time someone buys the product, the number in the "Quantity in stock" field will be reduced automatically by the number of units that have been purchased. If you have a stock refill, you edit the value in the  "Quantity in stock" field increasing the value by the number of units you require. As a result, you will be able to tell how many units of the product you have in stock at any time. If the product quantity is unlimited and does not need to be tracked, the inventory tracking feature can be disabled.

*   **Quantity in stock**: The current inventory level of the product (the number of product units in stock). The value specified in this field is used for the Inventory tracking feature.

*   **Available for backorder**: This field is only available if X-Cart's [Backorder / Preorder](https://market.x-cart.com/addons/backorder-preorder.html?sl=en&utm_source=XC5admin&utm_medium=addons_list_installed&utm_campaign=XC5admin "Adding products") addon is active; it enables you to specify that the current product can be purchased even when it is out of stock. After enabling the "Available for backorder" option, you will also be able to set a backorder label for the product and to limit the backorder quantity (see below).

*   **Backorder label**: This field is only available if the previous setting ("Available for backorder") is enabled. It allows you to add a message regarding the backordering of the current product which your store visitors will see attached to this product in product lists and on the product page when the product is out of stock. You can insert the number of units available for backordering into this message by using the "%number%" placeholder; for example: "You can backorder up to %number% items."

*   **Limit the backorder quantity**: This field is only available if the setting "Available for backorder" is enabled. It allows you to specify that only a limited number of units of the current product can be purchased on backorder, and to specify the maximum limit via the **Max. backorder quantity** field (appears when the "Limit the backorder quantity" option is enabled).

_Shipping_

*   **Weight**: Product weight.

*   **Requires shipping**: Whether this product requires shipping.

*   **Freight**: This field is enabled by the addon Free shipping and Shipping freights.

*   **Free shipping**: Whether the product should be shipped free of charge.

*   **Exclude from shipping cost calculation**:

*   **Separate box**: Whether the product needs to be shipped separately from other products. If it needs to be shipped in a separate box, you can define the box dimensions and the maximum number of product units that fit in this box.
    
_Marketing_

*   **Open Graph meta tags**: The custom META tags for sharing the product page on Facebook.

*   **Meta description**: The description to be used in the description META tag on the product page (for SEO purposes).

*   **Meta keywords**: The keywords to be used in the keywords META tag on the product page (for SEO purposes).

*   **Product page title**: The title to be used in the title bar of this product details page (for SEO purposes). 

*   **Clean URL**: The product page Clean URL (human-readable SEO-friendly URL, typically based on the product name). The URL can be configured manually (by editing of the field contents directly) or generated automatically (by enabling the "Autogenerate Clean URL" option below before saving the product). Note that if the Clean URLs feature is disabled, you will need to activate it for the SEO-friendly page URLs to become available to store visitors. More info on Clean URLs is available via the {% link "Setting up seo-friendly URLs" ref_nJxrzFEZ %} section of this manual.

## Advanced product setup 

Once a new product has been [added](#adding-a-new-product) to your store, you can edit any of its settings configured during the [basic product setup] and, if necessary, configure some advanced product settings for it as well. To do so, you will need to find the product in the store's Admin area (**Catalog** > **Products**) and click on the product name to access the product details. The result will be a page with all the information you have provided regarding this product so far - basically, the same page with the product information form you have completed during the basic product setup - but now this page will have tabs allowing you to access some additional sections for product configuration. The set of tabs that will be available to you will depend on your X-Cart edition and the set of addons activated in your store. Below is an overview of some of the popular tasks that can be accomplished by adjusting the advanced product settings via the various tabs of the product page - with information on what X-Cart addons/features you will require.

### Set additional Inventory tracking options

   * **Notify administrator if the stock quantity of this product goes below a certain limit**: X-Cart allows you to set a low stock threshold for each product and get automated email notifications whenever a product stock goes down to this level. To get low stock email notifications for this product, enable this setting. You will also need to specify the inventory level at which a notification needs to be sent (Use the "Low limit quantity" field below). 
   * **Low limit quantity**: Use this field to specify what product quantity should be considered "low". You will be notified when this quantity is reached.
    
### Specify additional product parameters 

If you want to specify additional parameters (like color, material, country of origin, ISBN, etc.) for the product so they can be viewed by your store visitors on the "Specification" tab of the product page, you will want to use X-Cart's {% link "Product classes and attributes" ref_T90ZcEpP %} feature. This feature is part of X-Cart's core and, if you just want the attributes, does not require any X-Cart addons. The attributes can be specified via the "Attributes" tab of the product page.

### Specify product options (color, size, etc.)

In X-Cart 5, product options can be configured based on product attributes. You add an attribute like "Size" and specify multiple attribute values for it like "XS", "S", "M", "L" and "XL". The buyer will then be able to choose the option they require. Some examples of how you can set product options based on attributes are provided in the article {% link "Managing attribute values" ref_bTfJ9bTS %}. For detailed information on product attributes, see {% link "Product classes and attributes" ref_T90ZcEpP %}.

### Set wholesale prices
"Wholesale" addon
"Wholesale pricing" tab - set price tiers for different user membership levels.
"Inventory tracking" tab - set minimum product purchase quantities for different user membership levels.
