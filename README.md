#Example
#Lists
#Unordered
#* Item 1
#* Item 2
#  * Item 2a
#  * Item 2b

#Ordered
#1. Item 1
#1. Item 2
#1. Item 3
#   1. Item 3a
#   1. Item 3b

#Images
#![GitHub Logo](/images/logo.png)
#Format: ![Alt Text](url)

#Links
#http://github.com - automatic!
#[GitHub](http://github.com)

#Blockquotes
#As Kanye West said:

#table
# text | text
# ----|-----
#text |text



> We're living the future so
> the present is our past.
Inline code
I think you should use an
`<addr>` element here instead.


In this repository I want to discribe, how you can setting the **LDAP** on Opensearch.
## Opensearch with LDAPS
For settin you need:
1. Open the directory */opt/...plugins/opensearch-security/securityconfig/config.yml*
2. Change setting for **ldap**:
  *This setting on **config.yml**:
 ```
authc:
  ldap:
    http_enabled: true
    transport_enabled: true
    order: 1
    http_authenticator:
      type: basic
      challenge: false
    authentication_backend:
      type: ldap
      config:
        ...
```
  *This setting  on **config.yml** too:
```
authc:
  ldap:
    http_enabled: true
    transport_enabled: true
    order: 1
    http_authenticator:
      type: basic
      challenge: false
    authentication_backend:
      type: ldap
      config:
        ...
```

Configuretion for second paer code:
Name | Description
---------|-------------
**rolebase** | Specifies the subtree in the directory where role/group information is stored.


If you complite two part, ldaps well be work sucsessfully
* [x] First part
* [x] Second part

And how say someone:
>Well done!

All information you can find on [official site](https://opensearch.org/docs/security-plugin/configuration/ldap/)
![Rubius](https://planyway.com/)
