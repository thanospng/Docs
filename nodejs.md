## URLs

![URL anatomy](./url_anatomy.jpg)

Node provides (through its ['url' module](https://nodejs.org/api/url.html)) two apis that deal with urls, a legacy and a newer one (the one that you should use).

```js
const url = require('url');

// Parse a url string
const myURL = new URL('https://user:pass@sub.host.com:8080/p/a/t/h?query=string#hash');

// Or use the two-argument constructor for relative urls
const myURL = new URL('/foo', 'https://example.org/');

// Be careful, if neither argument is a valid url, a TypeError will be thrown.

// An URL object has properties that you can read and set, like:
url.hash
url.host // hostname + port
url.hostname
url.href // construct the url string
url.origin // protocol + host, read-only
url.password
url.pathname
url.port
url.protocol
url.search // query
url.searchParams // read-only object, return URLSearchParams object
url.username

// Use .href to get the constructed url (same as toString() and toJSON()), while
// setting the value of this property to a new value is equivalent to creating a new URL object.
```
