# Pizza Yard Website

Files:
- index.html
- style.css
- script.js

## Formspree setup

1. Create a Formspree account at https://formspree.io/
2. Create a new form.
3. Set the form's destination/business email inside Formspree.
4. Copy the endpoint Formspree gives you. It looks like:
   https://formspree.io/f/xxxxxxxx
5. Open `script.js`.
6. Find:
   `formspreeEndpoint: "YOUR_EMAIL_SERVICE_ENDPOINT"`
7. Replace only the placeholder with your real endpoint.

Do not put email passwords or private API credentials in the website code.

## GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html`, `style.css`, and `script.js` to the repository root.
3. Open repository Settings → Pages.
4. Under "Build and deployment", choose "Deploy from a branch".
5. Select the main branch and `/ (root)`.
6. Save.
7. Wait for GitHub Pages to publish the site.

## Testing

Test:
- 1 topping = $20
- 2 toppings = $25
- 3 toppings = $28
- 4 toppings = $31
- 5 toppings = $34
- 6 toppings = $37
- quantity 2 + 2 toppings = $50
- quantity 3 + 2 toppings = $75
- quantity 3 + 2 toppings + delivery = $80
- quantity 3 + 3 toppings + delivery = $89
- pickup hides the delivery address
- delivery requires 3+ boxes
- delivery adds exactly $5
- invalid email is blocked
- invalid Saint Lucia phone is blocked
- successful Formspree submission stays on the website
- failed submission keeps the customer's entered information
- Place Order is disabled during submission
- mobile navigation and layout work without horizontal scrolling
