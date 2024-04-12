Use when patching the data or setting default on person column

```
{
   '@odata.type':"#Microsoft.Azure.Connectors.SharePoint.SPListExpandedUser",
   Claims: "i:0#.f|membership|" & User().Email ,
   Department: "",
   DisplayName: User().FullName,
   Email: User().Email,
   JobTitle: "",
   Picture: ""
}

```
