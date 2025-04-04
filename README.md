# HTTP API Test Iframe

A lightweight and customizable component designed to quickly test and interact with HTTP APIs. Easily embed this iframe in your project to debug API endpoints and visualize responses without leaving your browser.

## Features

 - Easy Embedding: Insert the provided iframe code into your HTML.
 - Customizable Settings: Configure base URLs, paths, HTTP methods, headers, and request bodies.
 - Responsive Design: The iframe automatically adjusts its height based on content.
 - Quick API Testing: Send requests and view responses instantly.

## Demo

Try out the live demo below (or view it directly in the [live demo](https://lucasmenendez.github.io/http-api-test-iframe/demo.html)):

```html
<iframe
    style="border: 0;"
    width="60%"
    src='https://lucasmenendez.github.io/http-api-test-iframe/?conf={"baseUrl": "https://httpbin.org","defaultPath": "/anything/{id}","defaultMethod": "POST"}'
    onload='javascript:(function(o){o.style.height=o.contentWindow.document.body.scrollHeight+"px";}(this));'
></iframe>
```

<br/>

<div style="text-align: center;">
    <img src="./screenshot.png" width="400px"/>
</div>

## Default configuration

By default, the component uses the following configuration. You can override these settings by passing a custom configuration via the conf parameter in the iframe URL:

```javascript
const defaultConfig = {
    baseUrl: "https://api.example.com",
    defaultPath: "/users/{id}",
    defaultMethod: "GET",
    defaultHeaders: {
        "Content-Type": "application/json",
    },
    defaultBody: '{"name": "John Doe"}',
    excludedMethods: [],
}
```

## How to Use

1. **Embed the Iframe**: Copy the demo code into your HTML file where you want the component to appear.
2. **Customize your request**: Adjust the conf parameter in the iframe’s src URL to change the API endpoint, HTTP method, headers, and body.
3. **Test your API**: Use the embedded interface to send requests and view the responses in real time.


## Contributing
Contributions are welcome! If you have suggestions or improvements, please open an issue or submit a pull request.

## License
This project is licensed under the [AGPL-3.0 license](./LICENSE).

## Contact
For questions or feedback, please open an [issue on the GitHub repository](https://github.com/lucasmenendez/http-api-test-iframe/issues/new).






