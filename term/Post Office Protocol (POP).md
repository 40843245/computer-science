# Post Office Protocol (POP)
## Intro
Post Office Protocol (POP) is an application-layer Internet standard protocol that is used by e-mail clients to retrieve e-mail from a mail server.
## History
### POP1
POP1, was specified in RFC 918 (in 1984 year) by Joyce K. Reynolds.

### POP2
POP2 was specified in RFC 937 (in 1985 year).

### POP3
POP3 was originated from RFC 1081 (in 1988 year).

But the most recent specification is RFC 1939

### POP4

POP4 exists only as an informal proposal adding basic folder management, multipart message support, as well as message flag management to compete with IMAP

However, its development has not progressed since 2003.

## Comparison 
The main difference between POP and IMAP are as follows:

| item to compare | POP | IMAP |
| - | - | ----- |
| easy to implementation? | easier to implement | harder to implement |
| How to treats the mailbox? | as a single store | `Unknown` |
| has concept of folders? | No | Yes |
| view | completely static view (and not provide a mechanism to show any external changes in state during the session.) | dynamic view (and sends responses for external changes in state, including newly arrived messages, as well as changes made to the mailbox by other concurrently connected clients.) |

For more details, visit [Comparison with IMAP section of POP (Wiki)](https://en.wikipedia.org/wiki/Post_Office_Protocol)

## Related requests for comments (RFCs)
+ RFC 918 – POP1
+ RFC 937 – POP2
+ RFC 1081 – POP3
+ RFC 1939 – POP3 (STD 53)
+ RFC 1957 – Some Observations on Implementations of the Post Office Protocol (POP3)
+ RFC 2195 – IMAP/POP AUTHorize Extension for Simple Challenge/Response
+ RFC 2384 – POP URL Scheme
+ RFC 2449 – POP3 Extension Mechanism
+ RFC 2595 – Using TLS with IMAP, POP3 and ACAP
+ RFC 3206 – The SYS and AUTH POP Response Codes
+ RFC 5034 – The Post Office Protocol (POP3) Simple Authentication and Security Layer (SASL) Authentication Mechanism
+ RFC 8314 – Cleartext Considered Obsolete: Use of Transport Layer Security (TLS) for Email Submission and Access



## Ref
[Post Office Protocol (POP)](https://en.wikipedia.org/wiki/Post_Office_Protocol)
