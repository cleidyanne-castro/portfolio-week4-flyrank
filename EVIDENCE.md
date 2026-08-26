# Evidence

## Scope

The single dynamic feature is the contact form. The page remains a static HTML site.

## Test matrix

| Case | Input | Expected result | Evidence |
| --- | --- | --- | --- |
| Required name | Empty name | Browser blocks submission | Native required validation |
| Email format | `not-an-email` | Browser blocks submission | Native email validation |
| Required message | Empty message | Browser blocks submission | Native required validation |
| Valid form | Name, valid email, and message | FormSubmit receives the request | Requires a real mailbox check |
| Narrow layout | Mobile viewport | No horizontal overflow and readable fields | Browser screenshot |

## Data flow

The browser sends the submitted name, email, and message to FormSubmit. FormSubmit forwards the message to the configured email address. No application database is used.

## Limits

The repository cannot prove mailbox delivery without access to the recipient inbox. FormSubmit is an external service and can change its response or delivery behaviour.
