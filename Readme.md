# arxiv2kindle
## Google App Password
For security reasons you need to create credentials.py file with dict like the following:  
credentials = {  
    'kindle_email': "YOUR_EMAIL@kindle.com",  
    'your_gmail': "YOUR_GMAIL@gmail.com",  
    'gmailpass': "YOUR_PASS",  
               }  

For creating gmailpass, please follow the [apppasswords](https://myaccount.google.com/apppasswords). Note that the account security settings will have to "allow unsecure apps" for permission to use the Gmail SMTP server with TLS.  

**Do not forget to add this file to .gitignore**