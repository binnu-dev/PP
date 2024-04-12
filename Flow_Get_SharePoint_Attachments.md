How to get SharePoint List Item Attachments and Use them (send email and etc)

1. Initialize Array Variable

2. Get Attachments (Identified by ID of SharePoint Item)

3. Get Attachment Content (by File Identifier from the previous step) -> Create a loop

4. Append to Array Variable

{
"name":DisplayName,
"content": body('Get_attachment_content')
}

5. for Attachment Items -> Use the Array Variable


https://www.youtube.com/watch?v=DCxwCALD7hk
