Facebook app:- See online friends while you chat is turned off 
=================================

This is simple require online_presence permmision to fetch the list of your online friend. There is not need to turn 
your chant on.

Run locally
-----------

Configure Apache with a `VirtualHost` that points to the location of this code checkout on your system.

[Create an app on Facebook](https://developers.facebook.com/apps) and set the Website URL to your local VirtualHost.

Copy the App ID and Secret from the Facebook app settings page into your `VirtualHost` config, something like:

    <VirtualHost *:80>
        DocumentRoot /Users/adam/Sites/myapp
        ServerName myapp.localhost
        SetEnv FACEBOOK_APP_ID 12345
        SetEnv FACEBOOK_SECRET abcde
    </VirtualHost>

Restart Apache, and you should be able to visit your app at its local URL.

[Demo] (https://apps.facebook.com/336197989828137/)
