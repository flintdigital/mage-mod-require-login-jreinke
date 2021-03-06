# A Magento module for requiring user authentication in frontend

![Magento Require Login](http://i.imgur.com/A9yU4SN.png)

## Installation

### Magento CE 1.6.x, 1.7.x, 1.8.x

Install with [modgit](https://github.com/jreinke/modgit):

    $ cd /path/to/magento
    $ modgit init
    $ modgit add mage-mod-require-login-jreinke git@github.com:flintdigital/mage-mod-require-login-jreinke.git

or download package manually:

* Download latest version [here](https://github.com/flintdigital/mage-mod-require-login-jreinke/archive/master.zip)
* Unzip in Magento root folder
* Clear cache
* Logout from admin then login again to access module configuration

Full overview available [here](http://www.bubblecode.net/en/2012/05/15/a-magento-module-to-require-login-on-your-store/).

## Configure

* Go to "System > Configuration > Bubble RequireLogin"
* Enable "Require Login" option
* Edit regular expression if needed __(do not forget to add your IPN urls otherwhise payment transaction cannot be completed)__
* To include the home page your regular expression will look like this `#(^/$|^$|customer\/account\/(log(in|out)|forgotpassword|resetpassword|create))#`

