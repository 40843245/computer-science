# Canonical Name (CNAME) record
## Intro
A Canonical Name (CNAME) record is a kind of resource record in DNS that maps one domain name into another canonical name.

## Specified
DNS CNAME records are specified in RFC 1034.

## Clarified 
DNS CNAME records are clarified in Section 10 of RFC 2181.

## Example

There is a DNS zone as follows:

| FQDN                  |  TYPE |  VALUE |
| --------------------- | ----- | ------ |
| bar.example.com.      | CNAME  | foo.example.com. |
| foo.example.com.      |  A   |   192.0.2.23 |

When an `A record` lookup for `bar.example.com.` is carried out, the process is described as follows.

The resolver will see a CNAME record then restart the lookup for `foo.example.com.`, and finally return `192.0.2.23`.

Illustrated as follows.

![CNAME_ex1](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

[CNAME_ex1](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

## Ref
[Canonical Name (CNAME) record](https://en.wikipedia.org/wiki/CNAME_record)
