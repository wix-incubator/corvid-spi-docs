# Overview

Velo’s SPIs enable you to extend Velo’s functionality so that you can: 

+ **Inject your own custom business logic into existing business app flows**

   With Velo SPIs, you don't have to code a new flow from beginning to end if you want to customize and extend just one part of an existing business app's flow. You can implement the code just for the customized part.
   
   For example, the standard, out-of-the-box Ecommerce checkout flow calculates the total charge based on the order's line items. With Velo's Additional Fees SPI, you can inject the ability to add additional fees that apply to the entire order. Examples of additional fees include fees for fragile handling or surcharges for deliveries outside your regular delivery area.

+ **Integrate external services with your Wix site**

  Use the SPIs to integrate with external 3rd-parties so that your Wix site and the external services can communicate seamlessly. For example, different shipping rates from different external services can be displayed to the buyer during checkout. 

To use the Velo SPIs, you’ll need a working knowledge of JavaScript. When integrating with an external service, you'll need familiarity with the external service’s APIs.

For more details about extending Velo functionality using SPIs, see [Custom Business App Extensions Using SPIs](https://support.wix.com/en/article/velo-custom-business-app-extensions-using-spis-beta).