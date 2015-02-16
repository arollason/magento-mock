Zookal Mock Objects for Magento
===============================

##### TL;DR: Transparent auto-detecting of disabled core modules and extensions and providing mock objects for 
not breaking Magento. Nothing to configure. No class rewrites. Only one observer. Works out of the box.

If you try to disable e.g. Mage_Newsletter or Mage_Wishlist or ... and you call certain parts of the backend 
or some rare parts of the frontend you will get errors that Magento cannot find the class XYZ. Best examples 
are the two previously mentioned. If you have disabled them and you open in the backend a customer entry to 
edit it, the page will generate an error. Mage_Customer Edit has many dependencies with other modules. 
So the **Zookal Mock Module** will provide you mock objects which catches all method calls to disabled
classes of that modules without breaking anything.

### Continuous Integration

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/Zookal/magento-mock/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/Zookal/magento-mock/?branch=master)

[![Build Status](https://scrutinizer-ci.com/g/Zookal/magento-mock/badges/build.png?b=master)](https://scrutinizer-ci.com/g/Zookal/magento-mock/build-status/master)

Author
------

[Cyrill Schumacher](http://cyrillschumacher.com) - [My pgp public key](http://www.schumacher.fm/cyrill.asc)

Made in Sydney, Australia :-)