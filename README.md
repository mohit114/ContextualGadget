# ContextualGadget
A contextual gadget to trigger when hello world is available in email subject or email body.

NOTE: The steps below do not result in a fully working gadget. 
      It shows up as being installed but no card is displayed when an email with "Hello World" is received. 
      This might need a paid account i.e we need to buy a domain from google. Please go through this link
      https://stackoverflow.com/questions/43329110/is-it-possible-to-test-and-develop-gmail-contextual-gadgets-using-regular-gmail
      Any help is highly appreciated.

# Steps to publish the gadget
1. Go to the https://console.developers.google.com and create a new project.
2. On the Dashboard for the new project click "ENABLE APIS AND SERVICES".
3. Select Google Apps Marketplace SDK under "Google APIs" tab.
4. On the "Google Apps Marketplace SDK" page click "Enable" button.
5. Click on the "Configuration" tab.
6. Click on "Create an OAuth 2.0 client ID" link.
7. Under Credentials tab click on Create credentials dropdown button and "select OAuth client ID".
8. Click on "Configure consent screen" 
9. Give a product name and click on save button.
10. Choose application type as WebApplication.
11. Give a name for client and click create button.
12. You will now get a clientId and secret key popup; click OK.
13. Go to Dashboard and click on "Google Apps Marketplace SDK" link under API section.
14. Click on Configuration tab.
15. Give a description to your gadget.
16. Check Enable Individual Install checkbox
17. Add 4 images. Size should be as mentioned in the configuration. Image links are below:
    https://raw.githubusercontent.com/mohit114/ContextualGadget/master/images/hello-world-128.png
    https://raw.githubusercontent.com/mohit114/ContextualGadget/master/images/hello-world-96.png
    https://raw.githubusercontent.com/mohit114/ContextualGadget/master/images/hello-world-48.png
    https://raw.githubusercontent.com/mohit114/ContextualGadget/master/images/hello-world-32.png
18. Enter Terms of service url as :
    https://raw.githubusercontent.com/mohit114/ContextualGadget/master/tos.html
19. Check "Universal navigation extension" checkbox and provide url as : (it is the url to navigate when your app is clicked which will be 
    available after installing the gadget under google apps section of gmail)
    https://github.com/mohit114/ContextualGadget
20. Check "Gmail contextual gadget extension"<br/>
    Extractor URL: google.com:HelloWorld<br/>
    Gadget URL: https://raw.githubusercontent.com/mohit114/ContextualGadget/master/gadget.xml<br/>
    Scopes: "Mail - Subject Line" and "Mail - Message Body"<br/>
21. Click Save changes button.
22. Now you will see a button "Test installation flow" at the top.
23. Click "Test Installation Flow" button
24. Installation should start. Choose to your gmail account and allow every access.
25. The gadget should now be installed to your Gmail account
26. Log into gmail with the clear gadget cache option set: https://mail.google.com/mail/u/0/?nogadgetcache=1
27. Click on google apps on universal navigation bar of gmail.
28. Scroll down and you could see your app. If not please sign out and sign in again.
