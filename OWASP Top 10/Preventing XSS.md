Preventing XSS

* Encoding - < becomes &lt;, breaks the scrip tag
* Filtering - <script> becomes script
* Validating - compare input against white list
* Sanitization - combination of escaping, filtering, and validation 