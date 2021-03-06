---
lang: en
layout: article_with_sidebar
updated_at: '2018-01-11 14:22 +0400'
identifier: ref_memberships_ext
title: Using Memberships
order: 100
published: true
description: memberships and products/categories/discounts/taxes/etc.
redirect_from:
  - /users/memberships_ext.html
---

{% toc %}

## Membership-specific Access to Products and Categories

In the section [Setting up wholesale prices and minimum purchase quantites for different membership levels](https://kb.x-cart.com/products/setting_up_wholesale_prices_and_minimum_purchase_quantites_for_different_membership_levels.html) of this manual you can find out how to set special prices for the customers who buy items in bulk. Allowing access to a certain product, group of products or product category based on membership level works a bit differently. Using this function you can grant access to specific products or categories only to certain members of your site and hide them from the rest of your site visitors. The hidden products and categories will still be indexed by Google, so this won't affect the ranks.

To hide a category and grant access to it only to certain store members:
    
   1. Go the the 'Catalog: Categories' section in the your store's Amin area.
   
   2. Choose the category you require and open it.
   
   3. Specify the membership(s) that should be able to access this category in the 'Memberships' field (Figure 1). Hold down the _**Shift**_ key to select multiple memberships. 
   
   4 Save your changes.

![Figure 1]({{site.baseurl}}/attachments/X Cart online store builder    Your company name    Manage category  Apparel.png)

The same needs to be done about the products in this category:
 
   1. Open the 'Catalog: Products' section in the Admin area.
   
   2. Filter the product list so it shows only the products from the category you require (the one you worked on at the previous step). This can be done by specifying the category name in the category selector (where it says 'Any Category') and clicking _**Search**_. (Figire 2)
      ![Figure 2]({{site.baseurl}}/attachments/Products.png)

   3. Scroll down the product list and select 'Bulk Edit' > 'Price and Membership' (Figure 3)
      ![Figure 3]({{site.baseurl}}/attachments/bulk edit.png)
      
      You will be redirected to a new page where you will be able to bulk edit product options. 
    
   4. Choose the 'Membersips' option and click to specify the membership(s) you need.
   
   5. Save your changes. (Figure 4)
      ![Figure 4]({{site.baseurl}}/attachments/membership.png)

That's all. The category and all the products in it are now hidden from any unregistered users. To be able to see this category or a product in it, a customer will need to be logged in and have a membership that we have specified as allowed to access this category/product.

If a non-member tries to open a members-only category page using a direct link, the store will show a `page not found` error. With a members-only product, the store will show an `access denied` error with a link to the 'Contact Us' page so the user can contact the store administrator and request the required membership. (Figure 5)
      ![Figure 5]({{site.baseurl}}/attachments/access.png)

Note that a store administrator can give membership to registered customers only (Access Level - Customer), but not to anonymous visitors. 

## Membership-specific Taxes

If some of your clients need to be given lower tax rates or have an exemption from paying the sales tax, you can adjust your store to meet this need by setting up tax rates specifically for different membership levels. 

To set membership-specific tax rates:
   
   1. Go to the 'Store Setup: Taxes' section of your store's Admin area to set up your tax.
   
   2. When adjusting the details of your tax, make sure the option 'Use the same tax rates for all user membership levels' is disabled.
   
   3. Create a new tax rate or edit an existing one specifying the required membership (Figure 6). 
   
   4. Be sure to save your changes. 
   ![Fig 6]({{site.baseurl}}/attachments/tax.png)

The detailed description of the tax configuration process is available in the section {% link "Setting up sales tax" ref_aJPK4DHN %} of this manual.


## Membership-specific Discounts, Coupons and Special Offers

By using memberships you can vary the discount level between different groups of customers, provide coupons of limited edition that will be valid only for a specific membership level, and extend membership sales with special offers.

Membership-specific discounts can be set up using the module **[Volume Discounts](https://market.x-cart.com/addons/volume-discounts.html)** via the section 'Discounts: Volume Discounts' of the Admin back end. More info on volume discounts is provided in the section {% link "Setting up volume discounts for products" ref_xEadpu9F %}. 

The process of setting up a membership-specific volume discount is rather straightforward:

   1. In the Volume discounts section of the store back end (**Discounts** > **Volume discounts**), choose to add a new discount.
   2. Specify the subtotal amount starting from which the discount will be available. 
   3. Set the discount amount (may be set as an absolute value or as a percentage)
   4. Choose the membership level that a customer must have to be able to use the discount (Figure 7). 
   5. Save your changes.
    
      ![Figure 7]({{site.baseurl}}/attachments/Screen Shot 2018-01-12 at 21.27.47.png)


Membership-specific coupons can be configured using the module **[Coupons](https://market.x-cart.com/addons/discount-coupons.html)** via the Coupons section of the store back end (**Discounts** > **Coupons**). More info on coupons is available in the section {% link "Setting up discount coupons" ref_SGI1FqdC %}. 

To configure a coupon that only members will be able to use, you will need to specify the membership(s) you require in the 'Membership' field (Figure 8). 

![Fig 8]({{site.baseurl}}/attachments/coupons.png)

If a non-member uses a members-only coupon at checkout, they will get an error message like the following: "Sorry, the coupon you entered is not valid for your membership level. Contact the administrator."

Special offers for members can be set up using the modules [Special Offers: Buy X Get Y](https://market.x-cart.com/addons/buy-x-get-y.html "Promote Sales with User Memberships") and [Special Offers: Spend X Get Y](https://market.x-cart.com/addons/spend-x-get-y.html "Promote Sales with User Memberships"). By using these modules, you will be able to provide such special offers to your member users as the following:
- Buy N items from specified categories to get a discount on M of them (the cheapest ones). If the discount is set to 100%, your customers will get the items for free. 
- Spend a certain amount in specified categories to get a discount on M of the items bought from these categories (the cheapest ones).

To configure the offers, you will need to have the modules installed as described in {% link "How to Install Modules in X-Cart 5" ref_fTUahl4n %}. Once the modules are installed, the features will become available in the 'Discounts: Special Offers' section of your store's Admin back end (Figure 9).
   ![Fig 9]({{site.baseurl}}/attachments/so.png)

To create an offer that will be available only to members:
   1. Start creating a special offer specifying all the necessary offer details. 
   2. In the 'Conditions' section of the special offer details, specify the membership level(s) to which the offer should be available. This can be done via the 'Eligible membership levels' field (Figure 10).
   ![Fig 10]({{site.baseurl}}/attachments/conditions.png)
   3. Save your changes.
   
For detailed information on the setup of special offers, refer to the section {% link "Special Offers" ref_special_offers %} in this manual.


## Membership-specific Payment Methods

With the module [Memberships for payment methods](https://market.x-cart.com/addons/memberships-for-payment-methods.html) you will be able to give additional payment options to certain groups of customers in your store; for example, to enable PayPal Express Checkout for wholesale buyers only. 

To enable the feature, install the module 'Memberships for payment methods' module first as described in {% link "How to Install Modules in X-Cart 5" ref_fTUahl4n %}. Once the module is installed, a special 'Memberships' field will appear under each payment method in the 'Store Setup: Payment Methods' section of your store's Admin area (Figure 11).
   ![Fig 11]({{site.baseurl}}/attachments/payment.png)

You'll need to use this field to specify the membership to which the payment method should be available (Figure 12). At checkout your customers will be able to see only the payment methods available to their membership group.
   ![Fig 12]({{site.baseurl}}/attachments/Screen Shot 2018-01-15 at 16.16.45.png)


## Paid Memberships

The standard membership feature can be extended using the module [Paid Memberships](https://market.x-cart.com/addons/paid-memberships.html). This module enables you to sell paid memberships as regular products. If your customers may be willing to pay for member access to advanced buying options - like closed sales, vip prices and exclusive discounts - this module may be just the thing for you.

To enable paid memberships, make sure the module is installed as described in {% link "How to Install Modules in X-Cart 5" ref_fTUahl4n %}. Once the module is installed, you will be able to create memberships as products and sell them to your customers. 

To create a paid membership:

   1. If you haven't yet done so, add the membership that you wish to offer to your customers as a paid one.
   
   2. Go to the '**Catalog** > **Products**' section of your store's Admin area and choose to add a new product (Figure 12).
      ![Fig 12]({{site.baseurl}}/attachments/add_product.png)
      
   3. On the page that opens, specify the product details as you require; for example, name, SKU, description, etc. - just like any regular product in your store. 
   
   4. To turn the product into a paid membership, use the setting **Membership to assign to product purchaser** to specify the membership that your customers will be able to get by purchasing the current product (Figure 13) and set the period for which the membership will be granted by adjusting the setting **Membership duration** (Figure 14).
      ![Fig 13]({{site.baseurl}}/attachments/Screen Shot 2018-01-15 at 19.31.27.png)
      ![Fig 14]({{site.baseurl}}/attachments/Screen Shot 2018-01-15 at 19.31.51.png)
      
   5. If necessary you can enable your existing members to purchase this membership at a special price and get a level up. The membership price for existing members can be adjusted via the **Prices & Inventory** section (Figure 15). 
      ![Fig 15]({{site.baseurl}}/attachments/Screen Shot 2018-01-15 at 19.37.44.png)

   6. Save the changes.

Once created, the paid membership will become available for sale and your customers will be able to purchase it (Figure 16).
   ![Fig 16]({{site.baseurl}}/attachments/product.png)

If anonymous checkout is enabled in the store, and a buyer of premium membership access chooses to check out without creating an account, the membership will not be assigned to that buyer automatically until an account  is created for them. The store administrator will be notified of such orders with an "action required" warning. 

After the order gets the status 'Paid', the customer will get the membership they have purchased automatically and will be able to access all the membership-specific privileges right away.

When the membership expires the customer will get an email notification. 

Email notifications for the **Paid Membership** module can be managed via the Email notifications section of the Admin area (**Store setup** > **Email notifications**).
   ![notifications.png]({{site.baseurl}}/attachments/ref_memberships_ext/notifications.png)
