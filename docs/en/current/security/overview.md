# Security

## Encryption in transit

When configured appropriately, K-9 Mail protects your email from being read by eavesdroppers when
in transit from your phone to your mail server. It uses an encryption protocol called TLS for this.

You configure TLS in each of the appropriate account setup screens:

- [IMAP](../accounts/incoming_imap.md#security) or [POP3](../accounts/incoming_pop3.md#security)
- [SMTP](../accounts/outgoing.md#security)

TLS has an additional feature that allows you to authenticate to a server with a client certificate,
either instead of, or in addition to, a normal username and password.
If you have been told you need a client certificate to connect to your mail server,
you can configure it in the above linked screens.

### TLS, SSL, STARTTLS - what is the difference?

TLS was originally an enhancement to an older protocol called SSL, so in some documentation you might
see SSL mentioned. Additionally, [sometimes](https://www.washingtonpost.com/world/national-security/nsa-infiltrates-links-to-yahoo-google-data-centers-worldwide-snowden-documents-say/2013/10/30/e51d661e-4166-11e3-8b74-d89d714ca4dd_story.html)
people informally use "SSL" when they mean "TLS", although SSL itself is now deprecated for security reasons.

STARTTLS is a way of using TLS in certain internet protocols, and is just as secure as TLS.

For more information see [Fastmail's article](https://www.fastmail.help/hc/en-us/articles/360058753834-SSL-TLS-and-STARTTLS).

## End-to-end encryption

K-9 Mail can also use end-to-end encryption, which means that even when your emails are being processed
by intermediate mail servers, they cannot be read other than by the recipient.

It uses a protocol called PGP for this. This is more complicated to set up, but is the only way to ensure your email
wasn't exposed to eavesdroppers somewhere between your phone and the recipient.

End-to-end encryption in K-9 Mail also digitally signs your email, which means a recipient can be
sure that it was you that sent it, rather than someone pretending to be you.

You can set up PGP by following [these instructions](pgp.md).

S/MIME, an alternative end-to-end encryption system, is not currently supported by K-9 Mail.