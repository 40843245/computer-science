# Fully qualified domain name (FQDN)
## Intro
A fully qualified domain name (FQDN), sometimes also referred to as an absolute domain name, is a domain name that specifies its exact location in the tree hierarchy of the Domain Name System (DNS). It specifies all domain levels, including the top-level domain and the root zone. A fully qualified domain name is distinguished by its lack of ambiguity in terms of DNS zone location in the hierarchy of DNS labels: it can be interpreted only in one way.

## Rule
Each `identifier` must 

+ consist of one or many `digit` (i.e. `0` to `9`), `uppercase letter` (i.e. `A` to `Z`), `lowercase letter` (`a` to `z`), and `hypen` (i.e. `-`).
+ start with an `uppercase letter` or `lowercase letter`

Here, each labels is an `identifier`.

FQDN must 
+ consist of many `labels`.
+ each word is seperated by `delimiter` `.`.
+ ends with the `delimiter` `.`.

## Example
### Example 1
The url `https://en.wikipedia.org/wiki/Fully_qualified_domain_name` has a DNS
`en.wikipedia.org` and the hierarchy of its corresponding FQDN `en.wikipedia.org.` shows as follows.

![image](https://github.com/user-attachments/assets/3695c578-954f-49c4-b47f-ece403377aee)

## Ref
[Fully qualified domain name (FQDN)](https://en.wikipedia.org/wiki/Fully_qualified_domain_name)
