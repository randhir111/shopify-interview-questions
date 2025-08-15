# shopify-interview-questions
Shopify Interview Questions and Answers
### Table of Contents

<!-- TOC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [What are the possible ways to create objects in JavaScript](#what-are-the-possible-ways-to-create-objects-in-javascript) |
| 2 | [What is a prototype chain](#what-is-a-prototype-chain) |
| 3 | [What is the Difference Between `call`, `apply`, and `bind`](#what-is-the-difference-between-call-apply-and-bind) |
| 4 | [What is JSON and its common operations](#what-is-json-and-its-common-operations) |
| 5 | [What is the purpose of the array slice method](#what-is-the-purpose-of-the-array-slice-method) |
| 6 | [What is the purpose of the array splice method](#what-is-the-purpose-of-the-array-splice-method) |
| 7 | [What is the difference between slice and splice](#what-is-the-difference-between-slice-and-splice) |
| 8 | [How do you compare Object and Map](#how-do-you-compare-object-and-map) |
| 9 | [What is the difference between == and === operators](#what-is-the-difference-between--and--operators) |
| 10 | [What are lambda expressions or arrow functions](#what-are-lambda-expressions-or-arrow-functions) |
| 11 | [What is a first class function](#what-is-a-first-class-function) |
| 12 | [What is a first order function](#what-is-a-first-order-function) |
| 13 | [What is a higher order function](#what-is-a-higher-order-function) |
| 14 | [What is a unary function](#what-is-a-unary-function) |
| 15 | [What is the currying function](#what-is-the-currying-function) |
| 16 | [What is a pure function](#what-is-a-pure-function) |
| 17 | [What are the benefits of pure functions](#what-are-the-benefits-of-pure-functions) |
| 18 | [What is the purpose of the let keyword](#what-is-the-purpose-of-the-let-keyword) |
| 19 | [What is the difference between let and var](#what-is-the-difference-between-let-and-var) |
| 20 | [What is the reason to choose the name let as a keyword](#what-is-the-reason-to-choose-the-name-let-as-a-keyword) |
| 21 | [How do you redeclare variables in a switch block without an error](#how-do-you-redeclare-variables-in-a-switch-block-without-an-error) |
| 22 | [What is the Temporal Dead Zone](#what-is-the-temporal-dead-zone) |
| 23 | [What is an IIFE (Immediately Invoked Function Expression)](#what-is-an-iife-immediately-invoked-function-expression) |
| 24 | [How do you decode or encode a URL in JavaScript?](#how-do-you-decode-or-encode-a-url-in-javascript) |
| 25 | [What is memoization](#what-is-memoization) |
| 26 | [What is Hoisting](#what-is-hoisting) |
| 27 | [What are classes in ES6](#what-are-classes-in-es6) |
| 28 | [What are closures](#what-are-closures) |
| 29 | [What are modules](#what-are-modules) |
| 30 | [Why do you need modules](#why-do-you-need-modules) |
| 31 | [What is scope in javascript](#what-is-scope-in-javascript) |
| 32 | [What is a service worker](#what-is-a-service-worker) |
| 33 | [How do you manipulate DOM using a service worker](#how-do-you-manipulate-dom-using-a-service-worker) |
| 34 | [How do you reuse information across service worker restarts](#how-do-you-reuse-information-across-service-worker-restarts) |
| 35 | [What is IndexedDB](#what-is-indexeddb) |
| 36 | [What is web storage](#what-is-web-storage) |
| 37 | [What is a post message](#what-is-a-post-message) |
| 38 | [What is a Cookie](#what-is-a-cookie) |
| 39 | [Why do you need a Cookie](#why-do-you-need-a-cookie) |
| 40 | [What are the options in a cookie](#what-are-the-options-in-a-cookie) |
| 41 | [How do you delete a cookie](#how-do-you-delete-a-cookie) |
| 42 | [What are the differences between cookie, local storage and session storage](#what-are-the-differences-between-cookie-local-storage-and-session-storage) |
| 43 | [What is the main difference between localStorage and sessionStorage](#what-is-the-main-difference-between-localstorage-and-sessionstorage) |
| 44 | [How do you access web storage](#how-do-you-access-web-storage) |
| 45 | [What are the methods available on session storage](#what-are-the-methods-available-on-session-storage) |
| 46 | [What is a storage event and its event handler](#what-is-a-storage-event-and-its-event-handler) |
| 47 | [Why do you need web storage](#why-do-you-need-web-storage) |
| 48 | [How do you check web storage browser support](#how-do-you-check-web-storage-browser-support) |
| 49 | [How do you check web workers browser support](#how-do-you-check-web-workers-browser-support) |
| 50 | [Give an example of a web worker](#give-an-example-of-a-web-worker) |
| 51 | [What are the restrictions of web workers on DOM](#what-are-the-restrictions-of-web-workers-on-dom) |
| 52 | [What is a promise](#what-is-a-promise) |
| 53 | [Why do you need a promise](#why-do-you-need-a-promise) |
| 54 | [Explain the three states of promise](#explain-the-three-states-of-promise) |
| 55 | [What is a callback function](#what-is-a-callback-function) |
| 56 | [Why do we need callbacks](#why-do-we-need-callbacks) |
| 57 | [What is a callback hell](#what-is-a-callback-hell) |
| 58 | [What are server-sent events](#what-are-server-sent-events) |
| 59 | [How do you receive server-sent event notifications](#how-do-you-receive-server-sent-event-notifications) |
| 60 | [How do you check browser support for server-sent events](#how-do-you-check-browser-support-for-server-sent-events) |
| 61 | [What are the events available for server sent events](#what-are-the-events-available-for-server-sent-events) |
| 62 | [What are the main rules of promise](#what-are-the-main-rules-of-promise) |
| 63 | [What is callback in callback](#what-is-callback-in-callback) |
| 64 | [What is promise chaining](#what-is-promise-chaining) |
| 65 | [What is promise.all](#what-is-promiseall) |
| 66 | [What is the purpose of the race method in promise](#what-is-the-purpose-of-the-race-method-in-promise) |
| 67 | [What is a strict mode in javascript](#what-is-a-strict-mode-in-javascript) |
| 68 | [Why do you need strict mode](#why-do-you-need-strict-mode) |
| 69 | [How do you declare strict mode](#how-do-you-declare-strict-mode) |
| 70 | [What is the purpose of double exclamation](#what-is-the-purpose-of-double-exclamation) |
| 71 | [What is the purpose of the delete operator](#what-is-the-purpose-of-the-delete-operator) |
| 72 | [What is typeof operator](#what-is-typeof-operator) |
| 73 | [What is undefined property](#what-is-undefined-property) |
| 74 | [What is null value](#what-is-null-value) |
| 75 | [What is the difference between null and undefined](#what-is-the-difference-between-null-and-undefined) |
| 76 | [What is eval](#what-is-eval) |
| 77 | [What is the difference between window and document](#what-is-the-difference-between-window-and-document) |
| 78 | [How do you access history in javascript](#how-do-you-access-history-in-javascript) |
| 79 | [How do you detect caps lock key turned on or not](#how-do-you-detect-caps-lock-key-turned-on-or-not) |
| 80 | [What is isNaN](#what-is-isnan) |
| 81 | [What are the differences between undeclared and undefined variables](#what-are-the-differences-between-undeclared-and-undefined-variables) |
| 82 | [What are global variables](#what-are-global-variables) |
| 83 | [What are the problems with global variables](#what-are-the-problems-with-global-variables) |
| 84 | [What is NaN property](#what-is-nan-property) |
| 85 | [What is the purpose of isFinite function](#what-is-the-purpose-of-isfinite-function) |
| 86 | [What is an event flow](#what-is-an-event-flow) |
| 87 | [What is event capturing](#what-is-event-capturing) |
| 88 | [What is event bubbling](#what-is-event-bubbling) |
| 89 | [How do you submit a form using JavaScript](#how-do-you-submit-a-form-using-javascript) |
| 90 | [How do you find operating system details](#how-do-you-find-operating-system-details) |
| 91 | [What is the difference between document load and DOMContentLoaded events](#what-is-the-difference-between-document-load-and-domcontentloaded-events) |
| 92 | [What is the difference between native, host and user objects](#what-is-the-difference-between-native-host-and-user-objects) |
| 93 | [What are the tools or techniques used for debugging JavaScript code](#what-are-the-tools-or-techniques-used-for-debugging-javascript-code) |
| 94 | [What are the pros and cons of promises over callbacks](#what-are-the-pros-and-cons-of-promises-over-callbacks) |
| 95 | [What is the difference between an attribute and a property](#what-is-the-difference-between-an-attribute-and-a-property) |
| 96 | [What is same-origin policy](#what-is-same-origin-policy) |
| 97 | [What is the purpose of void 0](#what-is-the-purpose-of-void-0) |
| 98 | [Is JavaScript a compiled or interpreted language](#is-javascript-a-compiled-or-interpreted-language) |
| 99 | [Is JavaScript a case-sensitive language](#is-javascript-a-case-sensitive-language) |
| 100 | [Is there any relation between Java and JavaScript](#is-there-any-relation-between-java-and-javascript) |
| 101 | [What are events](#what-are-events) |
| 102 | [Who created javascript](#who-created-javascript) |
| 103 | [What is the use of preventDefault method](#what-is-the-use-of-preventdefault-method) |
| 104 | [What is the use of stopPropagation method](#what-is-the-use-of-stoppropagation-method) |
| 105 | [What are the steps involved in return false usage](#what-are-the-steps-involved-in-return-false-usage) |
| 106 | [What is BOM](#what-is-bom) |
| 107 | [What is the use of setTimeout](#what-is-the-use-of-settimeout) |
| 108 | [What is the use of setInterval](#what-is-the-use-of-setinterval) |
| 109 | [Why is JavaScript treated as Single threaded](#why-is-javascript-treated-as-single-threaded) |
| 110 | [What is an event delegation](#what-is-an-event-delegation) |
| 111 | [What is ECMAScript](#what-is-ecmascript) |
| 112 | [What is JSON](#what-is-json) |
| 113 | [What are the syntax rules of JSON](#what-are-the-syntax-rules-of-json) |
| 114 | [What is the purpose JSON stringify](#what-is-the-purpose-json-stringify) |
| 115 | [How do you parse JSON string](#how-do-you-parse-json-string) |
| 116 | [Why do you need JSON](#why-do-you-need-json) |
| 117 | [What are PWAs](#what-are-pwas) |
| 118 | [What is the purpose of clearTimeout method](#what-is-the-purpose-of-cleartimeout-method) |
| 119 | [What is the purpose of clearInterval method](#what-is-the-purpose-of-clearinterval-method) |
| 120 | [How do you redirect new page in javascript](#how-do-you-redirect-new-page-in-javascript) |
| 121 | [How do you check whether a string contains a substring](#how-do-you-check-whether-a-string-contains-a-substring) |
| 122 | [How do you validate an email in javascript](#how-do-you-validate-an-email-in-javascript) |
| 123 | [How do you get the current url with javascript](#how-do-you-get-the-current-url-with-javascript) |
| 124 | [What are the various url properties of location object](#what-are-the-various-url-properties-of-location-object) |
| 125 | [How do get query string values in javascript](#how-do-get-query-string-values-in-javascript) |
| 126 | [How do you check if a key exists in an object](#how-do-you-check-if-a-key-exists-in-an-object) |
| 127 | [How do you loop through or enumerate javascript object](#how-do-you-loop-through-or-enumerate-javascript-object) |
| 128 | [How do you test for an empty object](#how-do-you-test-for-an-empty-object) |
| 129 | [What is an arguments object](#what-is-an-arguments-object) |
| 130 | [How do you make first letter of the string in an uppercase](#how-do-you-make-first-letter-of-the-string-in-an-uppercase) |
| 131 | [What are the pros and cons of for loops](#what-are-the-pros-and-cons-of-for-loops) |
| 132 | [How do you display the current date in javascript](#how-do-you-display-the-current-date-in-javascript) |
| 133 | [How do you compare two date objects](#how-do-you-compare-two-date-objects) |
| 134 | [How do you check if a string starts with another string](#how-do-you-check-if-a-string-starts-with-another-string) |
| 135 | [How do you trim a string in javascript](#how-do-you-trim-a-string-in-javascript) |
| 136 | [How do you add a key value pair in javascript](#how-do-you-add-a-key-value-pair-in-javascript) |
| 137 | [Is the !-- notation represents a special operator](#is-the----notation-represents-a-special-operator) |
| 138 | [How do you assign default values to variables](#how-do-you-assign-default-values-to-variables) |
| 139 | [How do you define multiline strings](#how-do-you-define-multiline-strings) |
| 140 | [What is an app shell model](#what-is-an-app-shell-model) |
| 141 | [Can we define properties for functions](#can-we-define-properties-for-functions) |
| 142 | [What is the way to find the number of parameters expected by a function](#what-is-the-way-to-find-the-number-of-parameters-expected-by-a-function) |
| 143 | [What is a polyfill](#what-is-a-polyfill) |
| 144 | [What are break and continue statements](#what-are-break-and-continue-statements) |
| 145 | [What are js labels](#what-are-js-labels) |
| 146 | [What are the benefits of keeping declarations at the top](#what-are-the-benefits-of-keeping-declarations-at-the-top) |
| 147 | [What are the benefits of initializing variables](#what-are-the-benefits-of-initializing-variables) |
| 148 | [What are the recommendations to create new object](#what-are-the-recommendations-to-create-new-object) |
| 149 | [How do you define JSON arrays](#how-do-you-define-json-arrays) |
| 150 | [How do you generate random integers](#how-do-you-generate-random-integers) |
| 151 | [Can you write a random integers function to print integers within a range](#can-you-write-a-random-integers-function-to-print-integers-within-a-range) |
| 152 | [What is tree shaking](#what-is-tree-shaking) |
| 153 | [What is the need of tree shaking](#what-is-the-need-of-tree-shaking) |
| 154 | [Is it recommended to use eval](#is-it-recommended-to-use-eval) |
| 155 | [What is a Regular Expression](#what-is-a-regular-expression) |
| 156 | [What are the string methods that accept Regular expression](#what-are-the-string-methods-that-accept-regular-expression) |
| 157 | [What are modifiers in regular expression](#what-are-modifiers-in-regular-expression) |
| 158 | [What are regular expression patterns](#what-are-regular-expression-patterns) |
| 159 | [What is a RegExp object](#what-is-a-regexp-object) |
| 160 | [How do you search a string for a pattern](#how-do-you-search-a-string-for-a-pattern) |
| 161 | [What is the purpose of exec method](#what-is-the-purpose-of-exec-method) |
| 162 | [How do you change the style of a HTML element](#how-do-you-change-the-style-of-a-html-element) |
| 163 | [What would be the result of 1+2+'3'](#what-would-be-the-result-of-123) |
| 164 | [What is a debugger statement](#what-is-a-debugger-statement) |
| 165 | [What is the purpose of breakpoints in debugging](#what-is-the-purpose-of-breakpoints-in-debugging) |
| 166 | [Can I use reserved words as identifiers](#can-i-use-reserved-words-as-identifiers) |
| 167 | [How do you detect a mobile browser](#how-do-you-detect-a-mobile-browser) |
| 168 | [How do you detect a mobile browser without regexp](#how-do-you-detect-a-mobile-browser-without-regexp) |
| 169 | [How do you get the image width and height using JS](#how-do-you-get-the-image-width-and-height-using-js) |
| 170 | [How do you make synchronous HTTP request](#how-do-you-make-synchronous-http-request) |
| 171 | [How do you make asynchronous HTTP request](#how-do-you-make-asynchronous-http-request) |
| 172 | [How do you convert date to another timezone in javascript](#how-do-you-convert-date-to-another-timezone-in-javascript) |
| 173 | [What are the properties used to get size of window](#what-are-the-properties-used-to-get-size-of-window) |
| 174 | [What is a conditional operator in javascript](#what-is-a-conditional-operator-in-javascript) |
| 175 | [Can you apply chaining on conditional operator](#can-you-apply-chaining-on-conditional-operator) |
| 176 | [What are the ways to execute javascript after a page load](#what-are-the-ways-to-execute-javascript-after-a-page-load) |
| 177 | [What is the difference between proto and prototype](#what-is-the-difference-between-proto-and-prototype) |
| 178 | [Can you give an example of when you really need a semicolon](#can-you-give-an-example-of-when-you-really-need-a-semicolon) |
| 179 | [What is the freeze method](#what-is-the-freeze-method) |
| 180 | [What is the purpose of the freeze method](#what-is-the-purpose-of-the-freeze-method) |
| 181 | [Why do I need to use the freeze method](#why-do-i-need-to-use-the-freeze-method) |
| 182 | [How do you detect a browser language preference](#how-do-you-detect-a-browser-language-preference) |
| 183 | [How to convert a string to title case with javascript](#how-to-convert-a-string-to-title-case-with-javascript) |
| 184 | [How do you detect if javascript is disabled on the page](#how-do-you-detect-if-javascript-is-disabled-on-the-page) |
| 185 | [What are various operators supported by javascript](#what-are-various-operators-supported-by-javascript) |
| 186 | [What is a rest parameter](#what-is-a-rest-parameter) |
| 187 | [What happens if you do not use rest parameter as a last argument](#what-happens-if-you-do-not-use-rest-parameter-as-a-last-argument) |
| 188 | [What are the bitwise operators available in javascript](#what-are-the-bitwise-operators-available-in-javascript) |
| 189 | [What is a spread operator](#what-is-a-spread-operator) |
| 190 | [How do you determine whether object is frozen or not](#how-do-you-determine-whether-object-is-frozen-or-not) |
| 191 | [How do you determine two values same or not using object](#how-do-you-determine-two-values-same-or-not-using-object) |
| 192 | [What is the purpose of using object is method](#what-is-the-purpose-of-using-object-is-method) |
| 193 | [How do you copy properties from one object to other](#how-do-you-copy-properties-from-one-object-to-other) |
| 194 | [What are the applications of the assign method](#what-are-the-applications-of-the-assign-method) |
| 195 | [What is a proxy object](#what-is-a-proxy-object) |
| 196 | [What is the purpose of the seal method](#what-is-the-purpose-of-the-seal-method) |
| 197 | [What are the applications of the seal method](#what-are-the-applications-of-the-seal-method) |
| 198 | [What are the differences between the freeze and seal methods](#what-are-the-differences-between-the-freeze-and-seal-methods) |
| 199 | [How do you determine if an object is sealed or not](#how-do-you-determine-if-an-object-is-sealed-or-not) |
| 200 | [How do you get enumerable key and value pairs](#how-do-you-get-enumerable-key-and-value-pairs) |
| 201 | [What is the main difference between Object.values and Object.entries method](#what-is-the-main-difference-between-objectvalues-and-objectentries-method) |
| 202 | [How can you get the list of keys of any object](#how-can-you-get-the-list-of-keys-of-any-object) |
| 203 | [How do you create an object with a prototype](#how-do-you-create-an-object-with-a-prototype) |
| 204 | [What is a WeakSet](#what-is-a-weakset) |
| 205 | [What are the differences between WeakSet and Set](#what-are-the-differences-between-weakset-and-set) |
| 206 | [List down the collection of methods available on WeakSet](#list-down-the-collection-of-methods-available-on-weakset) |
| 207 | [What is a WeakMap](#what-is-a-weakmap) |
| 208 | [What are the differences between WeakMap and Map](#what-are-the-differences-between-weakmap-and-map) |
| 209 | [List down the collection of methods available on WeakMap](#list-down-the-collection-of-methods-available-on-weakmap) |
| 210 | [What is the purpose of uneval](#what-is-the-purpose-of-uneval) |
| 211 | [How do you encode an URL](#how-do-you-encode-an-url) |
| 212 | [How do you decode an URL](#how-do-you-decode-an-url) |
| 213 | [How do you print the contents of web page](#how-do-you-print-the-contents-of-web-page) |
| 214 | [What is the difference between uneval and eval](#what-is-the-difference-between-uneval-and-eval) |
| 215 | [What is an anonymous function](#what-is-an-anonymous-function) |
| 216 | [What is the precedence order between local and global variables](#what-is-the-precedence-order-between-local-and-global-variables) |
| 217 | [What are javascript accessors](#what-are-javascript-accessors) |
| 218 | [How do you define property on Object constructor](#how-do-you-define-property-on-object-constructor) |
| 219 | [What is the difference between get and defineProperty](#what-is-the-difference-between-get-and-defineproperty) |
| 220 | [What are the advantages of Getters and Setters](#what-are-the-advantages-of-getters-and-setters) |
| 221 | [Can I add getters and setters using defineProperty method](#can-i-add-getters-and-setters-using-defineproperty-method) |
| 222 | [What is the purpose of switch-case](#what-is-the-purpose-of-switch-case) |
| 223 | [What are the conventions to be followed for the usage of switch case](#what-are-the-conventions-to-be-followed-for-the-usage-of-switch-case) |
| 224 | [What are primitive data types](#what-are-primitive-data-types) |
| 225 | [What are the different ways to access object properties](#what-are-the-different-ways-to-access-object-properties) |
| 226 | [What are the function parameter rules](#what-are-the-function-parameter-rules) |
| 227 | [What is an error object](#what-is-an-error-object) |
| 228 | [When do you get a syntax error](#when-do-you-get-a-syntax-error) |
| 229 | [What are the different error names from error object](#what-are-the-different-error-names-from-error-object) |
| 230 | [What are the various statements in error handling](#what-are-the-various-statements-in-error-handling) |
| 231 | [What are the two types of loops in javascript](#what-are-the-two-types-of-loops-in-javascript) |
| 232 | [What is nodejs](#what-is-nodejs) |
| 233 | [What is the Intl object](#what-is-the-intl-object) |
| 234 | [How do you perform language specific date and time formatting](#how-do-you-perform-language-specific-date-and-time-formatting) |
| 235 | [What is an Iterator](#what-is-an-iterator) |
| 236 | [How does synchronous iteration works](#how-does-synchronous-iteration-works) |
| 237 | [What is the event loop](#what-is-the-event-loop) |
| 238 | [What is the call stack](#what-is-the-call-stack) |
| 239 | [What is the event queue](#what-is-the-event-queue) |
| 240 | [What is a decorator](#what-is-a-decorator) |
| 241 | [What are the properties of the Intl object](#what-are-the-properties-of-the-intl-object) |
| 242 | [What is an Unary operator](#what-is-an-unary-operator) |
| 243 | [How do you sort elements in an array](#how-do-you-sort-elements-in-an-array) |
| 244 | [What is the purpose of compareFunction while sorting arrays](#what-is-the-purpose-of-comparefunction-while-sorting-arrays) |
| 245 | [How do you reverse an array](#how-do-you-reverse-an-array) |
| 246 | [How do you find the min and max values in an array](#how-do-you-find-the-min-and-max-values-in-an-array) |
| 247 | [How do you find the min and max values without Math functions](#how-do-you-find-the-min-and-max-values-without-math-functions) |
| 248 | [What is an empty statement and purpose of it](#what-is-an-empty-statement-and-purpose-of-it) |
| 249 | [How do you get the metadata of a module](#how-do-you-get-the-metadata-of-a-module) |
| 250 | [What is the comma operator](#what-is-the-comma-operator) |
| 251 | [What is the advantage of the comma operator](#what-is-the-advantage-of-the-comma-operator) |
| 252 | [What is typescript](#what-is-typescript) |
| 253 | [What are the differences between javascript and typescript](#what-are-the-differences-between-javascript-and-typescript) |
| 254 | [What are the advantages of typescript over javascript](#what-are-the-advantages-of-typescript-over-javascript) |
| 255 | [What is an object initializer](#what-is-an-object-initializer) |
| 256 | [What is a constructor method](#what-is-a-constructor-method) |
| 257 | [What happens if you write constructor more than once in a class](#what-happens-if-you-write-constructor-more-than-once-in-a-class) |
| 258 | [How do you call the constructor of a parent class](#how-do-you-call-the-constructor-of-a-parent-class) |
| 259 | [How do you get the prototype of an object](#how-do-you-get-the-prototype-of-an-object) |
| 260 | [What happens If I pass string type for getPrototype method](#what-happens-if-i-pass-string-type-for-getprototype-method) |
| 261 | [How do you set the prototype of one object to another](#how-do-you-set-the-prototype-of-one-object-to-another) |
| 262 | [How do you check whether an object can be extended or not](#how-do-you-check-whether-an-object-can-be-extended-or-not) |
| 263 | [How do you prevent an object from being extend](#how-do-you-prevent-an-object-from-being-extend) |
| 264 | [What are the different ways to make an object non-extensible](#what-are-the-different-ways-to-make-an-object-non-extensible) |
| 265 | [How do you define multiple properties on an object](#how-do-you-define-multiple-properties-on-an-object) |
| 266 | [What is the MEAN stack](#what-is-the-mean-stack) |
| 267 | [What is obfuscation in javascript](#what-is-obfuscation-in-javascript) |
| 268 | [Why do you need Obfuscation](#why-do-you-need-obfuscation) |
| 269 | [What is Minification](#what-is-minification) |
| 270 | [What are the advantages of minification](#what-are-the-advantages-of-minification) |
| 271 | [What are the differences between obfuscation and Encryption](#what-are-the-differences-between-obfuscation-and-encryption) |
| 272 | [What are the common tools used for minification](#what-are-the-common-tools-used-for-minification) |
| 273 | [How do you perform form validation using javascript](#how-do-you-perform-form-validation-using-javascript) |
| 274 | [How do you perform form validation without javascript](#how-do-you-perform-form-validation-without-javascript) |
| 275 | [What are the DOM methods available for constraint validation](#what-are-the-dom-methods-available-for-constraint-validation) |
| 276 | [What are the available constraint validation DOM properties](#what-are-the-available-constraint-validation-dom-properties) |
| 277 | [What are the validity properties](#what-are-the-validity-properties) |
| 278 | [Give an example usage of the rangeOverflow property](#give-an-example-usage-of-the-rangeoverflow-property) |
| 279 | [Are enums available in javascript](#are-enums-available-in-javascript) |
| 280 | [What is an enum](#what-is-an-enum) |
| 281 | [How do you list all properties of an object](#how-do-you-list-all-properties-of-an-object) |
| 282 | [How do you get property descriptors of an object](#how-do-you-get-property-descriptors-of-an-object) |
| 283 | [What are the attributes provided by a property descriptor](#what-are-the-attributes-provided-by-a-property-descriptor) |
| 284 | [How do you extend classes](#how-do-you-extend-classes) |
| 285 | [How do I modify the url without reloading the page](#how-do-i-modify-the-url-without-reloading-the-page) |
| 286 | [How do you check whether or not an array includes a particular value](#how-do-you-check-whether-or-not-an-array-includes-a-particular-value) |
| 287 | [How do you compare scalar arrays](#how-do-you-compare-scalar-arrays) |
| 288 | [How to get the value from get parameters](#how-to-get-the-value-from-get-parameters) |
| 289 | [How do you print numbers with commas as thousand separators](#how-do-you-print-numbers-with-commas-as-thousand-separators) |
| 290 | [What is the difference between java and javascript](#what-is-the-difference-between-java-and-javascript) |
| 291 | [Does JavaScript support namespaces](#does-javascript-support-namespaces) |
| 292 | [How do you declare a namespace](#how-do-you-declare-a-namespace) |
| 293 | [How do you invoke javascript code in an iframe from the parent page](#how-do-you-invoke-javascript-code-in-an-iframe-from-the-parent-page) |
| 294 | [How do you get the timezone offset of a date object](#how-do-you-get-the-timezone-offset-of-a-date-object) |
| 295 | [How do you load CSS and JS files dynamically](#how-do-you-load-css-and-js-files-dynamically) |
| 296 | [What are the different methods to find HTML elements in DOM](#what-are-the-different-methods-to-find-html-elements-in-dom) |
| 297 | [What is jQuery](#what-is-jquery) |
| 298 | [What is V8 JavaScript engine](#what-is-v8-javascript-engine) |
| 299 | [Why do we call javascript as dynamic language](#why-do-we-call-javascript-as-dynamic-language) |
| 300 | [What is a void operator](#what-is-a-void-operator) |
| 301 | [How to set the cursor to wait](#how-to-set-the-cursor-to-wait) |
| 302 | [How do you create an infinite loop](#how-do-you-create-an-infinite-loop) |
| 303 | [Why do you need to avoid with statement](#why-do-you-need-to-avoid-with-statement) |
| 304 | [What is the output of the following for loops](#what-is-the-output-of-the-following-for-loops) |
| 305 | [List down some of the features of ES6](#list-down-some-of-the-features-of-es6) |
| 306 | [What is ES6](#what-is-es6) |
| 307 | [Can I redeclare let and const variables](#can-i-redeclare-let-and-const-variables) |
| 308 | [Does the `const` variable make the value immutable](#does-the-const-variable-make-the-value-immutable) |
| 309 | [What are default parameters](#what-are-default-parameters) |
| 310 | [What are template literals](#what-are-template-literals) |
| 311 | [How do you write multi-line strings in template literals](#how-do-you-write-multi-line-strings-in-template-literals) |
| 312 | [What are nesting templates](#what-are-nesting-templates) |
| 313 | [What are tagged templates](#what-are-tagged-templates) |
| 314 | [What are raw strings](#what-are-raw-strings) |
| 315 | [What is destructuring assignment](#what-is-destructuring-assignment) |
| 316 | [What are default values in destructuring assignment](#what-are-default-values-in-destructuring-assignment) |
| 317 | [How do you swap variables in destructuring assignment](#how-do-you-swap-variables-in-destructuring-assignment) |
| 318 | [What are enhanced object literals](#what-are-enhanced-object-literals) |
| 319 | [What are dynamic imports](#what-are-dynamic-imports) |
| 320 | [What are the use cases for dynamic imports](#what-are-the-use-cases-for-dynamic-imports) |
| 321 | [What are typed arrays](#what-are-typed-arrays) |
| 322 | [What are the advantages of module loaders](#what-are-the-advantages-of-module-loaders) |
| 323 | [What is collation](#what-is-collation) |
| 324 | [What is for...of statement](#what-is-forof-statement) |
| 325 | [What is the output of below spread operator array](#what-is-the-output-of-below-spread-operator-array) |
| 326 | [Is PostMessage secure](#is-postmessage-secure) |
| 327 | [What are the problems with postmessage target origin as wildcard](#what-are-the-problems-with-postmessage-target-origin-as-wildcard) |
| 328 | [How do you avoid receiving postMessages from attackers](#how-do-you-avoid-receiving-postmessages-from-attackers) |
| 329 | [Can I avoid using postMessages completely](#can-i-avoid-using-postmessages-completely) |
| 330 | [Is postMessages synchronous](#is-postmessages-synchronous) |
| 331 | [What paradigm is Javascript](#what-paradigm-is-javascript) |
| 332 | [What is the difference between internal and external javascript](#what-is-the-difference-between-internal-and-external-javascript) |
| 333 | [Is JavaScript faster than server side script](#is-javascript-faster-than-server-side-script) |
| 334 | [How do you get the status of a checkbox](#how-do-you-get-the-status-of-a-checkbox) |
| 335 | [What is the purpose of double tilde operator](#what-is-the-purpose-of-double-tilde-operator) |
| 336 | [How do you convert character to ASCII code](#how-do-you-convert-character-to-ascii-code) |
| 337 | [What is ArrayBuffer](#what-is-arraybuffer) |
| 338 | [What is the output of below string expression](#what-is-the-output-of-below-string-expression) |
| 339 | [What is the purpose of Error object](#what-is-the-purpose-of-error-object) |
| 340 | [What is the purpose of EvalError object](#what-is-the-purpose-of-evalerror-object) |
| 341 | [What are the list of cases error thrown from non-strict mode to strict mode](#what-are-the-list-of-cases-error-thrown-from-non-strict-mode-to-strict-mode) |
| 342 | [Do all objects have prototypes](#do-all-objects-have-prototypes) |
| 343 | [What is the difference between a parameter and an argument](#what-is-the-difference-between-a-parameter-and-an-argument) |
| 344 | [What is the purpose of some method in arrays](#what-is-the-purpose-of-some-method-in-arrays) |
| 345 | [How do you combine two or more arrays](#how-do-you-combine-two-or-more-arrays) |
| 346 | [What is the difference between Shallow and Deep copy](#what-is-the-difference-between-shallow-and-deep-copy) |
| 347 | [How do you create specific number of copies of a string](#how-do-you-create-specific-number-of-copies-of-a-string) |
| 348 | [How do you return all matching strings against a regular expression](#how-do-you-return-all-matching-strings-against-a-regular-expression) |
| 349 | [How do you trim a string at the beginning or ending](#how-do-you-trim-a-string-at-the-beginning-or-ending) |
| 350 | [What is the output of below console statement with unary operator](#what-is-the-output-of-below-console-statement-with-unary-operator) |
| 351 | [Does javascript uses mixins](#does-javascript-uses-mixins) |
| 352 | [Mixin Example using Object composition](#mixin-example-using-object-composition) |
| 353 | [Benefits](#benefits) |
| 354 | [What is a thunk function](#what-is-a-thunk-function) |
| 355 | [What are asynchronous thunks](#what-are-asynchronous-thunks) |
| 356 | [What is the output of below function calls](#what-is-the-output-of-below-function-calls) |
| 357 | [How to remove all line breaks from a string](#how-to-remove-all-line-breaks-from-a-string) |
| 358 | [What is the difference between reflow and repaint](#what-is-the-difference-between-reflow-and-repaint) |
| 359 | [What happens with negating an array](#what-happens-with-negating-an-array) |
| 360 | [What happens if we add two arrays](#what-happens-if-we-add-two-arrays) |
| 361 | [What is the output of prepend additive operator on falsy values](#what-is-the-output-of-prepend-additive-operator-on-falsy-values) |
| 362 | [How do you create self string using special characters](#how-do-you-create-self-string-using-special-characters) |
| 363 | [How do you remove falsy values from an array](#how-do-you-remove-falsy-values-from-an-array) |
| 364 | [How do you get unique values of an array](#how-do-you-get-unique-values-of-an-array) |
| 365 | [What is destructuring aliases](#what-is-destructuring-aliases) |
| 366 | [How do you map the array values without using map method](#how-do-you-map-the-array-values-without-using-map-method) |
| 367 | [How do you empty an array](#how-do-you-empty-an-array) |
| 368 | [How do you round numbers to certain decimals](#how-do-you-round-numbers-to-certain-decimals) |
| 369 | [What is the easiest way to convert an array to an object](#what-is-the-easiest-way-to-convert-an-array-to-an-object) |
| 370 | [How do you create an array with some data](#how-do-you-create-an-array-with-some-data) |
| 371 | [What are the placeholders from console object](#what-are-the-placeholders-from-console-object) |
| 372 | [Is it possible to add CSS to console messages](#is-it-possible-to-add-css-to-console-messages) |
| 373 | [What is the purpose of dir method of console object](#what-is-the-purpose-of-dir-method-of-console-object) |
| 374 | [Is it possible to debug HTML elements in console](#is-it-possible-to-debug-html-elements-in-console) |
| 375 | [How do you display data in a tabular format using console object](#how-do-you-display-data-in-a-tabular-format-using-console-object) |
| 376 | [How do you verify that an argument is a Number or not](#how-do-you-verify-that-an-argument-is-a-number-or-not) |
| 377 | [How do you create copy to clipboard button](#how-do-you-create-copy-to-clipboard-button) |
| 378 | [What is the shortcut to get timestamp](#what-is-the-shortcut-to-get-timestamp) |
| 379 | [How do you flattening multi dimensional arrays](#how-do-you-flattening-multi-dimensional-arrays) |
| 380 | [What is the easiest multi condition checking](#what-is-the-easiest-multi-condition-checking) |
| 381 | [How do you capture browser back button](#how-do-you-capture-browser-back-button) |
| 382 | [How do you disable right click in the web page](#how-do-you-disable-right-click-in-the-web-page) |
| 383 | [What are wrapper objects](#what-are-wrapper-objects) |
| 384 | [What is AJAX](#what-is-ajax) |
| 385 | [What are the different ways to deal with Asynchronous Code](#what-are-the-different-ways-to-deal-with-asynchronous-code) |
| 386 | [How to cancel a fetch request](#how-to-cancel-a-fetch-request) |
| 387 | [What is web speech API](#what-is-web-speech-api) |
| 388 | [What is minimum timeout throttling](#what-is-minimum-timeout-throttling) |
| 389 | [How do you implement zero timeout in modern browsers](#how-do-you-implement-zero-timeout-in-modern-browsers) |
| 390 | [What are tasks in event loop](#what-are-tasks-in-event-loop) |
| 391 | [What is microtask](#what-is-microtask) |
| 392 | [What are different event loops](#what-are-different-event-loops) |
| 393 | [What is the purpose of queueMicrotask](#what-is-the-purpose-of-queuemicrotask) |
| 394 | [How do you use javascript libraries in typescript file](#how-do-you-use-javascript-libraries-in-typescript-file) |
| 395 | [What are the differences between promises and observables](#what-are-the-differences-between-promises-and-observables) |
| 396 | [What is heap](#what-is-heap) |
| 397 | [What is an event table](#what-is-an-event-table) |
| 398 | [What is a microTask queue](#what-is-a-microtask-queue) |
| 399 | [What is the difference between shim and polyfill](#what-is-the-difference-between-shim-and-polyfill) |
| 400 | [How do you detect primitive or non primitive value type](#how-do-you-detect-primitive-or-non-primitive-value-type) |
| 401 | [What is babel](#what-is-babel) |
| 402 | [Is Node.js completely single threaded](#is-nodejs-completely-single-threaded) |
| 403 | [What are the common use cases of observables](#what-are-the-common-use-cases-of-observables) |
| 404 | [What is RxJS](#what-is-rxjs) |
| 405 | [What is the difference between Function constructor and function declaration](#what-is-the-difference-between-function-constructor-and-function-declaration) |
| 406 | [What is a Short circuit condition](#what-is-a-short-circuit-condition) |
| 407 | [What is the easiest way to resize an array](#what-is-the-easiest-way-to-resize-an-array) |
| 408 | [What is an observable](#what-is-an-observable) |
| 409 | [What is the difference between function and class declarations](#what-is-the-difference-between-function-and-class-declarations) |
| 410 | [What is an async function](#what-is-an-async-function) |
| 411 | [How do you prevent promises swallowing errors](#how-do-you-prevent-promises-swallowing-errors) |
| 412 | [What is deno](#what-is-deno) |
| 413 | [How do you make an object iterable in javascript](#how-do-you-make-an-object-iterable-in-javascript) |
| 414 | [What is a Proper Tail Call](#what-is-a-proper-tail-call) |
| 415 | [How do you check an object is a promise or not](#how-do-you-check-an-object-is-a-promise-or-not) |
| 416 | [How to detect if a function is called as constructor](#how-to-detect-if-a-function-is-called-as-constructor) |
| 417 | [What are the differences between arguments object and rest parameter](#what-are-the-differences-between-arguments-object-and-rest-parameter) |
| 418 | [What are the differences between spread operator and rest parameter](#what-are-the-differences-between-spread-operator-and-rest-parameter) |
| 419 | [What are the different kinds of generators](#what-are-the-different-kinds-of-generators) |
| 420 | [What are the built-in iterables](#what-are-the-built-in-iterables) |
| 421 | [What are the differences between for...of and for...in statements](#what-are-the-differences-between-forof-and-forin-statements) |
| 422 | [How do you define instance and non-instance properties](#how-do-you-define-instance-and-non-instance-properties) |
| 423 | [What is the difference between isNaN and Number.isNaN?](#what-is-the-difference-between-isnan-and-numberisnan) |
| 424 | [How to invoke an IIFE without any extra brackets?](#how-to-invoke-an-iife-without-any-extra-brackets) |
| 425 | [Is that possible to use expressions in switch cases?](#is-that-possible-to-use-expressions-in-switch-cases) |
| 426 | [What is the easiest way to ignore promise errors?](#what-is-the-easiest-way-to-ignore-promise-errors) |
| 427 | [How do style the console output using CSS?](#how-do-style-the-console-output-using-css) |
| 428 | [What is nullish coalescing operator (??)?](#what-is-nullish-coalescing-operator-) |
| 429 | [How do you group and nest console output?](#how-do-you-group-and-nest-console-output) |
| 430 | [What is the difference between dense and sparse arrays?](#what-is-the-difference-between-dense-and-sparse-arrays) |
| 431 | [What are the different ways to create sparse arrays?](#what-are-the-different-ways-to-create-sparse-arrays) |
| 432 | [What is the difference between setTimeout, setImmediate and process.nextTick?](#what-is-the-difference-between-settimeout-setimmediate-and-processnexttick) |
| 433 | [How do you reverse an array without modifying original array?](#how-do-you-reverse-an-array-without-modifying-original-array) |
| 434 | [How do you create custom HTML element?](#how-do-you-create-custom-html-element) |
| 435 | [What is global execution context?](#what-is-global-execution-context) |
| 436 | [What is function execution context?](#what-is-function-execution-context) |
| 437 | [What is debouncing?](#what-is-debouncing) |
| 438 | [What is throttling?](#what-is-throttling) |
| 439 | [What is optional chaining?](#what-is-optional-chaining) |
| 440 | [What is an environment record?](#what-is-an-environment-record) |
| 441 | [How to verify if a variable is an array?](#how-to-verify-if-a-variable-is-an-array) |
| 442 | [What is pass by value and pass by reference?](#what-is-pass-by-value-and-pass-by-reference) |
| 443 | [What are the differences between primitives and non-primitives?](#what-are-the-differences-between-primitives-and-non-primitives) |
| 444 | [How do you create your own bind method using either call or apply method?](#how-do-you-create-your-own-bind-method-using-either-call-or-apply-method) |
| 445 | [What are the differences between pure and impure functions?](#what-are-the-differences-between-pure-and-impure-functions) |
| 446 | [What is referential transparency?](#what-is-referential-transparency) |
| 447 | [What are the possible side-effects in javascript?](#what-are-the-possible-side-effects-in-javascript) |
| 448 | [What are compose and pipe functions?](#what-are-compose-and-pipe-functions) |
| 449 | [What is module pattern?](#what-is-module-pattern) |
| 450 | [What is Function Composition?](#what-is-function-composition) |
| 451 | [How to use await outside of async function prior to ES2022?](#how-to-use-await-outside-of-async-function-prior-to-es2022) |
| 452 | [What is the purpose of the this keyword in JavaScript?](#what-is-the-purpose-of-the-this-keyword-in-javascript) |
| 453 | [What are the uses of closures?](#what-are-the-uses-of-closures) |
| 454 | [What are the phases of execution context?](#what-are-the-phases-of-execution-context) |
| 455 | [What are the possible reasons for memory leaks?](#what-are-the-possible-reasons-for-memory-leaks) |
| 456 | [What are the optimization techniques of V8 engine?](#what-are-the-optimization-techniques-of-v8-engine) |
| 457 | [What are the examples of built-in higher order functions?](#what-are-the-examples-of-built-in-higher-order-functions) |
| 458 | [What are the benefits higher order functions?](#what-are-the-benefits-higher-order-functions) |
| 459 | [How do you create polyfills for map, filter and reduce methods?](#how-do-you-create-polyfills-for-map-filter-and-reduce-methods) |
| 460 | [What is the difference between map and forEach functions?](#what-is-the-difference-between-map-and-foreach-functions) |
| 461 | [Give an example of statements affected by automatic semicolon insertion?](#give-an-example-of-statements-affected-by-automatic-semicolon-insertion) |
| 462 | [What are the event phases of a browser?](#what-are-the-event-phases-of-a-browser) |
| 463 | [What are the real world use cases of proxy?](#what-are-the-real-world-use-cases-of-proxy) |
| 464 | [What are hidden classes?](#what-are-hidden-classes) |
| 465 | [What is inline caching?](#what-is-inline-caching) |
| 466 | [What are the different ways to execute external scripts?](#what-are-the-different-ways-to-execute-external-scripts) |
| 467 | [What is Lexical Scope?](#what-is-lexical-scope) |
| 468 | [How to detect system dark mode in javascript?](#how-to-detect-system-dark-mode-in-javascript) |
| 469 | [What is the purpose of requestAnimationFrame method?](#what-is-the-purpose-of-requestanimationframe-method) |
| 470 | [What is the difference between substring and substr methods?](#what-is-the-difference-between-substring-and-substr-methods) |
| 471 | [How to find the number of parameters expected by a function?](#how-to-find-the-number-of-parameters-expected-by-a-function) |
| 472 | [What is globalThis, and what is the importance of it?](#what-is-globalthis-and-what-is-the-importance-of-it) |
| 473 | [What are the array mutation methods?](#what-are-the-array-mutation-methods) |
| 474 | [What is module scope in JavaScript?](#what-is-module-scope-in-javascript) |
| 475 | [What are shadowing and illegal shadowing?](#what-are-shadowing-and-illegal-shadowing) |
| 476 | [Why is it important to remove event listeners after use?](#why-is-it-important-to-remove-event-listeners-after-use) |
<!-- TOC_END -->

<!-- QUESTIONS_START -->

1. ### What are the possible ways to create objects in JavaScript

    There are many ways to create objects in javascript as mentioned below:

    1. **Object literal syntax:**

       The object literal syntax (or object initializer), is a comma-separated set of name-value pairs wrapped in curly braces.

       ```javascript
       var object = {
         name: "Sudheer",
         age: 34,
       };
       ```

       Object literal property values can be of any data type, including array, function, and nested object.

       **Note:** This is one of the easiest ways to create an object and it's most commonly used for creating simple, ad-hoc objects.

    2. **Object constructor:**

       The simplest way to create an empty object is using the `Object` constructor. Currently this approach is not recommended.

       ```javascript
       var object = new Object();
       ```

       The `Object()` is a built-in constructor function so "new" keyword is not required for creating plain objects. The above code snippet can be re-written as:

       ```javascript
       var object = Object();
       ```
       However, `Object()` can be used to either create a plain object or convert a given value into its corresponding object wrapper, whereas `new Object()` is specifically used to explicitly create a new object instance.
       
    3. **Object's create method:**

       The `create` method of Object is used to create a new object by passing the specified prototype object and properties as arguments, i.e., this pattern is helpful to create new objects based on existing objects. In other words, this is useful for setting up **prototypal inheritance**. The second argument is optional and it is used to create properties on a newly created object.

       The following code creates a new empty object whose prototype is null.

       ```javascript
       var object = Object.create(null);
       ```

       The following example creates an object along with additional new properties.

       ```javascript
       let vehicle = {
         wheels: "4",
         fuelType: "Gasoline",
         color: "Green",
       };
       let carProps = {
         type: {
           value: "Volkswagen",
         },
         model: {
           value: "Golf",
         },
       };

       var car = Object.create(vehicle, carProps);
       console.log(car);
       ```

    4. **Function constructor:**

       In this approach, create any function and apply the new operator to create object instances. This was the main way to do constructor-based OOP before ES6 classes.

       ```javascript
       function Person(name) {
         this.name = name;
         this.age = 21;
       }
       var object = new Person("Sudheer");
       ```
    5. **Function constructor with prototype:**

       This is similar to function constructor but it uses prototype for their properties and methods. Using prototype means you're sharing methods/properties across instances, which saves memory and improve performance.

       ```javascript
       function Person() {}
       Person.prototype.name = "Sudheer";
       var object = new Person();
       ```

       This is equivalent to creating an instance with `Object.create` method with a function prototype and then calling that function with an instance and parameters as arguments.

       ```javascript
       function func(x, y, z) {
        this.x = x;
        this.y = y;
        this.z = z;
       }

       var instance = new func(1, 2, 3);
       ```

       **(OR)**

       ```javascript
       function func(x, y, z) {
          this.x = x;
          this.y = y;
          this.z = z;
       }
       // Create a new instance using function prototype.
       var newInstance = Object.create(func.prototype)

       // Call the function
       var result = func.call(newInstance, 1, 2, 3),

       // If the result is a non-null object then use it otherwise just use the new instance.
       console.log(result && typeof result === 'object' ? result : newInstance);
       ```

    6. **Object's assign method:**

       The `Object.assign` method is used to copy all the properties from one or more source objects and stores them into a target object. This is mainly used for cloning and merging

       The following code creates a new staff object by copying properties of his working company and the car he owns.

       ```javascript
       const orgObject = { company: "XYZ Corp" };
       const carObject = { name: "Toyota" };
       const staff = Object.assign({}, orgObject, carObject);
       ```

    7. **ES6 Class syntax:**

       ES6 introduces class feature to create objects. This is syntactic sugar over the prototype-based system.

       ```javascript
       class Person {
         constructor(name) {
           this.name = name;
         }
       }

       var object = new Person("Sudheer");
       ```

    8. **Singleton pattern:**

       A Singleton is an object which can only be instantiated one time. Repeated calls to its constructor return the same instance. This way one can ensure that they don't accidentally create multiple instances.

        ##### Singleton with Closure (Classic JS Pattern)
        ```javascript
        const Singleton = (function () {
        let instance;

        function createInstance() {
          return { name: "Sudheer" };
        }

        return {
          getInstance: function () {
            if (!instance) {
              instance = createInstance();
            }
            return instance;
          }
        };
        })();

        // Usage
        const obj1 = Singleton.getInstance();
        const obj2 = Singleton.getInstance();

        console.log(obj1 === obj2); // true
        ```
         In modern JavaScript applications, singletons are commonly implemented using ES6 modules for their built-in caching behavior, or closures for encapsulated state management.

      **[⬆ Back to Top](#table-of-contents)**

2. ### What is a prototype chain

    The prototype chain is a core concept in JavaScript’s inheritance model. It allows objects to inherit properties and methods from other objects. When you try to access a property or method on an object, JavaScript first looks for it on that object itself. If it’s not found, the engine looks up the object's internal `[[Prototype]]` reference (accessible via `Object.getPrototypeOf(obj)` or the deprecated `__proto__` property) and continues searching up the chain until it finds the property or reaches the end (usually `null`).

    For objects created via constructor functions, the prototype chain starts with the instance, then refers to the constructor’s `.prototype` object, and continues from there. For example:

    ```javascript
    function Person() {}
    const person1 = new Person();

    console.log(Object.getPrototypeOf(person1) === Person.prototype); // true
    ```

    This mechanism allows for property and method sharing among objects, enabling code reuse and a form of inheritance.

    **Summary:**

    *   The prototype chain enables inheritance in JavaScript.
    *   If a property isn’t found on an object, JavaScript looks up its prototype chain.
    *   The prototype of an object instance can be accessed with `Object.getPrototypeOf(obj)` or `__proto__`.
    *   The prototype of a constructor function is available via `Constructor.prototype`.
    *   The chain ends when the prototype is `null`.

    The prototype chain among objects appears as below, 
    
    ![Screenshot](images/prototype_chain.png)

    **[⬆ Back to Top](#table-of-contents)**

3. ### What is the Difference Between `call`, `apply`, and `bind`

  In JavaScript, `call`, `apply`, and `bind` are methods that allow you to control the context (`this` value) in which a function is executed. While their purposes are similar, they differ in how they handle arguments and when the function is invoked.

  ---

  #### `call`

  - **Description:**  
    The `call()` method invokes a function immediately, allowing you to specify the value of `this` and pass arguments individually (comma-separated).

  - **Syntax:**  
    ```js
    func.call(thisArg, arg1, arg2, ...)
    ```

  - **Example:**
    ```js
    var employee1 = { firstName: "John", lastName: "Rodson" };
    var employee2 = { firstName: "Jimmy", lastName: "Baily" };

    function invite(greeting1, greeting2) {
      console.log(
        greeting1 + " " + this.firstName + " " + this.lastName + ", " + greeting2
      );
    }

    invite.call(employee1, "Hello", "How are you?"); // Hello John Rodson, How are you?
    invite.call(employee2, "Hello", "How are you?"); // Hello Jimmy Baily, How are you?
    ```

  ---

  #### `apply`

  - **Description:**  
    The `apply()` method is similar to `call()`, but it takes the function arguments as an array (or array-like object) instead of individual arguments.

  - **Syntax:**  
    ```js
    func.apply(thisArg, [argsArray])
    ```

  - **Example:**
    ```js
    var employee1 = { firstName: "John", lastName: "Rodson" };
    var employee2 = { firstName: "Jimmy", lastName: "Baily" };

    function invite(greeting1, greeting2) {
      console.log(
        greeting1 + " " + this.firstName + " " + this.lastName + ", " + greeting2
      );
    }

    invite.apply(employee1, ["Hello", "How are you?"]); // Hello John Rodson, How are you?
    invite.apply(employee2, ["Hello", "How are you?"]); // Hello Jimmy Baily, How are you?
    ```

  ---

  #### `bind`

  - **Description:**  
    The `bind()` method creates a new function with a specific `this` value and, optionally, preset initial arguments. Unlike `call` and `apply`, `bind` does **not** immediately invoke the function; instead, it returns a new function that you can call later.

  - **Syntax:**  
    ```js
    var boundFunc = func.bind(thisArg[, arg1[, arg2[, ...]]])
    ```

  - **Example:**
    ```js
    var employee1 = { firstName: "John", lastName: "Rodson" };
    var employee2 = { firstName: "Jimmy", lastName: "Baily" };

    function invite(greeting1, greeting2) {
      console.log(
        greeting1 + " " + this.firstName + " " + this.lastName + ", " + greeting2
      );
    }

    var inviteEmployee1 = invite.bind(employee1);
    var inviteEmployee2 = invite.bind(employee2);

    inviteEmployee1("Hello", "How are you?"); // Hello John Rodson, How are you?
    inviteEmployee2("Hello", "How are you?"); // Hello Jimmy Baily, How are you?
    ```

  ---

  #### Summary

  | Method | Invokes Function Immediately? | How Arguments Are Passed         | Returns      |
  |--------|-------------------------------|----------------------------------|--------------|
  | `call` | Yes                           | Comma-separated list             | Function's result |
  | `apply`| Yes                           | Array or array-like object       | Function's result |
  | `bind` | No                            | (Optional) preset, then rest     | New function      |

  ---
