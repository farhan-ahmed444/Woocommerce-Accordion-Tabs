In searching around the interwebs for a quick and easy way to replace the default woocommerce tabs with something a bit more sleak, I couldn't find anything. As I was already using Bootstrap for the project I was working on, I figured their accordion would be a good enough fit so I rewrote tabs.php to be an accordion. If you want to do the same, here's the code! 

As far as actually implementing this goes, don't hack the core of Woocommerce, but rather go into your custom theme or child theme and within a woocommerce directory containing all your woocommerce overwrites (for me it was in views for you it may be partials or elsewhere) and setup the directory structure as follows:

``` woocommerce/single-product/tabs/tabs.php ```

You can then stick the contents of this repo's tabs.php in there. 

In adding this, you'll want to pull the contents of the script tag out of the bottom and stick it wherever the JavaScript for your theme lives. 

You'll also want to do the same to the contents of the style tag, but stick it with your CSS.

Lastly, you'll need to be using bootstrap and jquery for this all to work. Someday, maybe I'll circle back and pull the accordion stuff out of bootstrap and add it to the script for this so that you don't have to use bootstrap for this to work. I'll probalby also replace the jQuery with Vanilla JS. 

Anyhow, I hope you find this helpful if you are in need and stumble accross it. Blessings!