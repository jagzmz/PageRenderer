# Page-Renderer
- A simple plugin for rendering html pages on server side that are generated by javascript.
- It creates the html page on server side for SEO purposes and OG:Tags.


# Example
- Let us consider we need the http://example.com to be rendered on server-side.

- this plugin makes it extremey easy to do so. Just add an entry for http://example.com to the configuration provided to the pageRenderer.init() method.


- It should look like this:

```js
#!/usr/bin/env node
pageRenderer.init({
    "port":3007, // port on which the pagerenderer must run default is 3007
    "sites":[
        {
            "hostBot":"http://example.bot.com",
            "hostClient":"http://example.com"
        },
        {
            "hostBot":"http://anotherexample.bot.com",
            "hostClient":"http://anotherexample.com"
        }
    ]
});

```

- Now you just have to redirect all the requests comming from bots to http://example.bot.com


       
