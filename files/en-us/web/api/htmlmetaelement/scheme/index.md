---
title: HTMLMetaElement.scheme
slug: Web/API/HTMLMetaElement/scheme
page-type: web-api-instance-property
tags:
  - API
  - Deprecated
  - HTML DOM
  - HTMLMetaElement
  - Property
  - Reference
browser-compat: api.HTMLMetaElement.scheme
---

{{APIRef("HTML DOM")}}{{Deprecated_Header}}

The **`HTMLMetaElement.scheme`** property defines the scheme of the value in the {{domxref("HTMLMetaElement.content")}} attribute.
The `scheme` property was created to enable providing additional information to be used to interpret the value of the `content` property. The `scheme` property takes as its value a scheme format (i.e. `YYYY-MM-DD`) or scheme format name (i.e. `ISBN`), or a URI providing more information regarding the scheme format. The scheme defines the format of the value of the `content` attribute.
The `scheme` content is interpreted as an extension of the element's {{domxref("HTMLMetaElement.name")}} if a browser or user agent recognizes the scheme.

This property is deprecated and should not be used on new web pages.

## Value

A string.

## Examples

```js
// given <meta name="identifier" content="1580081754" scheme="ISBN">
let meta = document.querySelector("meta[name='identifier']");
console.log(meta.scheme);
// "ISBN"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{HTMLElement("meta")}}
