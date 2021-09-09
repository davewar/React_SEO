# Adding SEO to React App on each app if not using Next.js

- install "react-helmet-async"
- wrap Helmet provider around app
- In the Meta tag on the index.html file - add: data-rh="true"
- In each page - use Helmet to add meta data - see Shop component

https://www.npmjs.com/package/react-helmet-async

```
    <Helmet>

        <title>Hello World</title>
        <link rel="canonical" href="https://www.tacobell.com/" />

    </Helmet>
```

use META SEO inspector to check Helmet working

# Robots.txt

Use Disallow when you dont want crawlers on the page.

Disallow: /login Disallow: /secret

if you want to guarantee no crawler then add below to page

<meta name="robots" content="no index" />

# sitemap.txt

- Deploy site
- Create sitemap.txt file

e.g

```
https://testdw.netlify.app/
https://testdw.netlify.app/login
https://testdw.netlify.app/shop

```

- go to Google Search Console & obtain meta tag. Add meta tag to index.html

e.g

```
<meta
    name="google-site-verification"
    content="12345678978978987blahblah"
/>
```

- Google Search Console - press Verify tag
- added Google Search Console - Add sitemap.txt
