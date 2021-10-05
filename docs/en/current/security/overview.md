# Security

Communication security is an increasingly important subject. K-9 Mail aims to provide intuitive e-mail security in many 
forms, both in terms of supporting secure login to your e-mail server and in the security of the e-mail itself.

To this end, K-9 Mail supports a variety of mail server authentication methods and has had 
longstanding support for OpenPGP and future plans to support S/MIME.

## Server Authentication

We currently support the following secure authentication methods

* Client-side TLS certificates
* CRAM-MD5 encryption (the most common form)

We support both the STARTTLS and running over TLS. We review our [TLS protocols and ciphers](ssl.md) in 
response to recent attacks.

## Encryption & Signing Emails

K-9 currently supports PGP/MIME encrypted e-mail through an open API that any application can implement in order to 
encrypt and decrypt e-mail. We have worked on this API along with the developers of OpenKeychain, a security-audited 
application that supports PGP.

For more information on using PGP/MIME in K-9 see our [documentation on PGP/MIME](pgpmime.md).

The other common e-mail encryption and signing implementation is S/MIME. K-9 currently does not directly integrate with 
any S/MIME providers. Some apps may provide S/MIME functionality but they are neither maintained nor do they directly 
integrate with K-9. For information on S/MIME see our [documentation](smime.md).
