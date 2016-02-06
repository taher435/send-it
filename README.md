MailChimp + Mandrill
===

####Set up

1. Configure mandrill_settings in <environment>.rb in config folder
  
    ````
    config.mandrill_settings = {
    	:api_key => "X",
      	:from_email => "from@example.com",
      	:reply_to => "reply@example.com",
      	:from_name => "Sender Name",
  	}
	````
You can get **api_key** from your mandrill account. Also, make sure you configure your sending domain in mandrill to avoid mail bounce.

######Note

You need to verify the sending email address domain in order to send emails using the mandrill API. See the notice from mandrill below

![mandrill notice](http://i.imgur.com/KkVlg7A.png?1)

####Thanks to
1. [http://codepen.io/Albzi/pen/aOwvay](http://codepen.io/Albzi/pen/aOwvay) for Sending animation on processing screen

####To Do

1. ~~Proper validations on page~~
2. Use SideKiq for background processing
3. Use Web socket to report status to the client
4. Write unit tests
5. Clean up code
6. Support attachments
7. Support tracking (Google analytics)
8. Test the entire thing
9. Add login with Google option