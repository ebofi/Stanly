# Stanly
This is a Simple Code for Magento 2 implementing Custom Attributes to Custom tabs in Product page


Installing this Module

Copy the files Stanly.zip to app/code/ and extract it. Now goto your magento admin and find the attribute name that you wish to show in custom tabs in the products listing page 
(front end). And open the file Stanly\incre\view\frontend\layout\catalog_product_view.xml

In that specify your attribute code by replacing the code demo on that.

Now on Magento SSH Cli
php bin/magento setup:db-schema:upgrade
php bin/magento setup:db-data:upgrade
php bin/magento cache:clean && php bin/magento cache:flush


Now you can see on your product details page the custom attribute you created is displaying as a Custom CMS block ( custom tab)

