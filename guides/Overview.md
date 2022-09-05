# Overview

Velo’s SPIs enable you to extend Velo’s functionality so that you can: 

+ **Inject your own custom logic into existing app flows**

   With Velo SPIs, you don't have to code a new flow from beginning to end if you want to customize and extend just one part of an existing app's flow. You can implement the code just for the customized part.
   
   For example, the out-of-the-box eCommerce checkout flow calculates the total charge for an order based on its line items. With Velo's [Additional Fees](https://www.wix.com/velo/reference/spis/ecom-additional-fees) SPI, you can inject the ability to add additional fees that apply to the entire order. Examples of additional fees include fees for fragile items or surcharges for deliveries outside your regular delivery area.

+ **Integrate external services with your Wix site**

  Use the SPIs to integrate with 3rd-party services so that your Wix site and the external services can communicate seamlessly. 
  
  For example, Velo's [Shipping Rates](https://www.wix.com/velo/reference/spis/ecom-shipping-rates) SPI lets you display shipping rates from different external service providers during checkout. Customers can then choose the shipping provider best for them. 

>**Note**: The Custom Extensions feature is currently a Beta release. Some custom extensions are not yet available to all users.

To use the Velo SPIs, you’ll need a working knowledge of JavaScript. When integrating with an external service, you'll also need familiarity with the external service’s APIs.

To learn more: 
+ [Velo: Custom App Extensions Using SPIs](https://support.wix.com/en/article/velo-custom-business-app-extensions-using-spis-beta)