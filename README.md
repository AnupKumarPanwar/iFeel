Facebook Oauth + PHP in Ionic Framework
==============================


Download this example project from GitHub and run the following commands:

	$cordova platform add android
	$cordova plugin add cordova-plugin-inappbrowser
	$cordova plugin add cordova-plugin-whitelist
    $ionic run android

The above commands will add the Android build platform and install the required Apache InAppBrowser plugin.

This example application requires you to have your own Facebook application registered with Facebook.com.  Doing so
will give you a unique client id that can be included into your project.  When registering your application with Facebook,
make sure to set the callback uri to **http://localhost/callback**, otherwise ngCordova will not function.

With the client id in hand, open **www/js/app.js** and find the following line:

    $cordovaOauth.facebook("CLIENT_ID_HERE", ["email", "read_stream", "user_website", "user_location", "user_relationships"])

You will want to replace **CLIENT_ID_HERE** with the official key.




Resources
-------------

Ionic Framework - [http://www.ionicframework.com](http://www.ionicframework.com)

AngularJS - [http://www.angularjs.org](http://www.angularjs.org)

Apache Cordova - [http://cordova.apache.org](http://cordova.apache.org)

ngCordova - [http://www.ngcordova.com](http://www.ngcordova.com)

Nic Raboy's Code Blog - [https://blog.nraboy.com](https://blog.nraboy.com)
