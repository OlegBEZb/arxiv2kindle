# arxiv2kindle
This repository contains an *arxiv2kindle_with_latex_processing* notebook which does the following:
1. Downloads the original arxiv page
2. Processes it to fit the shape of your e-reader
3. Sends the obtained pdf file from you gmail to your kindle email. This moves the file to your e-reader
## Google App Password
For security reasons you need to create credentials.py file with dict like the following:  
credentials = {  
    'kindle_email': "YOUR_EMAIL@kindle.com",  
    'your_gmail': "YOUR_GMAIL@gmail.com",  
    'gmailpass': "YOUR_PASS",  
               }  

For creating gmailpass, please follow the [apppasswords](https://myaccount.google.com/apppasswords). Note that the account security settings will have to "allow unsecure apps" for permission to use the Gmail SMTP server with TLS.  
**Do not forget to add this file to .gitignore**
## Parameters
The parameters are initialized in the **Input parameters** passage
```
# the needed_article_url can be an arxiv URL or any string containing an arxiv ID.
needed_article_url = "http://arxiv.org/abs/1709.03856"

# paper settings (decrease width/height to increase font)
landscape = False # False=horizontal, True=vertical
width = "4.2in"
height = "6.55in"
margin = "0.1in"

show_generated_pdf = True
send = False
```
## Notebook launch
To execute the functionality set the parameters mentioned above and run the whole notebook
## TODO
1. Add fontsize parameter