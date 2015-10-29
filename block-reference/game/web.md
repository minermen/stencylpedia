# Game > Web

***

> View our article on [Web Requests](http://www.stencyl.com/help/view/web-requests/) for an explanation of these blocks.

***

## Web Browser

### Open URL in Browser

![open-url-block](http://static.stencyl.com/pedia2/block-images/8%20-%20Game/0%20-%20Web/show-browser.png)

Opens the given URL in the system's default web browser. On mobile devices, this will open up the browser app. To view pages in-game, use the [Web Views](http://community.stencyl.com/index.php/topic,26708.0.html) extension.

```
openURLInBrowser([TEXT]);
```

***

## HTTP Requests

### GET Request

![get-block](http://static.stencyl.com/pedia2/block-images/8%20-%20Game/0%20-%20Web/visit-site.png)

Issues an HTTP GET request at the given URL, then executes the enclosed blocks if the request succeeded. The server's response is enclosed in the `site's response` block.

```
visitURL([TEXT], function(event:Event):Void {
	[ACTIONS]
});
```

***

### POST Request

![post-block](http://static.stencyl.com/pedia2/block-images/8%20-%20Game/0%20-%20Web/visit-site-post.png)

Issues an HTTP POST request at the given URL with the given parameters, then executes the enclosed blocks if the request succeeded. The server's response is enclosed in the `site's response` block.

Parameters are pased in as key=value pairs, separated by ampersands (&), like this `name=John&id=123456`.

```
postToURL([TEXT], [TEXT], function(event:Event):Void {
	[ACTIONS]
});
```

***