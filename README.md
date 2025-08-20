# Shopify Interview Questions & Answers


---

### Table of Contents

<!-- TOC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [What is Shopify?](#What-is-Shopify) |
| 2 | [What is the difference between Shopify Online Store 2.0 and older themes?](#What-is-the-difference-between-Shopify-Online-Store-2.0-and-older-themes) |
| 3 | [What are sections and blocks in Shopify?](#What-are-sections-and-blocks-in-Shopify) |
| 4 | [Explain Metafields vs Metaobjects.](#Explain-Metafields-vs-Metaobjects) |
| 5 | [How do you use dynamic sources in theme editor?](#How-do-you-use-dynamic-sources-in-theme-editor) |
| 6 | [How does Shopify handle multi-currency and multi-language stores?](#How-does-Shopify-handle-multi-currency-and-multi-language-stores) |
| 7 | [What is the difference between Shopify Themes and Shopify Apps?](#What-is-the-difference-between-Shopify-Themes-and-Shopify-Apps) |
| 8 | [How does Shopify hosting work (CDN, Liquid rendering, caching)?](#How-does-Shopify-hosting-work-(CDN,-Liquid-rendering,-caching)) |
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
| 20 | [How to use forloop.index and forloop.last in Liquid?](#How-to-use-forloop.index-and-forloop.last-in-Liquid) |





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

2. ### What is the difference between Shopify Online Store 2.0 and older themes?

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

      
      1: What is the purpose of the Liquid templating language in Shopify?

      Ans: The purpose of the Liquid templating language in Shopify is to:

      1. Render dynamic content: Liquid allows developers to display data from Shopify objects (such as products, collections, and customer information) within themes and templates.
      2. Control flow: Liquid provides control structures like loops and conditionals to create more complex logic within templates.
      3. Improve readability: Liquid uses a simple and easy-to-understand syntax, making it easier for developers to read and maintain the code.
      4. Maintain consistency: Liquid is used across all Shopify themes, ensuring a consistent development experience for developers working with various themes.
      
      Q27: How do you create a dynamic content section using Liquid?

      Ans: To create a dynamic content section using Liquid, follow these steps:

      1. Create a new section file in the sections folder of your theme, e.g., dynamic-content.liquid.
      2. Define the section settings using the schema tag:
      {% schema %} { "name": "Dynamic Content", "settings": [ { "type": "text", "id": "heading", "label": "Heading", "default": "Sample Heading" }, { "type": "richtext", "id": "content", "label": "Content", "default": "Sample content" } ] } {% endschema %}

      1. Add the Liquid code to render the content based on the section settings:
      <div class="dynamic-content-section"> <h2>{{ section.settings.heading }}</h2> <div class="dynamic-content"> {{ section.settings.content }} </div> </div>

      2. Include the section in a template file using the section tag:
      {% section 'dynamic-content' %}

      Q28: Can you explain the difference between filters and tags in Liquid?
      Ans: In Liquid:

      1. Filters are used to modify output. They take an input, apply a transformation, and return a modified output. Filters are added to Liquid objects using the pipe character |. Example: {{ product.title | upcase }} - this would output the product title in uppercase.
      2. Tags are used to create logic and control flow in templates. They are written within curly braces and percentage signs {% %}. Tags can be used for loops, conditionals, variables, and other control structures. Example: {% if product.available %}In Stock{% else %}Out of Stock{% endif %} - this would display "In Stock" if the product is available, and "Out of Stock" otherwise.
      
      Q29: What are some techniques for troubleshooting Liquid code?
      Ans: Techniques for troubleshooting Liquid code include:

      1. Reviewing the documentation: Consult the official Shopify Liquid documentation to verify the correct usage of tags, filters, and objects.
      2. Using the comment tag: Temporarily disable sections of code by wrapping them in {% comment %} and {% endcomment %} tags to isolate issues.
      3. Debugging with assign: Use the assign tag to create temporary variables to track values and debug issues within your code.
      4. Inspecting the browser console: Check for any errors or warnings in the browser console, which may indicate issues with JavaScript, CSS, or Liquid rendering.
      
      Q30: How do you optimize Liquid code for performance?
      Ans: To optimize Liquid code for performance:

      1. Minimize loops: Limit the use of for loops, especially nested loops, as they can significantly slow down page rendering.
      2. Use pagination: When displaying large collections or product lists
      3. Cache expensive operations: Use the cache tag to store the output of resource-intensive operations and reuse them later, reducing the need to perform the same operation multiple times.
      4. Optimize images: Use Liquid filters like img_url and img_tag to optimize and serve appropriately sized images to different devices.
      5. Reduce HTTP requests: Combine multiple Liquid assets (CSS or JavaScript files) into a single file using the stylesheet_tag and javascript_tag filters to reduce the number of HTTP requests.
      6. Use conditional rendering: Use the if and unless tags to conditionally render content based on specific criteria, reducing the amount of unnecessary content on the page.
      7. Minimize the use of global objects: Accessing global objects, such as all_products, can be resource-intensive. Use more specific queries to retrieve data when possible

  **[⬆ Back to Top](#table-of-contents)**




## Disclaimer

Good luck with your interview 😊

---
