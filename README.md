# Shopify Developer Challenge

Hi there, thanks for the opportunity.

# Description: 

## Following the instructions, 
I rendered the product data and created a simple product details page (PDP). I displayed the product title, description, images, variants, and variant prices. Additionally, I implemented JavaScript to dynamically update product or variant data, such as prices and slider images. I also used the Shopify "Add to Cart" AJAX API to add the product to the cart based on the selected variant ID and quantity input.

## Choices and Improvements: 
I chose to loop through the variants instead of looping through the product options. The reason is that the provided product data currently has only one option. If there were more than one option, or if this were a real Shopify store, I would loop through the product options instead of looping through the variants. After looping through the options, I would get the selected options array and compare it with the product variant options, which I would retrieve by sending a product API request using the product handle. Then, I would update the input with name="id" accordingly.

* Furthermore, I would use the Shopify product form with the product_form_id, method POST, and action /cart/add to add the product to the cart. *

If this were a real Shopify store, I would use the product form instead of sending an API request with JavaScript. Also, as mentioned, I would handle product options rather than looping through variants. For pricing, I have already applied Shopify's money filters.
