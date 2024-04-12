## Add Person

Use HTTP Request to SharePoint Action

How to get "GroupId" of SharePoint Group.
1. Go to the group page in Site Permission page
2. Look at the URL on the web browser
3. https://URL.sharepoint.com/sites/siteaddress/_layouts/15/people.aspx?MembershipGroupId=4826 => 4826 is this group's Id

```
Method: POST

_api/web/sitegroups/GetById(GroupId)/users

Headers
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose"
}

Body
{"__metadata":{"type":"SP.User"},"LoginName":"i:0#.f|membership|[user email goes here]"}
```



## Remove Person

Use HTTP Request to SharePoint Action

```
Method: POST

_api/web/sitegroups/GetById(GroupId)/users/getbyemail('UserEmail')

Headers
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose",
  "X-HTTP-Method": "DELETE"
}
```
