# Tag manager e-commerce datalayer

I've put this here in the hope it may save someone half an hour of googling.

Standard shopify gives you full control of your theme files until it gets to the payment gateway and the checkout process.
You can however inject code from within the admin, and get access to the full checkout object supplied in the liquid template.

[shopify checkout docs](https://help.shopify.com/themes/liquid/objects/checkout)

Navigate to shopify admin -> Settings -> Checkout

Scroll to 'Additional scripts' at the end of 'Order processing' section and paste the contents of [tag manager include](tag-manager-include.liquid)

_Disclaimer: This adds tag manager in the 'wrong' place, if you are using ta assistant to check it will compain, and trying to more than fir this event, you may run into issues, but for this purpose this doesn't seem to pose an issue._ 
