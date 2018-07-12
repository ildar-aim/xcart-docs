---
lang: en
layout: article_with_sidebar
updated_at: '2016-09-30 13:20 +0400'
identifier: ref_xEadpu9F
title: Setting up volume discounts for products
categories:
  - User manual
published: true
order: 140
---

X-Cart 5 allows you to configure volume discounts. A volume discount may be expressed as a fixed amount or a percentage off the order subtotal amount. Unlike {% link "coupon discounts" ref_SGI1FqdC %}, volume discounts do not require your customers to enter any kind of secret code: a volume discount is applied automatically to any order that meets certain requirements. You define what these requirements should be. For example, you may create a discount that will be applied to orders with a subtotal amount equal to or greater than a certain amount, or will be applied to orders placed by users of a specific membership level.

When a volume discount is applied, the cart and checkout pages will show the discount amount on a separate line:
![xc5_volumedisounts_discount_in_customer.png]({{site.baseurl}}/attachments/ref_xEadpu9F/xc5_volumedisounts_discount_in_customer.png)

For purchases with a subtotal amount below the level needed to get a discount, a message like the following will be displayed:
![xc5_volumedisounts_get_discount_msg.png]({{site.baseurl}}/attachments/ref_xEadpu9F/xc5_volumedisounts_get_discount_msg.png)

The volume discounts feature in X-Cart 5 is enabled by the module **Volume Discounts**:
![mv_volumediscounts_addon.png]({{site.baseurl}}/attachments/ref_xEadpu9F/mv_volumediscounts_addon.png)

To use the volume discounts feature, make sure the module is installed and enabled at your store. If the module is not installed, you can install it from the X-Cart Marketplace. For general module installation instructions, see {% link "Installing modules from the Marketplace" ref_Vn1mMUw9 %}.

To configure a volume discount:

1.  In your store's Admin area, go to the Volume discounts section (**Promotions** > **Volume discounts**) and click **Add discount**:
    ![]({{site.baseurl}}/attachments/6389792/8719440.png)
    
    A section for adding a new discount will be displayed:
    ![]({{site.baseurl}}/attachments/6389792/8719441.png)
    
2.  Specify the parameters of your discount in the fields of the section that has appeared. 
    For example, we want to create a discount to let **all our customers** (regardless of their membership level) to get a **10% discount** on orders wth a total amount **equal to or** **greater than $100**. In this case we need to configure the discount parameters as follows:
    ![]({{site.baseurl}}/attachments/6389792/8719442.png)
    
3.  Once you are done, click the **Save changes** button.
    ![]({{site.baseurl}}/attachments/6389792/8719443.png)

The discount will be added:

![]({{site.baseurl}}/attachments/6389792/8719450.png)

If necessary, you can add more than one discounts for the different subtotal ranges and membership levels. For example, with a setup like in the following screenshot all our customers will get a 10% discount off orders with a subtotal amount of $100 or more, and a 20% discount off orders with a subtotal amount of $200 or more; customers of the membership level "Wholesaler" will get 30% off any order of $200 or more.

![]({{site.baseurl}}/attachments/6389792/8719452.png)

_Related pages:_

   * {% link "Volume Discounts: Usage with Multivendor" ref_117NpIm9 %}
   * {% link "Configuring volume discounts and coupons in X-Cart 5" ref_6xFWK5tC %} (video)
