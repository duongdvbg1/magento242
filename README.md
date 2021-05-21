I - Install theme test

1. Install a magento base 2.4.x
2. Copy source folder Webprovide to path "app/design/frontend"
3. Admin > Content > Configuration > Edit Default Store View and Choose Magento Default
4. Clear Cache

II - Requirements Tasks
1. On product listing page: move the filter navigation to right column. Change the product image when hover (like this https://www.made.com/storage/wardrobes)
- Reply: 
+ Change category page to right column. Filter auto move to right column. (Change file catalog_category_view.xml - layout="2columns-right")
+ Change images when hover. In Admin Panel > Product > Add images and choose image hover "Small".

2. Change the font for whole site to Montserrat
- Reply: Add google font Montserrat in default_head_blocks.xml and apply it in file web/css/source/_variable.less

3. Show recently viewed products slider on product detail page.
- Reply: 
+ Show Recently Veiwed Products in Admin > Content > Widget > Add Widget > Same screenshot ( https://prnt.sc/137pv6v )
+ Add slider libraries slick.min.js in requirejs-config.js and _slick.less in web/css/source/ import in _variable.less
+ Add slider to recently viewed products in file Magento_Catalog/web/template/product/list/listing.html