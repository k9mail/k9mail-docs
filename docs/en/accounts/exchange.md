# Office 365 Server Settings

We intend to improve the Office365 support in K-9 Mail. For now you’ll have to manually set up Office365 accounts. Make
sure you’re using at least K-9 Mail 6.201.

For this to work, **IMAP** and **SMTP** need to be enabled for the domain. Depending on the configuration the
administrator may
also have to specifically allow the app “K-9 Mail” to be used to access your account.

1. In the **Set up a new account** screen enter your email address.
2. Tap the **Next** button.
3. In case no automatic configuration is found, tap the **Next** button. Otherwise expand the configuration by tapping the
   arrow next to **Configuration Found** and tap **Edit Configuration**.

4. You should be in the **Incoming server settings** screen now:
    1. Ensure `IMAP` is selected as protocol.
    2. Enter `outlook.office365.com` under server.
    3. Change Security to `SSL/TLS` (Port should automatically change to 993).
    4. Change Authentication to `OAuth 2.0`.
    5. Tap the **Next** button.

5. If your browser is not already logged in to your Office365 account, you will be asked to log in.
6. Afterwards you’ll be asked to grant K-9 Mail (published by Mzla Technologies Corporation) the following permissions:
    - Read and write access to your mail.
    - Access to sending emails from your mailbox. 
    - Maintain access to data you have given K-9 Mail access to 
    - View your basic profile  
7. Tap **Accept**.

8. You should be in the **Outgoing server settings** screen now:
    1. Enter `smtp.office365.com` under server.
    2. Change Security to `STARTTLS` (Port should automatically change to 587).
    3. Change Authentication to `OAuth 2.0`.
    4. Tap the **Next** button.
9. K-9 Mail will automatically use the access you’ve granted it in step 5 and 6.
10. Follow the rest of the account setup procedure