**Add Person

Use HTTP Request to SharePoint Action

```
Method: POST

_api/web/sitegroups/GetById(14)/users

Headers
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose"
}

Body
{"__metadata":{"type":"SP.User"},"LoginName":"i:0#.f|membership|[user email goes here]"}
```



**Remove Person

Use HTTP Request to SharePoint Action

```
Method: POST

_api/web/sitegroups/GetById(14)/users/getbyemail('UserEmail')

Headers
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose",
  "X-HTTP-Method": "DELETE"
}
```
