---
title: "Request: method property"
short-title: method
slug: Web/API/Request/method
page-type: web-api-instance-property
browser-compat: api.Request.method
---

{{APIRef("Fetch API")}}{{AvailableInWorkers}}

The **`method`** read-only property of the
{{domxref("Request")}} interface contains the request's method (`GET`,
`POST`, etc.)

## Value

A {{jsxref("String")}} indicating the method of the request.

## Examples

In the following snippet, we create a new request using the
{{domxref("Request.Request", "Request()")}} constructor (for an image file in the same directory as
the script), then save the method of the request in a variable:

```js
const myRequest = new Request("flowers.jpg");
const myMethod = myRequest.method; // GET
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [ServiceWorker API](/en-US/docs/Web/API/Service_Worker_API)
- [HTTP access control (CORS)](/en-US/docs/Web/HTTP/Guides/CORS)
- [HTTP](/en-US/docs/Web/HTTP)
