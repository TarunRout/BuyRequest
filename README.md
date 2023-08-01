# BuyRequest
Introduction:-
The "BuyRequest" module is a custom Magento 2 module developed by Codilar that adds functionality related to Buy Request. The module allows customers to request a quote or ask for more information about a product before making a purchase. 

Approach:-
1. I have created a module with Vendor name as - Codilar, Module name as - BuyRequest
1. To remove Add to cart button and price. I have used reference in catalog_product_view.xml.
2. To add Buy Request button I have created a template custom_buttom.phtml.
3. To add pop up form, I used jquery inside the same phtml file in point 2.
4. After entering data, the data are stored in database which was created by db_schema and connected through model.
5. To display data in admin panel, I have created a separate menu as Buy Request with a sub menu Manage Request.
6. The data are displayed in grid which has been created by UI Component

Installation
To install the "BuyRequest" module, follow these steps:

1. Download or clone the module's codebase.

2. Create a new directory Codilar/BuyRequest in the app/code directory of your Magento installation.

3. Copy the downloaded files and paste them inside the app/code/Codilar/BuyRequest directory.

4. Run the following commands from your Magento root directory:
php bin/magento module:enable Codilar_BuyRequest
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
php bin/magento cache:clean

Configuration
After installing the "BuyRequest" module, there are no additional configurations required. The module automatically adds the necessary functionality to the product detail page, allowing customers to submit their buy requests.
