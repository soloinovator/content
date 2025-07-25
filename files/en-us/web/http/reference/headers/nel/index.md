---
title: NEL header
short-title: NEL
slug: Web/HTTP/Reference/Headers/NEL
page-type: http-header
status:
  - experimental
browser-compat: http.headers.NEL
sidebar: http
---

{{SeeCompatTable}}

The HTTP **`NEL`** {{Glossary("response header")}} is used to configure network request logging.

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">Header type</th>
      <td>{{Glossary("Response header")}}</td>
    </tr>
    <tr>
      <th scope="row">{{Glossary("Forbidden request header")}}</th>
      <td>No</td>
    </tr>
  </tbody>
</table>

## Syntax

```http
NEL: { "report_to": "name_of_reporting_group", "max_age": 12345, "include_subdomains": false, "success_fraction": 0.0, "failure_fraction": 1.0 }
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Network Error Logging (NEL) explainer](/en-US/docs/Web/HTTP/Guides/Network_Error_Logging)
