# Shopify Interview Questions & Answers


---

### Table of Contents

<!-- TOC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [What is Shopify?](#What-is-Shopify) |
| 2 | [What is the difference between Shopify Online Store and older themes?](#What-is-the-difference-between-Shopify-Online-Store-and-older-themes) |
| 3 | [What are sections and blocks in Shopify?](#What-are-sections-and-blocks-in-Shopify) |
| 4 | [Explain Metafields vs Metaobjects.](#Explain-Metafields-vs-Metaobjects) |
| 5 | [How do you use dynamic sources in theme editor?](#How-do-you-use-dynamic-sources-in-theme-editor) |
| 6 | [How does Shopify handle multi-currency and multi-language stores?](#How-does-Shopify-handle-multi-currency-and-multi-language-stores) |
| 7 | [What is the difference between Shopify Themes and Shopify Apps?](#What-is-the-difference-between-Shopify-Themes-and-Shopify-Apps) |
| 8 | [How does Shopify hosting work (CDN, Liquid rendering, caching)?](#How-does-Shopify-hosting-work-CDN-Liquid-rendering-caching) |
| 9 | [Explain storefront vs admin side in Shopify.](#Explain-storefront-vs-admin-side-in-Shopify) |
| 10 | [What are limitations of Shopify themes compared to custom apps?](#What-are-limitations-of-Shopify-themes-compared-to-custom-apps) |
| 11 | [What is Shopify Liquid?](#What-is-Shopify-Liquid) |
| 12 | [Difference between objects, filters, and tags in Liquid.](#Difference-between-objects-filters-and-tags-in-Liquid) |
| 13 | [How do you output product price with currency?](#How-do-you-output-product-price-with-currency) |
| 14 | [How to display related products in Liquid?](#How-to-display-related-products-in-Liquid) |
| 15 | [How to check if a product is in stock?](#How-to-check-if-a-product-is-in-stock) |
| 16 | [How do you show customer-specific content (logged-in vs guest)?](#How-do-you-show-customer-specific-content-logged-in-vs-guest) |
| 17 | [Write Liquid code to show a rating metafield if available.](#Write-Liquid-code-to-show-a-rating-metafield-if-available) |
| 18 | [How to create a custom template in Shopify?](#How-to-create-a-custom-template-in-Shopify) |
| 19 | [How to implement pagination in a collection template?](#How-to-implement-pagination-in-a-collection-template) |
| 20 | [How to use forloop.index and forloop.last in Liquid?](#How-to-use-forloop-index-and-forloop-last-in-Liquid) |
| 21 | [Difference between Storefront API and Admin API.](#Difference-between-Storefront-API-and-Admin-API.) |
| 22 | [What is GraphQL Storefront API?](#What-is-GraphQL-Storefront-API) |
| 23 | [How do you fetch products via Storefront API using JS/React?]() |
| 24 | [What is a Private App vs Custom App?](How-do-you-fetch-products-via-Storefront-API-using-JS/React) |
| 25 | [Explain App Bridge and Polaris UI.](#Explain-App-Bridge-and-Polaris-UI) |
| 26 | [How do you authenticate with the Shopify Admin API?](#How-do-you-authenticate-with-the-Shopify-Admin-API) |
| 27 | [How to create a custom checkout UI extension?](#How-to-create-a-custom-checkout-UI-extension) |
| 28 | [How do you store and fetch custom metafields via API?](#How-do-you-store-and-fetch-custom-metafields-via-API) |
| 29 | [How to create a subscription app in Shopify?](#How-to-create-a-subscription-app-in-Shopify) |
| 30 | [Difference between Hydrogen (Headless) vs Liquid theme.](#Difference-between-Hydrogen-(Headless)-vs-Liquid-theme.) |
| 31 | [What is Shopify Plus?](#What-is-Shopify-Plus) |
| 32 | [Difference between Checkout.liquid and Checkout Extensibility.](#Difference-between-Checkout.liquid-and-Checkout-Extensibility) |
| 33 | [How do you add a custom discount box in checkout?](#How-do-you-add-a-custom-discount-box-in-checkout?) |
| 34 | [How do you implement post-purchase checkout extension?](#How-do-you-implement-post-purchase-checkout-extension) |
| 35 | [How to add checkout UI components with React?](#How-to-add-checkout-UI-components-with-React) |
| 36 | [How to customize checkout for B2B customers?](#How-to-customize-checkout-for-B2B-customers) |
| 37 | [Can you run custom scripts in checkout (discount, shipping)?](#Can-you-run-custom-scripts-in-checkout-discount,-shipping) |
| 38 | [What are Shopify Functions and how are they different from scripts?](#What-are-Shopify-Functions-and-how-are-they-different-from-scripts) |
| 39 | [Example use case of function for product discounts.](#Example-use-case-of-function-for-product-discounts) |
| 40 | [How do you implement custom shipping logic in checkout extensibility?](#How-do-you-implement-custom-shipping-logic-in-checkout-extensibility) |
| 41 | [How to update cart dynamically using AJAX API?](#How-to-update-cart-dynamically-using-AJAX-API) |
| 42 | [Explain the difference between cart/add.js and cart/update.js](#Explain-the-difference-between-cart/add.js-and-cart/update.js) |
| 43 | [How to implement a debounce search for products?](#How-to-implement-a-debounce-search-for-products) |
| 44 | [How to fetch products with fetch API in JavaScript?](#How-to-fetch-products-with-fetch-API-in-JavaScript) |
| 45 | [How to implement infinite scroll on collection page?](#How-to-implement-infinite-scroll-on-collection-page) |
| 46 | [How to validate discount codes before checkout?](#How-to-validate-discount-codes-before-checkout) |
| 47 | [How to use event delegation in Shopify cart?](#How-to-use-event-delegation-in-Shopify-cart) |
| 48 | [How do you handle variant change with JS?](#How-do-you-handle-variant-change-with-JS) |
| 49 | [How do you fetch and show reviews dynamically?](#How-do-you-fetch-and-show-reviews-dynamically) |
| 50 | [How to show recently viewed products using localStorage?](#How-to-show-recently-viewed-products-using-localStorage) |
| 51 | [What is Hydrogen in Shopify?](#What-is-Hydrogen-in-Shopify) |
| 52 | [How does Hydrogen + Oxygen hosting work?](#How-does-Hydrogen-+-Oxygen-hosting-work) |
| 53 | [How do you fetch product data using GraphQL in a Next.js app?](#How-do-you-fetch-product-data-using-GraphQL-in-a-Next.js-app) |
| 54 | [How to implement a cart system in headless Shopify?](#How-to-implement-a-cart-system-in-headless-Shopify) |
| 55 | [Difference between server components vs client components in Next.js.](#Difference-between-server-components-vs-client-components-in-Next.js) |
| 56 | [How to handle ISR/SSG/SSR in Next.js with Shopify?](#How-to-handle-ISR/SSG/SSR-in-Next.js-with-Shopify) |
| 57 | [How to implement Shopify checkout redirect in Next.js?](#How-to-implement-Shopify-checkout-redirect-in-Next.js) |
| 58 | [How do you manage global state (cart, auth) in React?](#How-do-you-manage-global-state-(cart,-auth)-in-React) |
| 59 | [How to implement lazy loading product images in React?](#How-to-implement-lazy-loading-product-images-in-React) |
| 60 | [How to handle SEO in a headless Shopify setup?](#How-to-handle-SEO-in-a-headless-Shopify-setup) |
| 61 | [How to implement wishlist functionality?](#How-to-implement-wishlist-functionality) |
| 62 | [How to build a custom product builder (personalization)?](#How-to-build-a-custom-product-builder-personalization) |
| 63 | [How to implement upsell / cross-sell sections?](#How-to-implement-upsell-cross-sell-sections) |
| 64 | [How do you build a mega menu in Shopify?](#How-do-you-build-a-mega-menu-in-Shopify) |
| 65 | [How to create a multi-store setup with shared data?](#How-to-create-a-multi-store-setup-with-shared-data) |
| 66 | [What are the biggest challenges you faced in Shopify development?](#What-are-the-biggest-challenges-you-faced-in-Shopify-development) |



<!-- TOC_END -->

<!-- QUESTIONS_START -->

1. ### What is Shopify?

    Shopify is a leading e-commerce platform that enables businesses to create online stores and sell products easily.

     - Shopify provides customizable templates for online stores, allowing businesses to create a unique brand presence.
     - It offers a user-friendly interface for managing products, orders, and customer data without needing extensive technical skills.
     - Shopify supports various payment gateways, making it easy for customers to complete transactions securely.
     - The platform includes built-in SEO features to help improve online visibility and attract more customers.
     - Shopify has a vast app ecosystem, allowing merchants to extend functionality with tools for marketing, inventory management, and analytics.  

    **[⬆ Back to Top](#table-of-contents)**

2. ### What is the difference between Shopify Online Store and older themes?

    🔹**Shopify Online Store 2.0:** 
        A modern theme architecture introduced by Shopify that allows merchants and developers to build highly customizable, modular, and performace storefronts. It supports sections on every page, app blocks, JSON templates, and dynamic content via metafields.

    🔹**older themes:** 
        Older Shopify themes built before Online Store 2.0. These themes are more hard, allowing sections only on the homepage, requiring manual code edits for app integration, and lacking support for dynamic data and modular templates.
    

    **[⬆ Back to Top](#table-of-contents)**

3. ### What are sections and blocks in Shopify?

    🔹**Sections in Shopify:**
        Sections are modular, customizable components that make up a page in a Shopify theme. They are the building blocks of page layout (e.g., header,  footer, product info, collection grid, slideshow).

    - **Types of Sections:**
        1. **Static Sections:-** Fixed on every page (e.g., header, footer).
        2. **Dynamic Sections:-** Can be added, reordered, or removed in the Theme Editor (e.g., image banner, product recommendations).

    - **File Structure:** Each section is a .liquid file inside the sections/ folder (e.g., sections/product.liquid).

    🔹 **Blocks in Shopify:**
        Blocks are sub-elements inside a section. They provide more smooth control within a section. Example: In a product section → blocks might include product title, price, buy button, description, reviews, etc.

    - **Usage:** Blocks allow merchants to reorder or toggle individual elements within a section from the Theme Editor.

    - **File Structure:** Blocks are defined in the section’s schema ({% schema %} JSON inside the section file).

    **Example (Product Section with Blocks):**

     ```javascript
    {% schema %}
        {
        "name": "Product information",
        "settings": [],
        "blocks": [
            {
            "type": "title",
            "name": "Product title"
            },
            {
            "type": "price",
            "name": "Product price"
            },
            {
            "type": "button",
            "name": "Add to cart button"
            }
        ],
        "presets": [
            {
            "name": "Default product info"
            }
        ]
        }
    {% endschema %}

     ```

    **[⬆ Back to Top](#table-of-contents)**

4. ### Explain Metafields vs Metaobjects.

    🔹**Metafields:**
        Metafields are custom fields that we store extra information about Shopify resources (like products, collections, orders, customers, etc.).
        Example: Material, size guide, care instructions, ISBN for books, expiry date, etc.

    - **Scope:** Attached to a specific resource (e.g., product.metafields.custom.material).
    - **Data Type Support:** Text, number, file, URL, boolean, date, JSON, reference, etc.
    - **Usage Example:**
            - Show a “Fabric Material” metafield on a product page.
            - Add a “Custom Badge” metafield to display “Bestseller” or “Limited Edition”.
    - **Best For:** When you want to store small, resource-specific, extra data.

    🔹**Metaobject:**
        Metaobjects are structured data models in Shopify, like a custom database table. They let you define reusable collections of data that can be linked across the store.

    - **Scope:** Independent objects that you define (like "Author", "Recipe", "FAQ", "Team Member"). Then you can reference them in multiple places.
    - **Structure:**
            - Each metaobject has fields (like columns in a table).
            - You can create multiple entries (like rows in a table).
    - **Usage Example:**
            - Create a “Team Members” metaobject → fields: Name, Photo, Role, Bio.
            - Create entries for each team member, then display them on an "About Us" page.
            - Create a “Size Guide” metaobject → reusable across multiple products.

    **[⬆ Back to Top](#table-of-contents)**

5. ### How do you use dynamic sources in theme editor?

    Dynamic Sources in Shopify Theme Editor allow you to connect theme settings with Shopify data like metafields or metaobjects. Instead of entering static values, merchants can dynamically pull data such as product material, custom images, or size guides directly from Shopify’s database. This makes themes more flexible and reduces the need for hardcoding or third-party apps.

    **How to Use (Step by Step):**

    1. **Define a metafield or metaobject** in your Shopify Admin.
        - Example: Products → Metafields → Add definition → Material (Text, Single line).
    2. **Open Theme Editor** (Customize → Select Product Page).
    3. Select a section/block (e.g., "Product description" block).
    4. In the settings, look for the dynamic source icon (🔗 small database icon).
    5. Click it → Shopify shows available metafields/metaobjects you can bind.
    6. Choose the metafield (e.g., Product > Material).
    7. Save → Now the value auto-populates from the metafield for each product.

    **Example in Liquid:**

    ```javascript

        {% if product.metafields.custom.material != blank %}
        <p class="product-material">
            Material: {{ product.metafields.custom.material }}
        </p>
        {% endif %}

    ```

    **[⬆ Back to Top](#table-of-contents)**

6. ### How does Shopify handle multi-currency and multi-language stores?  
    Shopify handles multi-currency through Shopify Payments and Markets, allowing customers to browse, checkout, and pay in their local currency with features like automatic conversion, rounding, and regional pricing. For multi-language, Shopify provides translation APIs, localization files, and Markets integration, enabling merchants to offer store content in multiple languages with native or app-based language switchers. Both features are managed under Shopify Markets, which unifies currencies, languages, and domains for global selling.

    **Multi-Currency How it Works in Themes (Frontend):**
    - Use Liquid money filters:

    ```javascript

        {{ product.price | money }}
        {{ 1000 | money_with_currency }}

    ```
    - Shopify automatically formats according to customer’s chosen currency.
    - Currency switchers can be implemented using:
     1. Shopify Markets selector (native)
     2. Shopify Geolocation app
     3. Custom selector using Liquid + JavaScript

    **Multi-Language How it Works in Themes (Frontend):**
    - Use localization variables in Liquid:

    ```javascript

        {{ 'products.product.add_to_cart' | t }}

    ```
    - Theme editor automatically pulls translations for supported languages.
    - Language switchers can be implemented with:
     1. Native selector (in Dawn and OS 2.0 themes)
     2. Custom dropdown linked to localization.locale

    **[⬆ Back to Top](#table-of-contents)**

7. ### What is the difference between Shopify Themes and Shopify Apps?

    **Shopify Themes:**
    A Shopify Theme is a collection of templates, layouts, and assets that define the visual design, structure, and user experience of a Shopify store. It controls how a store looks and feels to customers on the storefront.

    **Shopify Apps:**
    A Shopify App is software that extends a store’s functionality and business logic beyond what themes can do. Apps integrate with Shopify via APIs and can handle things like subscriptions, shipping, analytics, and third-party integrations. Unlike themes, which control the storefront design, apps handle features, automation, and backend logic.

    **[⬆ Back to Top](#table-of-contents)**

8. ### How does Shopify hosting work (CDN, Liquid rendering, caching)?
    Shopify is fully hosted and runs on a global CDN. All static assets (images, JS, CSS) are cached and delivered from the nearest edge location for speed. Liquid templates are rendered server-side, pulling store data and outputting HTML before it reaches the browser. Shopify also uses layered caching — assets, pages, and API responses — with automatic cache invalidation when data changes. This ensures stores are fast, secure, and scalable without merchants needing to manage hosting.

    **[⬆ Back to Top](#table-of-contents)**

9. ### Explain storefront vs admin side in Shopify.
    The storefront is the customer-facing side of Shopify where themes (Liquid, HTML, CSS, JS) control how products and pages are displayed. It focuses on the shopping experience. The admin side is the backend dashboard for merchants to manage products, orders, customers, and apps. It’s extended using the Admin API, Polaris, and App Bridge. In short, storefront = design & customer experience, admin = store management & business logic.

    **[⬆ Back to Top](#table-of-contents)**

10. ### What are limitations of Shopify themes compared to custom apps?
    Shopify themes are limited to frontend design and layout using Liquid. They cannot access the Admin API, automate workflows, or integrate with third-party services. Custom apps, on the other hand, can extend Shopify’s backend logic, use APIs, automate processes, and integrate external tools. In short, themes control how the store looks, while apps control what the store can do.

    **[⬆ Back to Top](#table-of-contents)**

11. ### What is Shopify Liquid?
    Shopify Liquid is a templating language used to build Shopify themes. It takes store data (products, collections, customers, etc.) and renders it into HTML for the storefront. Liquid provides objects, tags, and filters to display and format data. While powerful for presentation logic, it has limitations compared to apps (no direct API calls or complex logic).

    **How Liquid Works:**
    - Liquid has 3 main components:

    1. Objects → Output Shopify data

    ```javascript

        {{ product.title }}
        {{ cart.total_price | money }}

    ```
    2. Tags → Logic & control flow

    ```javascript

        {% if product.available %}
            In stock
        {% else %}
            Out of stock
        {% endif %}

    ```
    3. Filters → Modify output

    ```javascript

        {{ product.title | upcase }}
        {{ product.price | money_with_currency }}

    ```
    **[⬆ Back to Top](#table-of-contents)**

12. ### Difference between objects, filters, and tags in Liquid.
    In Liquid, objects are used to output Shopify store data, filters modify that data (formatting or transforming), and tags control logic and flow (conditions, loops, assignments).
    **Objects:**
    - Represent store data (products, collections, cart, customer, etc.).
    - Outputted using double curly braces {{ }}.
    - Think of them as variables that pull real data from Shopify.

    ```javascript

        {{ product.title }}         <!-- Outputs product name -->
        {{ cart.total_price }}      <!-- Outputs total cart price (in cents) -->

    ```
    **Filters:**
    - Modify or format the output of objects.
    - Placed after a pipe symbol |.
    - Can chain multiple filters together.

    ```javascript

        {{ product.title | upcase }} 
        <!-- Outputs product title in uppercase -->

        {{ product.price | money_with_currency }} 
        <!-- Formats price as $10.00 USD -->

    ```

    **Tags:**
    - Control logic and flow (conditions, loops, variables).
    - Written inside {% %} (curly + percentage signs).
    - Do not output data directly — they tell Liquid what to do.

    ```javascript

        {% if product.available %}
            In Stock
        {% else %}
            Out of Stock
        {% endif %}

        {% for product in collection.products %}
            {{ product.title }}
        {% endfor %}

    ```

    **[⬆ Back to Top](#table-of-contents)**

13. ### How do you output product price with currency?
    we output product price using the money or money_with_currency filters in Liquid.

    ```javascript

        {{ product.price | money_with_currency }}

    ```
    This will format the price and include the currency, like $19.99 USD.

    **[⬆ Back to Top](#table-of-contents)**

14. ### How to display related products in Liquid?
    There are three main ways to display related products in Liquid:
    - Show other products from the same collection.
    - Use Shopify’s Product Recommendations API (recommendations.products).
    - Use metafields (product reference) for manual selection.

     **[⬆ Back to Top](#table-of-contents)**

15. ### How to check if a product is in stock?
    In Shopify, inventory is tracked at the variant level (not the product level).
    **The key object is:**

    - variant.available → returns true if the variant is purchasable.
    - variant.inventory_quantity → returns the actual stock number (if inventory tracking is enabled).

    To check if a product is in stock, we use the available property.

     ```javascript

        {% if product.available %} In stock {% else %} Out of stock {% endif %}

    ```
    **[⬆ Back to Top](#table-of-contents)**

16. ### How do you show customer-specific content (logged-in vs guest)?
    In Shopify, we can show customer-specific content using the customer object in Liquid. This object only exists when the user is logged in, otherwise it’s nil. By wrapping content in `{% if customer %}` conditionals, we can separate experiences for logged-in vs guest users. For example, we can display a welcome message with the customer’s name, show exclusive discounts, or restrict certain content like wholesale pricing. Additionally, by checking `customer.tags`, we can create advanced personalization like showing VIP or wholesale-only content. This approach allows stores to deliver a more personalized shopping experience without needing third-party apps

    **[⬆ Back to Top](#table-of-contents)**

17. ### Write Liquid code to show a rating metafield if available.
    To display a rating metafield only if it exists, we check the metafield value in Liquid using `{% if product.metafields.namespace.key != blank %}`. For example, if we created a metafield custom.rating, 
    we can write:

    ```javascript

        {% if product.metafields.custom.rating != blank %}
        ⭐ {{ product.metafields.custom.rating }}
        {% endif %}

    ```
    This ensures that the rating appears only when a value is available. We can also enhance it by rendering star icons dynamically with a loop. This is a clean way to handle optional metafields without breaking the theme.

    **[⬆ Back to Top](#table-of-contents)**

18. ### How to create a custom template in Shopify?
    In Shopify, we create a custom template when we want a different layout for specific products, collections, or pages. To do this, we add a new template file inside `/templates` (e.g., `product.alternative.json`) and reference a custom section (like `/sections/product-alternative.liquid`). Then we design the section schema with customizable blocks. Finally, in Shopify Admin, we assign this new template to a product or page. This is very useful for product landing pages, wholesale layouts, or content-rich pages. With Online Store 2.0 JSON templates, we get much more flexibility compared to older `.liquid` templates because we can manage multiple sections directly in the editor.

    **[⬆ Back to Top](#table-of-contents)**

19. ### How to implement pagination in a collection template?
    To implement pagination in a collection template, we use the built-in Liquid `paginate` tag. For example, `{% paginate collection.products by 12 %}` will limit the products per page and automatically generate the `?page` parameter. Inside the paginate block, we loop over `collection.products`, and then use `paginate.previous`, `paginate.next`, and `paginate.parts` to render navigation links. This allows Shopify to handle large collections efficiently. We can further enhance this with AJAX-based pagination or infinite scrolling for better UX.

    **[⬆ Back to Top](#table-of-contents)**

20. ### How to use forloop.index and forloop.last in Liquid?
    In Liquid, when looping over a collection, we can use the special `forloop` object to get details about the iteration. For example, `forloop.index` gives the current iteration number starting at 1, and `forloop.last` returns true if the current item is the last in the loop. A common use case is printing numbered lists or avoiding a trailing comma in tag lists. For example, `{% unless forloop.last %}`, `{% endunless %}` ensures there’s no comma after the final item. Similarly, we can use `forloop.first` or `forloop.last` to apply special styles to the first or last elements in a grid.
    
    **[⬆ Back to Top](#table-of-contents)**

21. ### Difference between Storefront API and Admin API.
    The Storefront API is intended for customer-facing experiences — it’s GraphQL-based, uses storefront access tokens, and gives read access to catalog and customer data plus limited write operations for carts and checkouts. On the other hand, the Admin API is meant for merchant operations — it supports REST and GraphQL, uses secure admin tokens, and provides full CRUD capabilities for products, orders, inventory, and more. In short: Storefront API = frontend (headless, customers), Admin API = backend (merchants, store management)

    **[⬆ Back to Top](#table-of-contents)**

22. ### What is GraphQL Storefront API?
    The Shopify Storefront API is a GraphQL-based API that lets developers build custom, headless storefronts outside of Shopify’s Online Store. It’s optimized for customer-facing experiences, allowing access to products, collections, variants, carts, checkouts, and customer accounts. Since it’s GraphQL, developers can request only the data they need, making it efficient for mobile apps and modern frameworks like Next.js or Hydrogen. It uses a public Storefront Access Token and supports multi-currency and multi-language, making it ideal for global, headless commerce.

    **[⬆ Back to Top](#table-of-contents)**

23. ### How do you fetch products via Storefront API using JS/React?
    To fetch products via the Storefront API in JavaScript/React, I send a POST request to the `/graphql.json` endpoint with a GraphQL query. The request includes the Storefront Access Token in the headers. In React, I’d typically use `useEffect` and state to fetch and render products dynamically. Since the Storefront API is GraphQL, I can request only the fields I need, such as product title, images, and variant prices, which keeps the response lightweight and efficient.

    **[⬆ Back to Top](#table-of-contents)**

24. ### What is a Private App vs Custom App?
    A Private App was the older way to connect a single Shopify store with custom functionality using an API key and password, but it’s now deprecated because it lacked modern security. A Custom App is the new standard — still store-specific, but it uses OAuth authentication, can be developed using modern frameworks, and integrates securely with the Admin and Storefront APIs. In short, private apps were quick but insecure, while custom apps are the secure and supported way to build store-specific functionality today.

    **[⬆ Back to Top](#table-of-contents)**

25. ### Explain App Bridge and Polaris UI.
    Shopify App Bridge is a JavaScript SDK that allows my embedded app to integrate seamlessly with the Shopify Admin. It handles things like navigation, authentication, and showing modals or banners inside Shopify. Polaris, on the other hand, is a React component library that provides Shopify’s design system — buttons, cards, tables, forms — so the app looks consistent with Shopify Admin. In short, App Bridge is about functionality and integration, while Polaris is about UI and design.

    **[⬆ Back to Top](#table-of-contents)**

26. ### How do you authenticate with the Shopify Admin API?
    Shopify Admin API authentication is handled using OAuth 2.0 for public and custom apps. The app redirects the merchant for permission, exchanges an authorization code for an access token, and then uses that token in API requests via the X-Shopify-Access-Token header. For single-store integrations, Shopify provides a direct Admin API access token from the store’s developer settings. In embedded apps, session tokens (JWTs) are used to securely authenticate frontend calls. This ensures Shopify APIs are only accessible to authorized apps and merchants.

    **[⬆ Back to Top](#table-of-contents)**

27. ### How to create a custom checkout UI extension?
    To create a custom checkout UI extension, I use Shopify CLI to scaffold a new extension inside a custom app. It’s built with React and the Checkout UI Extension API. I define where it should render via `extension.config.yml`, and write React code using Shopify components like `Banner` or `TextField`. The extension runs in a sandboxed checkout environment, so it’s secure and upgrade-safe compared to old `checkout.liquid`. Once developed, I preview with `shopify app dev` and deploy with `shopify app deploy`. Then, the merchant can enable and place the extension inside Shopify’s Checkout Editor.

    **[⬆ Back to Top](#table-of-contents)**

28. ### How do you store and fetch custom metafields via API?
    Shopify metafields allow us to store custom data on resources. Using the Admin API, I can create metafields by specifying a namespace, key, type, and value. With REST, I POST to the `/metafields.json` endpoint under the resource, and with GraphQL I use `metafieldsSet`. To fetch them, I either query `/metafields.json` via REST or use GraphQL’s `metafields `field. Updates are made by calling `metafieldsSet` again or PUT on REST, and deletions via DELETE or `metafieldDelete`. This gives merchants the flexibility to store custom attributes beyond Shopify’s standard schema.

29. ### How to create a subscription app in Shopify?
    A subscription app in Shopify is built using the Subscription APIs and Checkout UI Extensions. The app creates selling plan groups (like weekly or monthly billing) and attaches them to products. During checkout, the app surfaces subscription options via extensions, and after purchase, Shopify generates a subscription contract that my app can manage (pause, cancel, update). I’d build the app using Remix or Node, authenticate via OAuth, and store contract/customer data in my DB for better customer portals. This setup lets merchants run recurring revenue businesses directly inside Shopify’s checkout.

    **[⬆ Back to Top](#table-of-contents)**

30. ### Difference between Hydrogen (Headless) vs Liquid theme.
    Liquid themes are Shopify’s traditional templating approach where the frontend is tightly coupled with Shopify’s backend. They’re easy to customize with the theme editor and great for most merchants. Hydrogen, on the other hand, is Shopify’s React-based headless framework that uses the Storefront API. It gives developers complete freedom to build custom experiences, integrate external systems, and optimize performance with SSR/streaming. However, Hydrogen is developer-heavy and doesn’t have the drag-and-drop editor that merchants love in Liquid. In short, Liquid is best for standard Shopify stores, while Hydrogen is best for complex, enterprise, or highly customized commerce experiences.
    1. Static Site Generation (SSG)
    - When to use:
        - For pages that don’t change often (e.g., product listing, homepage, about page).
        - Data fetched at build time.
        - Great for performance + SEO.
    - How:
        - Use getStaticProps in Next.js (if using pages/) OR fetch with cache: 'force-cache' in App Router.
        - Example: Fetch Shopify products at build time

    2. Incremental Static Regeneration (ISR)
    - When to use:
        - Products/prices change frequently, but don’t need real-time updates.
        - Example: Product catalog pages.
        - Rebuild specific pages in the background after a time interval.
    - How: Add revalidate in App Router or getStaticProps.
    - Example: ISR with Shopify product detail page

    3. Server-Side Rendering (SSR)
    - When to use:
        - Content changes per request (e.g., personalized prices, B2B discounts, logged-in customer cart).
        - Checkout-related pages.
    - How: Use cache: "no-store" or fetchCache: "force-no-store".
    - Example: SSR with customer-specific cart

    **[⬆ Back to Top](#table-of-contents)**

31. ### What is Shopify Plus?
   Shopify Plus is the enterprise version of Shopify designed for large brands and high-volume merchants. It offers advanced features like customizable checkout via extensions, higher API limits, automation tools such as Flow and Launchpad, built-in B2B support, and unlimited staff accounts. Plus merchants also get dedicated support and expansion stores for international commerce. Essentially, Shopify Plus is best suited for businesses that need scalability, deep customization, and enterprise-grade performance. 

   **[⬆ Back to Top](#table-of-contents)**

32. ### Difference between Checkout.liquid and Checkout Extensibility.
    Previously, Shopify Plus merchants used checkout.liquid to customize their checkout by editing Liquid templates directly. While this gave full control over layout and styling, it was risky, hard to maintain, and is now deprecated. Shopify has replaced this with Checkout Extensibility, which uses UI extensions, Functions, and Pixels to safely customize checkout in a structured, app-based way. Extensibility ensures customizations are upgrade-safe, works with one-page checkout and Shop Pay, and allows apps to extend checkout securely. While checkout.liquid offered more direct control, Checkout Extensibility is the modern, scalable, and future-proof approach.

    **[⬆ Back to Top](#table-of-contents)**

33. ### How do you add a custom discount box in checkout?
    To add a custom discount box in Shopify checkout, we can no longer inject fields with `checkout.liquid` since it’s deprecated. Instead, we use `Checkout Extensibility`. I’d create a Checkout UI Extension in React, place it at a checkout extension point, and use the `useApplyCartDiscountCodeChange` hook to let customers enter and apply a discount code. If we need advanced logic (like custom eligibility or tiered discounts), we’d combine this with a Shopify Discount Function. This approach is upgrade-safe, works with one-page checkout, and fully integrates into Shopify’s discount system.
    **Steps to Implement:**
    - Create a Shopify app (using Remix/CLI).
    - Add a Checkout UI Extension.
    - Register the extension in shopify.app.toml.
    - Deploy and enable it in Shopify Admin → Checkout Editor.
    - (Optional) Add a Discount Function if business logic requires.

    **[⬆ Back to Top](#table-of-contents)**

34. ### How do you implement post-purchase checkout extension?
    I did scaffold a Post-purchase UI extension with the Shopify CLI, target `purchase.post-purchase.render`, and build a React component that reads the order context, presents an upsell, and—on accept—applies a cart line change to charge the same payment method. I expose merchant settings (variant, copy), preview with `shopify app dev`, then deploy and enable it in the Checkout Editor. I keep it lean, idempotent, and instrumented for analytics since it runs between payment and the Thank-you page.

    **[⬆ Back to Top](#table-of-contents)**

35. ### How to add checkout UI components with React?
    To add checkout UI with React, I did scaffold a Checkout UI extension using Shopify CLI, choose a target like `Checkout::Dynamic::Render`, and use `@shopify/ui-extensions-react/checkout` components. For example, adding a `TextField` for a gift note. To persist data, I’d use useApplyAttributeChange so the note is saved as a checkout attribute and appears in the order. Finally, I’d preview with `shopify app dev`, then deploy and place the extension in the Checkout Editor. I’d keep UX minimal and validated since checkout is a critical funnel step.

    **[⬆ Back to Top](#table-of-contents)**

36. ### How to customize checkout for B2B customers?
    For B2B checkout, Shopify Plus provides dedicated tools. I’d first detect if the logged-in customer belongs to a company using the Checkout UI Extension API (useCustomer). Then, I can render custom fields like a Purchase Order number, VAT ID, or Terms acknowledgment. Using Shopify Functions, I’d enforce B2B rules like Net 30 payment terms or custom shipping rates. With Checkout Branding API, I can visually separate B2B checkout styling. This way, consumer customers get the standard checkout, while business buyers see a tailored, compliance-friendly experience.

    **[⬆ Back to Top](#table-of-contents)**

37. ### Can you run custom scripts in checkout (discount, shipping)?
    In the old checkout.liquid world, Plus merchants could run custom Ruby scripts in the Script Editor for discounts, shipping, and payments. With Checkout Extensibility, Shopify has replaced free-form scripts with Functions and Checkout UI Extensions. Functions allow us to write discount, shipping, and payment logic in a safe, scalable way, while Checkout UI Extensions let us add UI elements. This ensures checkout remains secure, upgrade-safe, and works with Shop Pay. So, while we can’t inject raw scripts anymore, we achieve the same (and more) with Functions and Extensions.

    **[⬆ Back to Top](#table-of-contents)**

38. ### What are Shopify Functions and how are they different from scripts?
    Shopify Scripts were Ruby-based checkout customizations available only to Plus merchants, but they’re being deprecated because they weren’t scalable, upgrade-safe, or shareable across stores. Shopify Functions replace them — they let us write discount, shipping, and payment logic in Rust or TypeScript, compiled to WebAssembly, and run natively inside Shopify’s backend. The big advantage is that Functions are faster, more secure, version-controlled, and deployable via apps, making them the future-proof way to customize checkout.

    **[⬆ Back to Top](#table-of-contents)**

39. ### Example use case of function for product discounts.
    With Shopify Functions, I can implement complex discount rules like Buy X Get Y, tiered pricing, or customer-specific discounts. For example, I built a ‘Buy 2 T-Shirts Get 1 Free’ function where I filter cart items by product type, sort them by price, and apply a 100% discount on the cheapest one. Unlike the old Ruby-based Scripts, Functions are packaged as apps, reusable, and run directly inside Shopify’s checkout pipeline, making them fast, secure, and upgrade-safe.

    **[⬆ Back to Top](#table-of-contents)**

40. ### How do you implement custom shipping logic in checkout extensibility?
    To implement custom shipping logic in Checkout Extensibility, I’d use a Delivery Customization Function. For example, to provide free shipping over ₹2000, I’d check the cart’s total inside my function and adjust the price of ‘Standard Shipping’ to 0. Similarly, I can hide or rename rates—for instance, hiding COD for US addresses. If I want to show contextual messages to the buyer, I can combine this with a Checkout UI Extension using React, displaying a banner like ‘Congrats, Free Shipping Unlocked.’ Unlike checkout.liquid or Ruby scripts, Functions run natively in Shopify’s checkout pipeline, are upgrade-safe, and work with Shop Pay.

    **[⬆ Back to Top](#table-of-contents)**

41. ### How to update cart dynamically using AJAX API
    Shopify provides an AJAX API that allows updating the cart dynamically without a page reload. For example, when a customer changes quantity in a cart drawer, I can call /cart/change.js with the line item key and new quantity. The API returns the updated cart JSON, which I use to re-render my UI. This approach improves UX significantly compared to the default cart page. It’s important to handle edge cases like stock limits, and to debounce input changes to avoid excessive API calls.

    **[⬆ Back to Top](#table-of-contents)**

42. ### Explain the difference between cart/add.js and cart/update.js
    The difference is that `/cart/add.js` is used to add a single product variant to the cart. If the item is already present, it increases the quantity. It only returns the added line item JSON. On the other hand, `/cart/update.js` is used to update multiple line items in bulk. It requires a map of variant IDs and their new quantities, and it returns the full cart object. In short, `add.js` is for adding, while `update.js` is for setting quantities across the cart.

    **[⬆ Back to Top](#table-of-contents)**

43. ### How to implement a debounce search for products?
    I did implement a debounce wrapper around my API call, use Shopify’s predictive search or Storefront API to fetch products, and display results in a dropdown. This ensures efficiency, avoids unnecessary API calls, and provides a smooth user experience.
    **Key Interview Talking Points**
    - Why debounce is important: improves performance, prevents API throttling.
    - Where to use: search bars, autocomplete, input validations.
    - Typical delay: 300–500ms for best UX.
    - Shopify-specific:
        - Use Predictive Search API for Online Store.
        - Use Storefront GraphQL API for headless/React builds.
    
    **Steps to Implement Debounced Product Search**
    1. Choose Data Source:
        - If you’re working with a Shopify Online Store theme, use Shopify’s Predictive Search API `(/search/suggest.json)` to fetch live product results.
        - If you’re working in a headless storefront (React, Next.js, Hydrogen), use the Storefront API (GraphQL).
    2. Create a Debounce Function

         ```javascript
        function debounce(func, delay) {
            let timer;
            return function(...args) {
                clearTimeout(timer);
                timer = setTimeout(() => func.apply(this, args), delay);
            };
        }
         ```
    3. Attach Debounce to Search Input
        - Wrap the API call with debounce().
        - Example with /search/suggest.json:

        ```javascript
        const searchInput = document.querySelector('#searchInput');
        searchInput.addEventListener('input', debounce((e) => {
        fetch(`/search/suggest.json?q=${e.target.value}&resources[type]=product`)
            .then(res => res.json())
            .then(data => console.log(data));
        }, 300));
        ```
    4. Render Results Dynamically
        - Show product title, image, and link in a dropdown list.
        - Handle empty query ("") and “no results” gracefully.

    **[⬆ Back to Top](#table-of-contents)**

44. ### How to fetch products with fetch API in JavaScript
    I use the Fetch API to get product data from Shopify’s /products.json or Predictive Search API for theme-side work. For headless or advanced use cases, I use the Storefront API with GraphQL. The choice depends on whether I’m working on a public storefront or a private app.
    **Key Interview Points**
    - Use /products.json for theme/public data.
    - Use Predictive Search API for search/autocomplete.
    - Use Storefront API (GraphQL) for headless apps.
    - Use Admin API only for private backend apps (not public JS).
    - Fetch API works with fetch(url, {method, headers, body}) and returns a Promise.

    **[⬆ Back to Top](#table-of-contents)**

45. ### How to implement infinite scroll on collection page?
    infinite scroll in Shopify is implemented by combining Liquid pagination with JavaScript fetch calls. Liquid provides the next page URLs, and JavaScript dynamically loads and appends new product cards. I also ensure normal pagination links exist as fallback for SEO and accessibility.
    **Key Interview Points:**
    - Shopify Liquid handles pagination, JavaScript handles infinite scroll logic.
    - Use paginate object for next.url.
    - Use AJAX (Fetch API) to load next pages without refreshing.
    - Intersection Observer is preferred over scroll event (better performance).
    - Always consider SEO & accessibility: keep normal pagination as fallback.

    **[⬆ Back to Top](#table-of-contents)**

46. ### How to validate discount codes before checkout?
    Since Shopify doesn’t validate discount codes on the cart page by default, I usually implement a custom discount form. When a customer enters a code, I send it to a backend app that uses the Admin API to validate it against active price rules. If valid, I store it in cart attributes and redirect to checkout with ?discount=CODE. This ensures customers know upfront whether a code is valid, improving UX and reducing checkout drop-offs

    **[⬆ Back to Top](#table-of-contents)**

47. ### How to use event delegation in Shopify cart?
    In Shopify’s AJAX cart, I always prefer event delegation. Instead of binding listeners to every quantity input or remove button, I attach a single listener to the cart container. This way, even when cart items are dynamically added or removed via AJAX, the events continue to work without re-initialization. It improves performance, reduces memory leaks, and makes the cart logic more maintainable.
    **Why Event Delegation is Useful in Shopify Cart?**
    - Dynamic content: Cart items are added/removed without full page reload. Delegation ensures new buttons/inputs work automatically.
    - Performance: Only one event listener instead of one per item.
    - Maintainability: Cleaner code, easier to scale for many cart actions.

    **[⬆ Back to Top](#table-of-contents)**

48. ### How do you handle variant change with JS?
    In Shopify, I usually expose the product JSON using Liquid, then use JavaScript to listen for variant changes (from dropdowns or radio buttons). Once the user selects an option, I find the matching variant object, update price, availability, SKU, and the add-to-cart button dynamically. I also update the hidden input variant ID so the correct variant is passed to `/cart/add.js`. This ensures a smooth UX similar to Shopify’s Dawn theme.

    **[⬆ Back to Top](#table-of-contents)**

49. ### How do you fetch and show reviews dynamically?
    Shopify does not natively handle reviews, so I either use metafields/metaobjects (for simple internal reviews) or integrate a 3rd-party review app (like Judge.me, Yotpo, Stamped). To make reviews dynamic, I fetch them via API or expose metafield JSON in Liquid, then use JavaScript to render them with pagination or 'Load more' functionality. In custom apps, I typically build an app proxy endpoint to return reviews as JSON, ensuring they can be dynamically loaded on the product page without full page reloads.

    **[⬆ Back to Top](#table-of-contents)**

50. ### How to show recently viewed products using localStorage?
    I would implement recently viewed products by leveraging localStorage to store product handles as customers browse. On each product page, I push the handle into a localStorage array (avoiding duplicates and limiting length). Then, on any page where I want to show recently viewed products, I read from localStorage, fetch product details from `Shopify’s /products/{handle}.js` endpoint, and dynamically inject them into the DOM. This approach is lightweight, doesn’t require backend changes, and works well for personalization.

    **[⬆ Back to Top](#table-of-contents)**

51. ### What is Hydrogen in Shopify?
    Hydrogen is Shopify’s React-based headless framework designed specifically for building custom storefronts. Unlike Liquid themes, which are template-driven, Hydrogen gives developers full flexibility to create unique eCommerce experiences using React, GraphQL (Storefront API), and server-side rendering. It comes with commerce-optimized components, hooks, and deployment via Oxygen, making it ideal for high-performance, modern, and highly customized online stores.

    **[⬆ Back to Top](#table-of-contents)**

52. ### How does Hydrogen + Oxygen hosting work?
    Hydrogen is the React framework for building headless storefronts, while Oxygen is Shopify’s global hosting platform that serves these storefronts at the edge. Together, they allow developers to build high-performance, fully customized commerce experiences with React, powered by Shopify’s APIs, and delivered with the scalability, speed, and security of Shopify’s infrastructure. The key advantage is that you get the flexibility of a headless setup without managing your own hosting or servers.
    **Example Flow (User Journey)**
    - User visits Hydrogen storefront → request goes to Oxygen edge server nearest to them.
    - Oxygen server renders the page using Hydrogen SSR.
    - Static content is cached at the edge, dynamic parts are fetched from Storefront API.
    - Page streams back to user — product title, price load first → images, reviews load after.
    - Checkout still happens via Shopify’s hosted checkout (extensible via Checkout UI extensions).

    **[⬆ Back to Top](#table-of-contents)**

53. ### How do you fetch product data using GraphQL in a Next.js app?
    In a Next.js app, I connect to Shopify’s Storefront GraphQL API using the storefront access token. I structure a GraphQL query to fetch product fields like title, handle, price, and images. Depending on use case, I fetch this data in `getStaticProps` (SSG) for performance, or `getServerSideProps` (SSR) for real-time updates. This approach gives me full control of rendering Shopify data inside a custom React storefront.
    **Key Interview Talking Points**
    - Storefront API requires Storefront token (not Admin token).
    - Use GraphQL queries instead of REST for efficiency (fetch multiple fields in one request).
    - Choose SSR (getServerSideProps) when product data changes frequently (like prices, stock).
    - Choose SSG (getStaticProps) + revalidation for performance and SEO.
    - Can integrate with Apollo Client or Urql for client-side fetching if needed.

    **[⬆ Back to Top](#table-of-contents)**

54. ### How to implement a cart system in headless Shopify?
    To implement a cart in headless Shopify, I use the Storefront GraphQL API. I create a cart with `cartCreate`, persist its ID in localStorage, and manage items using `cartLinesAdd`, `cartLinesUpdate`, and `cartLinesRemove`. For checkout, I redirect to Shopify’s `checkoutUrl`. This gives me full control of cart UI in React/Next.js while leveraging Shopify’s secure checkout.
    **Key Interview Talking Points**
    - In headless Shopify, the cart is built entirely with Storefront API mutations.
    - The cartId is persisted client-side (localStorage / cookie).
    - Cart is always tied to Shopify checkout (you can’t replace checkout without Plus).
    - You can extend functionality:
        - Apply discounts (cartDiscountCodesUpdate)
        - Attach logged-in customers (cartBuyerIdentityUpdate)
        - Manage shipping address (cartBuyerIdentityUpdate)

    **[⬆ Back to Top](#table-of-contents)**

55. ### Difference between server components vs client components in Next.js.
    In Next.js App Router, all components are Server Components by default. They run only on the server, can fetch data securely, and don’t add JS to the bundle. If we need interactivity like `useState` or event handlers, we mark the component with "`use client`", making it a Client Component that runs in the browser. Server Components can import both server and client components, but Client Components can only import client ones. This architecture improves performance by reducing JS shipped to the client.

    **[⬆ Back to Top](#table-of-contents)**

56. ### How to handle ISR/SSG/SSR in Next.js with Shopify?
    In a headless Shopify + Next.js setup, I decide rendering strategy based on content freshness. Static pages like homepage can use SSG for best performance. Product pages often use ISR, so they get updated automatically every few minutes when stock or prices change. For personalized or dynamic content like carts, checkout, and logged-in customer dashboards, I use SSR with cache: 'no-store'. This way, I balance performance with data accuracy.

**[⬆ Back to Top](#table-of-contents)**

57. ### How to implement Shopify checkout redirect in Next.js?
    In a headless Shopify + Next.js build, checkout is always hosted on Shopify for PCI compliance. The workflow is:
    1. Create a checkout session via Storefront API using `checkoutCreate`.
    2. Shopify returns a `webUrl`.
    3. Redirect the user to that URL with `window.location.href`.
        Optionally, I can modify the checkout with APIs like checkoutLineItemsUpdate before redirecting. This approach ensures security, leverages Shopify’s checkout extensibility, and keeps the storefront decoupled."*

    **[⬆ Back to Top](#table-of-contents)**

58. ### How do you manage global state (cart, auth) in React?
    In a React or Next.js Shopify storefront, I usually manage cart and auth globally using Context API or Zustand. For the cart, I maintain items, quantities, and totals in global state, sync it with Shopify’s Cart API, and persist it in localStorage. For authentication, I store the customerAccessToken securely (usually in HttpOnly cookies), keep it in state to control logged-in vs guest UI, and refresh it when it expires. In enterprise apps, I use Redux Toolkit because it provides better scalability and debugging via DevTools.
    **Best Practices (Interview Points)**
    - ✅ Use Context/Zustand for Shopify storefronts (lightweight, easy).
    - ✅ Use Redux Toolkit in enterprise apps with complex cart logic.
    - ✅ Persist state in localStorage or IndexedDB so cart/auth isn’t lost on refresh.
    - ✅ Sync with Shopify APIs (Cart API / Customer API).
    - ✅ Keep auth tokens in HttpOnly cookies (better security than localStorage).

    **[⬆ Back to Top](#table-of-contents)**

59. ### How to implement lazy loading product images in React?
    To implement lazy loading of product images in React, I usually rely on the native loading="lazy" attribute for simple cases. For more control, I use the Intersection Observer API to load images only when they enter the viewport and show placeholders until then. In Next.js headless builds, I prefer next/image since it comes with automatic lazy loading and optimizations. For production e-commerce sites, I also use low-res blurred placeholders to improve perceived performance.

    **[⬆ Back to Top](#table-of-contents)**

60. ### How to handle SEO in a headless Shopify setup?
    In a headless Shopify setup, SEO is not handled automatically like in Liquid themes, so we need to implement it ourselves. I make sure to fetch SEO fields (title, description, canonical URL) from Shopify and inject them into the head of the page. I also add structured data (JSON-LD) for products and collections to support Google Rich Snippets. Then I generate a dynamic sitemap and robots.txt for search engines. From a performance standpoint, I rely on Next.js features like ISR and lazy-loading images to improve Core Web Vitals. This ensures the headless store remains as SEO-friendly as a native Shopify store, while giving me full control.

    **[⬆ Back to Top](#table-of-contents)**

61. ### How to implement wishlist functionality?
    To implement wishlist functionality in Shopify, I usually start with a localStorage-based solution for guest users, where product IDs are stored in the browser. For logged-in users, I extend this by storing wishlist data in customer metafields via the Storefront/Admin API, so the wishlist is persistent across devices. In a headless setup, I’d use a custom backend (like Firebase or MongoDB) to store wishlist data tied to the customer account, and fetch product details dynamically with the Storefront API. This ensures flexibility and scalability while giving a smooth user experience.

    **[⬆ Back to Top](#table-of-contents)**

62. ### How to build a custom product builder (personalization)?
    To build a custom product builder in Shopify, I typically use line item properties when the customization doesn’t require a new SKU—for example, engraving text, uploaded images, or special notes. This ensures personalization details travel with the order. For more complex builders, like bundle products or multi-step configurations, I use AJAX API to handle product selection and pass custom properties to the cart. In headless setups, I’d store personalization data in a backend database and only send a reference ID to Shopify, which keeps checkout clean while allowing unlimited customization. I also enhance the UX with live previews, multi-step wizards, and conditional price adjustments using Shopify Functions.

    **[⬆ Back to Top](#table-of-contents)**

63. ### How to implement upsell / cross-sell sections?
    To implement upsell and cross-sell in Shopify, I use a combination of Shopify’s Product Recommendations API and custom metafields. On product and cart pages, I fetch related products via AJAX and display them dynamically, allowing one-click add-to-cart. For drawer carts, I often show cross-sell suggestions when an item is added. In Shopify Plus, I can also leverage checkout extensibility to show post-purchase upsells. This way, I cover multiple touchpoints—product page, cart, checkout, and post-purchase—maximizing AOV (average order value).

    **[⬆ Back to Top](#table-of-contents)**

64. ### How do you build a mega menu in Shopify?
    To build a mega menu in Shopify, I use the built-in Navigation menu system to create parent, child, and grandchild links. In the theme’s `header.liquid`, I loop through navigation links with Liquid and output a multi-column dropdown using grid CSS. I usually add hover interactions and support for banners or featured products. For advanced flexibility, I integrate metafields or metaobjects so that merchants can assign custom images or product blocks inside the mega menu, without editing code.

    **[⬆ Back to Top](#table-of-contents)**

65. ### How to create a multi-store setup with shared data?
    For multi-store setups, I usually evaluate whether Shopify Markets is enough, or if we need fully separate expansion stores. If we need separate stores (e.g., US/EU), I ensure data consistency by syncing products, customers, and inventory via the Admin API or a middleware service. On Shopify Plus, I’d use Multipass login for shared authentication, and webhook-driven sync for orders and stock. In a headless approach, I would fetch from a single Shopify backend via the Storefront API, while controlling region-specific catalog, currency, and tax logic in the frontend. This way, we achieve a global presence with centralized data.

    **[⬆ Back to Top](#table-of-contents)**

66. ### What are the biggest challenges you faced in Shopify development?
    Some of the biggest challenges I’ve faced include checkout customization under the new checkout extensibility model, syncing data across multi-store setups, and improving theme performance when multiple apps slowed down Core Web Vitals. I solved these by leveraging Shopify Functions, building middleware with APIs & webhooks, and optimizing themes with lazy loading and script management. Another challenge is Liquid’s limitation for dynamic logic — in those cases, I use metafields, metaobjects, or headless approaches with Hydrogen/Next.js. These experiences helped me deliver scalable and high-performing Shopify stores.

    **[⬆ Back to Top](#table-of-contents)**


## Disclaimer

Good luck with your interview 😊

---
