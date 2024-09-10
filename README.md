# backend-task

<h1>Task:</h1>

<li>Create backend application API for business domain.</li>
<li>Create your repo (preferably on Github) for backend-dev-task solution and share it us.</li>

<h2>Requirements:</h2>
<li>Use Laravel 11</li>
<li>Use OOP</li>
<li>Follow best practices SOLID, Clean code etc.</li>
<li>Data storage solution is up to you. DB, filesystem, cache, memory... </li>
<li>Cover code by tests. If you need use e.g. PHPUnit. There is no need to cover all code, just create a couple to show the principle</li>
 
<h3>Optional requirements for which additional points will be awarded for:</h3>
<li>Using DDD (Domain-Driven Design) together with Laravel</li>

<h2>Business logic:</h2>

Online shop has product sets and products. One product can only exist within one set. Product set is published if at least one product inside the set is published.
Set cannot contain 0 products. Only non-confidential data is returned for public API. Restricted API endpoints must be secured by API key.

<h4>Product set consists from:</h4>
<li>id</li>
<li>name - maximum length of 60</li>
<li>slug - made from name by default</li>
<li>collection of products</li>

<h4>Product consists from:</h4>
<li>id</li>
<li>sku code</li>
<li>name - maximum length of 40</li>
<li>slug - made from name by default</li>
<li>type - device or service</li>
<li>condition - new, used, refurbished</li>
<li>description title</li>
<li>description text</li>
<li>price</li>
<li>wholesalePrice - confidential</li>
<li>published - true, false</li>

<h4>Functionality</h4>
<li>[Public] Find product set - returns non-confidential data for active sets</li>
<li>[Restricted] Create product set</li>
<li>[Restricted] Update product set</li>
<li>[Restricted] Create product</li>
<li>[Restricted] Update product</li>
<li>[Restricted] Delete product</li>
