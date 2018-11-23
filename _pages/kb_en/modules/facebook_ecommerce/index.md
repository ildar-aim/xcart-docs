---
lang: en
layout: article_with_sidebar
updated_at: '2017-11-16 01:48 +0400'
identifier: ref_LA0TBHEA
title: Facebook eCommerce Module
order: 95
published: true
---

Social feeds are a good point to attract new visitors and boost sales, Facebook Marketing being one of the most popular and efficient. If you have a Facebook account, you can start using X-Cart's free [Facebook Ads and Instagram Ads](https://market.x-cart.com/addons/facebook-e-commerce.html) module (formerly known as "Facebook eCommerce") right away. This module enables you to upload your products to Facebook Catalog and to create personalized ads that will allow reaching the right audience in the right place at the right time. Facebook ads are synchronized with Instagram and are shown there as well even if you don't have an Instagram account.

You can learn more about Instagram ads [here](https://www.facebook.com/business/help/1634705703469129?helpref=faq_content "Facebook eCommerce Module") and [here](https://www.facebook.com/business/help/1513393428972189?helpref=faq_content "Facebook eCommerce Module"). 

{% note info %}

If you don't have a Facebook account as yet, don't lose time and create it now at [https://www.facebook.com/business](https://www.facebook.com/business "Facebook eCommerce Module")

{% endnote %}

Facebook eCommerce module uploads your products to Facebook Catalog automatically and syncs the product data always keeping the catalog up-to-date. 

To make use of Facebook and Instagram ads you'll need to:
{% toc %}

## **Install the Facebook eCommerce module** 

Install the module as described in {% link "Installing addons from the Marketplace" ref_Vn1mMUw9 %}
  
  ![xc5_fecommerce_module_in_mktplce.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_module_in_mktplce.png)
  
Once installed the module will become available in the **Sales Channels** > **Facebook E-Commerce** section of the store admin area. 

Also, each product will gain an _Add to Facebook product feed_ setting in the Marketing section on the product details page that is enabled by default. All products with the enabled _Add to Facebook product feed_ setting will be automatically added to the product feed and uploaded to your Facebook Catalog.

## **Configure the module** 

  You can configure the Facebook e-Commerce module in the **Sales Channels** > **Facebook E-Commerce** section of the store admin area
  
  ![xc5_fecommerce_settings.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_settings.png)
  
  OR by clicking the **Settings** link when the module installation is complete.
  
  ![xc5_fecommerce_settings_link.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_settings_link.png)
  
  To configure the module you'll need to define the following settings:
  * Frequency of Product Feed renewal : hourly/daily/weekly
  * Facebook Pixel ID : Here you need to place your Facebook Pixel ID 
  
  {% note info %}
  If you don't have a Facebook Pixel ID yet, you can generate it as described at [https://www.facebook.com/business/help/952192354843755](https://www.facebook.com/business/help/952192354843755 "Facebook eCommerce Module"). 
  
  Facebook Pixel will allow tracking such events as _View Content/Search/Add to Cart/Initiate Checkout/Purchase_ and you can get stats on these events to work with sales funnel, ads conversion and so on.
  {% endnote %}
  
  When defined, click the **Generate Product Feed** button to get a link that you should use to upload the product feed to your Facebook Catalog
  
  ![xc5_fecommerce_generate_prod_feed_w_id.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_generate_prod_feed_w_id.png)
  
  It will take some time to generate a Product Feed URL depending on the overall store inventory. When completed copy a _Product Feed URL_ that has been generated and paste it when creating a new catalog at https://www.facebook.com/products/catalogs/new.
  
  ![xc5_fecommerce_url_generated.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_url_generated.png)
  
  {% note info %}
  The _Frequency of Product Feed renewal_ setting itself will not make renewals automatical. You'll need to set up console.php as described in {% link "Сonfiguring your server to run scheduled X-Cart tasks" ref_lLqNzAaq %}
  {% endnote %}
  
## **Upload Product Feed to Facebook**
  
  To upload your product feed to Facebook go to [Catalog Manager](https://www.facebook.com/business/help/1659534074121655 "Facebook eCommerce Module") of your [Facebook Business account](https://business.facebook.com/overview/ "Facebook eCommerce Module") at https://www.facebook.com/products/
  
  ![facebook-catalog.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/facebook-catalog.png)
  
  Click to create a new catalog or click an exisitng one to edit it, if it has no products as yet. 
  
  ![paste-product-feed.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/paste-product-feed.png)
  
  On the _Add Products_ step, choose 'Set on a schedule' for _How do you want to upload your data feed?_, paste your Product Feed URL that X-Cart generated for you in the **Add a Data Feed URL** field, schedule the automatic uploads and name the feed the way you like it better. Click the **Start Upload** button to upload your products from X-Cart to Facebook.
  
  When the products are uploaded, you'll see them in the **Products** tab.
  
  ![Products.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/Products.png)
  
That's it! You can start advertising your products through Facebook.

_Related pages:_

   * {% link "Sales Channels" ref_ybdJste8 %}
