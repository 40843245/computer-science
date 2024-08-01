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

## Ref
[Canonical Name (CNAME) record](https://en.wikipedia.org/wiki/CNAME_record)
