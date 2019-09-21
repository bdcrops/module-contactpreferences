# BDC_ContactPreferences

This module is used as Customer Contact Preferences for all BDCrops Magento 2 extensions.



## 1. How to install & upgrade ContactPreferences


### 1.1 Copy and paste

If you don't want to install via composer, you can use this way.

- Download [the latest version here](https://github.com/bdcrops/module-contactpreferences/archive/master.zip)
- Extract `master.zip` file to `app/code/BDC/ContactPreferences` ; You should create a folder path `app/code/BDC/ContactPreferences` if not exist.
- Go to Magento root folder and run upgrade command line to install `BDC_ContactPreferences`:

```
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```


### 1.2 Install via composer

We recommend you to install BDC_ContactPreferences module via composer. It is easy to install, update and maintaince.Run the following command in Magento 2 root folder.

```
composer config repositories.module-contactpreferences git
https://github.com/bdcrops/module-contactpreferences.git

composer require bdcrops/module-contactpreferences:~1.0.0
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

#### 1.3 Upgrade    

```
composer update bdcrops/module-contactpreferences
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

Run compile if your store in Product mode:

```
php bin/magento setup:di:compile
```

## 2.  BDC_ContactPreferences

- create app/code/BDC/ContactPreferences/etc/module.xml
- create app/code/BDC/ContactPreferences/registration.php
- create app/code/BDC/ContactPreferences/etc/frontend/routes.xml
- create app/code/BDC/ContactPreferences/Controller/Contact/Preferences.php
- create app/code/BDC/ContactPreferences/Model/Entity/Attribute/Source/Contact/Preferences.php
- create app/code/BDC/ContactPreferences/Setup/InstallData.php  
- create app/code/BDC/ContactPreferences/etc/frontend/di.xml
- create app/code/BDC/ContactPreferences/CustomerData/Preferences.php
- create app/code/BDC/ContactPreferences/etc/frontend/sections.xml
- create app/code/BDC/ContactPreferences/view/frontend/layout/checkout_index_index.xml
- create app/code/BDC/ContactPreferences/view/frontend/layout/customer_account.xml
- create app/code/BDC/ContactPreferences/view/frontend/layout/customer_contact_preferences.xml
- create app/code/BDC/ContactPreferences/view/frontend/templates/customer/contact/preferences.phtml
- create app/code/BDC/ContactPreferences/view/frontend/requirejs-config.js
- create app/code/BDC/ContactPreferences/view/frontend/web/js/view/contact-preferences.js
- create app/code/BDC/ContactPreferences/view/frontend/web/template/contact-preferences.html

- Result
![](docs/ContactPrefAdmin.png)
![](docs/ContactPrefCuAcc.png)
![](docs/db.png)
##  Ref
