GetNetEZ customized ZendSkeletonApplication
===========================================

Introduction
------------
To create this version of the ZF2 Skeleton App, I created a new application on Zend Developer Cloud
[http://www.phpcloud.com/develop for a free account] and loaded the ZF2 Empty Zend Framework 2.x Application.

Once that was created,

    1. git cloned to my local dev
    2. installed the vendor modules I wanted in everything
    3. committed and pushed to github

Look for my upcoming series of video tutorials on this and more at http://getnetez.com

Enjoy

Installation
------------

Clone the repository and manually invoke `composer` using the shipped
`composer.phar`:

    cd my/project/dir
    git clone git://github.com/usulix/getNetEZ_Skeleton.git {optionally your_app_name instead of getNetEZ_Skeleton}
    cd getNetEZ_Skeleton {or your app name}
    php composer.phar self-update
    php composer.phar install

(The `self-update` directive is to ensure you have an up-to-date `composer.phar`
available.)

Virtual Host
------------
Afterwards, set up a virtual host to point to the public/ directory of the
project and you should be ready to go!

Bjy-Profiler
------------

The skeleton contains https://github.com/bjyoungblood/BjyProfiler and it will need to be configured or it will error out.

Create a file  /config/autoload/bjyprofiler.local.php and add the configuration contents as detailed at https://github.com/bjyoungblood/BjyProfiler under Configuration and use.

ZendDeveloperTools
------------

The skeleton project also includes https://github.com/zendframework/ZendDeveloperTools which does not require configuration. Without configuration, it will have no visual effect in your project... see https://github.com/zendframework/ZendDeveloperTools unders Installation step 3 for details on how to copy the configuration file from ./vendor/zendframework/zend-developer-tools/config/zenddevelopertools.local.php.dist to ./config/autoload/zenddevelopertools.local.php.
