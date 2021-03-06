---
lang: en
layout: article_with_sidebar
updated_at: '2016-12-23 15:17 +0400'
identifier: ref_Ah935naM
title: Using the module "XC4 to XC5 Migration wizard"
order: 140
published: true
---
Once the module "XC4 to XC5 Migration wizard" has been installed on your X-Cart 5 store, you get a new item at the top of the Admin area menu - "Migration wizard":
    ![xc5_mw_menu_item.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_menu_item.png)

Click on it to launch the migation process:

##  Step 1 - Start
    
   At the first step of the wizard, select the check box to confirm that you understand the consequences of using the wizard (namely, that any existing data in your X-Cart 5 store will be overwritten as a result of the migration process). 
   Click **Start migration** to proceed:
   ![xc5_mw_step1_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step1_1.png)

##  Step 2 - Connect
    
   At the second step of the wizard, specify your X-Cart 4 store database connection details.
   ![xc5_mw_step2_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step2_1.png)

   Start by completing the following fields:
    
   *   **Database name**: The name of your X-Cart 4 database.
   *   **Database username**: The username of your MySQL account.
   *   **Database password**: The password of your MySQL account.
    
   If this set of fields is not enough to provide all the necessary connection details, please use the **Advanced options** section (expands at the click of the respective button): 
   ![wizard-advanced.png]({{site.baseurl}}/attachments/ref_Ah935naM/wizard-advanced.png)
    
   In the **Advanced options** section, you can enter the following info:
    
   *   **Host name**: The name of the host where your MySQL server is running.
   *   **Port number**: The port number to use for the connection, for connections made using TCP/IP. The default port number is 3306.
   *   **Socket**: The MySQL Unix socket.
   *   **Table prefix**: The table prefix used in your X-Cart 4 database (as was specified during X-Cart 4 installation). If you do not remember the table prefix that was used for your X-Cart 4 store, you can look it up in the file init.php of your X-Cart 4.x installation (in X-Cart versions 4.5.3 and later, see the value of `XC_TBL_PREFIX`; in earlier versions - the value of `xcart_tbl_prefix`). The default table prefix for all X-Cart 4 versions is `xcart_`.
    
   After specifying the above details, define the following settings:
   ![xc5_mw_step2_4.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step2_4.png)
    
   * Encryption key: Your X-Cart 4 store Blowfish key (the secret key needed for access to certain types of data stored in X-Cart 4 in encrypted form, such as user passwords). For more info on X-Cart 4 Blowfish key, see [X-Cart 4 manual](http://help.x-cart.com/index.php?title=X-Cart:Blowfish#Blowfish_key_based_encryption_method "X-Cart 4 manual").
   * Site URL: The URL of your X-Cart 4 store.
   * Site path: The site path of your X-Cart 4 store.
    
   Click **Save and continue**.

##  Step 3 - Check
    
   At the third step of the wizard, your X-Cart 5 store tries to connect to the specified X-Cart 4 database using the connection details provided at earlier. 
   
   Provided that the connection details have been specified correctly you should be able to see a summary of information that X-Cart 5 was able to obtain regarding the data that can be migrated from your X-Cart 4 store:
    ![xc5_mw_step3_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step3_1.png)
     
   The "Images size" item shows the amount of space taken by the X-Cart 4 store images (in Mbytes). If you are going to migrate the images, be sure to check that you have a sufficient amount of disk space on your X-Cart 5 store hosting for them.

   Click **Continue** to proceed.
    
##  Step 4 - Select
    
   At the fourth step of the wizard, you will see a list of data types that can be migrated from your X-Cart 4 store to X-Cart 5 ("What to transfer"), with check boxes.
   
   Use the check boxes to select the data types that you want to be migrated to X-Cart 5, then click **Save and continue**:
   ![xc5_mw_step4_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step4_1.png)

   If you wish to just try the migration in demo mode this time, select the **Demo migration** option at the top of the page:
   ![xc5_mw_step4_3.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step4_3.png)
    
   Click **Save and continue**.
    
   {% note info %}
   More info on Demo migration is available in the section {% link "How XC4 to XC5 Migration wizard works: Demo migration" ref_37NAeGlf#demo-migration %} of this manual.
   {% endnote %}
    
##  Step 5 - Enable
    
   At the fifth step of the wizard, X-Cart will provide you with a list of X-Cart 5 modules that should be enabled if the wizard detects that your X-Cart 4 installation has features that are lacking in the default X-Cart 5 distribution pack but can be added by enabling certain X-Cart 5 modules:
   ![xc5_mw_step5_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_1.png)

   Click **Enable and continue**.

   What happens next depends on whether your X-Cart 5 store is a trial installation or is using some kind of license (free or non-free).
    
   *  On a TRIAL installation, the module installer will activate all the required modules:
      ![xc5_mw_step5_3.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_3.png)
       
      If any paid modules are installed and activated at this step you will get a license warning with a list of affected modules after the store has been deployed:
      ![xc5_migration_wizard_enable4.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_migration_wizard_enable4.png)
       
      In this case, you have two options available:
        
       *   Activate a license required to use the modules;
       *   Remove the modules from your store.
    
       You may choose to resolve the licensing problem right away, or you may close the popup window with the warning and continue with the migration process. However, please be aware that the license warning will continue to appear in your X-Cart 5 store (both the store's back end and the storefront) until you resolve the problem with your license or remove the modules. 
       
       {% note info %}
       On our demo, we used a trial installation, so we got the first type of warning and chose to activate a license key for X-Cart Ultimate. After activating the key, we got a message at the top of the screen showing that the key has been activated successfully:
       ![xc5_migration_wizard_enable5.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_migration_wizard_enable5.png)
        
       This means that our licensing problem has been resolved, and we need to go back to our migration wizard to continue with the migration process:
       ![xc5_migration_wizard_enable6.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_migration_wizard_enable6.png)
       {% endnote %}
       
   *  On a LICENSED installation, the scenario of the wizard "Step 5 - Enable" will be a bit different after the **Enable and continue** button has been clicked. 
      
      If, after downloading the modules recommended for activation in your X-Cart 5 store, the module installer detects that these modules may not be used with your type of X-Cart license, you will get a license warning as follows:
      
      ![xc5_migration_wizard_license_type.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_migration_wizard_license_type.png)
       
       In this case, you will be able to resolve the problem using one of the following methods:
       
       *   Upgrade your X-Cart license to the license type allowed to use the modules;
       *   Remove the modules from your store.
    
       {% note info %}
       The modules will not be installed, and you will not be able to continue with the migration process until you resolve the problem with your license or remove the modules. 
       {% endnote %}
      
   
##  Step 6 - Transfer
    
   At the sixth step of the wizard, you can see a list of X-Cart entities that will be transfered from your X-Cart 4 store to the X-Cart 5 platform hence the migration wizard has collected all the information it requires and is ready to start the data migration process:
    ![xc5_mw_step5_5.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_5.png)
    
   If orders are going to be migrated, you will get an alert message regarding the currency being used: "The orders will be migrated using the current store currency (_Currency symbol - Currency name_). You can change the currency _here_." 
   
   You need to make sure your X-Cart 5 store is using the same currency as was used in the X-Cart 4 store. Use the link in the alert message to quickly access your X-Cart 5 store's currency settings (Store setup > Localization, Currency tab).

   {% note info %}
   If you want to migrate not all your X-Cart 4 orders, but just the latest orders starting from a specific date, it is possible to specify the date using the **Migrate orders from date** field:
   ![xc5_mw_step5_6.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_6.png)
   
   It is also possible to skip any X-Cart 4 store data that has already been migrated previously by enabling the **Skip previously migrated data** option:
   ![xc5_mw_step5_6_1.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_6_1.png)
    
   More info on this option is available in the section {% link "How XC4 to XC5 Migration wizard works: Skipping previously migrated data" ref_37NAeGlf#skipping-previously-migrated-data %} of this manual.
   {% endnote %}
    
   To start the migration, click **Start migration**:
   ![xc5_mw_step5_7.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_7.png)
 
   The migration process may take a while to complete and only continues while the page is open. Hence be sure to keep the page open or, if you have to close it for a while, be sure to re-open it to allow the migration module to finish its work.
   ![xc5_mw_step5_8.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step5_8.png)

   While your data is being migrated from your X-Cart 4 store to X-Cart 5, you will be able to see the progress on the screen. Here are the stages that will have to be completed:
    
   * _Migrating data..._
      Moving the selected types of data from X-Cart 4 to X-Cart 5.

   * _Processing products..._
      Updating product related quick data and other types of data related to products, like calculating the bestsellers statistics based on the migrated orders. 
    
   * _Processing categories..._
      Updating quick data for categories. Until this step has been completed properly, the category tree will not be displayed correctly. 
       
   * _Removing duplicate images..._
      Removing any duplicate product images (if any product images got duplicated as a result of the migration).

   The above stages will be included in any migration process - regardless of whether you are importing products/categories or not. If your X-Cart 5 store has products and categories, the processes run at these stages are simply necessary to ensure that your store looks and functions correctly.

   {% note info %}
   The module "XC4 to XC5 Migration wizard" now does not do the resizing of images. The stage "Resizing images..." which used to be included in the migration process by earlier versions of the module has been excluded. Now if you need to resize the images before going into production with your X-Cart 5 store, you can do the resizing using the **Generate resized images** feature in the **Look & Feel** > **Images** section.
   {% endnote %}

## Step 7 - Complete
   
   This is the final step of the wizard. Your data has been successfully migrated.
   ![xc5_mw_step6.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step6.png)
   
   <a id="add-label-to-signin-form"></a>
   
   {% note info %}
   Please keep in mind that starting from X-Cart Classic v4.5.x user passwords are not stored in the database. Hence the passwords can't be transferred savefy during the migration process and all users will have to use the **Forgot password?** option on the next login to the X-Cart 5 store in order to get in. 
   
   We'd recommend to add a special banner to the X-Cart 5 **Sign in** pop-up prompting the users to restore the password because of migration. A sample custom module that will add a label to the sign in form you can download [here](https://www.dropbox.com/s/pydh4uv15x7m783/XCMod-RestorePasswordAfterMigration-v5_3_0.tar?dl=0 "Using the module "XC4 to XC5 Migration wizard"").
   {% endnote %}

In some cases things may not go as smoothly as one would hope during the data migration procedure, e.g. PHP execution may be interrupted. Problems like that tend to be related to the time limit settings of the web server, especially if working on a server with limited resources or on a slow internet connection. If you experience errors causing mid-process interruption of the migration, be sure to increase your server time limit (See {% link "Setting the time limit of your server" ref_xqnpttd4 %}) or decrease the **migration_chunk_length** value in etc/config.local.php (See [How XC4 to XC5 Migration wizard works: Migration process](http://kb.x-cart.com/en/modules/xc4_to_xc5_migration_wizard/how_xc4_to_xc5_migration_wizard_works.html#migration-process "Using the module "XC4 to XC5 Migration wizard"")).

If you wish to do another migration (for example, finish migrating your X-Cart 4 data after testing the migration in the **Demo migration** mode), you can restart the migration wizard using the **Restart wizard** button:
   ![xc5_mw_step6_restart.png]({{site.baseurl}}/attachments/ref_Ah935naM/xc5_mw_step6_restart.png)
   
## Checklist before going live

This is a basic checklist to make sure everything is migrated correctly and your store is ready to go live.

- You can create a product, category, and user in the admin area;
- You can edit orders according to your needs;
- Home, category and product pages look properly in store-front;
- Search section in store-front can find the correct products;
- New customers can create a new account and existing customers can recover their passwords;
- Shipping methods are calculated properly on checkout. 
	- If you use online shipping calculators, make sure their credentials are filled in in Store setup > Shipping section. 
	- If you use different shipping rates for different destination zones, make sure that right shipping rates are applied to right zones in the same  Store setup > Shipping section;
- Payment methods are configured and can accept payments;
- All static pages are displayed properly and filled with proper content;
- All orders are migrated and up to date;
- Contact information is properly filled in Store Setup > Contact information section;
- If you want to use SMTP server for email notifications, set it up in Store setup > Email notifications > E-Mail transfer settings section;
- Migration Wizard does not transfer existing Gift Certificates and Testimonials. Make sure you have copied them from the X-Cart 4 store manually;
- Migration Wizard does not transfer any sales taxes or tax classes. Make sure you have configured them manually. (If you don’t see Sales Tax line in Taxes section - install free modules «Sales Tax» and «VAT Tax» in the «My Addons» section).

The points above are required to check before switching your existing store with X-Cart 5, but they are not limited to them. You may need to check other parts of the store depending on what functionality is heavily used by your clients.

   

_Related pages:_

   *   {% link "How XC4 to XC5 Migration wizard works" ref_37NAeGlf %}
   *   {% link "XC4 to XC5 Migration wizard system requirements and installation" ref_KqsCJNRG %}
