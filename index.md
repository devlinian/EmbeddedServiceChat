<html>
  <body>
  <script type='text/javascript'>
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
            
            //Passing Web Context to Prechat - BEGIN
        
    window.addEventListener("onEmbeddedMessagingReady", e => {
        
        embeddedservice_bootstrap.prechatAPI.setVisiblePrechatFields({
            // List the pre-chat field names with the value and whether
            // it's editable in the pre-chat form.
            "_firstName": {
              "value": "Test",
              "isEditableByEndUser": true
            },
            "_lastName": {
              "value": "User",
              "isEditableByEndUser": true
            },
            "_subject": {
              "value": "test subject",
              "isEditableByEndUser": true
            },
            "Phone": {
              "value": "1234567898",
              "isEditableByEndUser": true
            },
            "_email": {
              "value": "test.user@test.com",
              "isEditableByEndUser": true
            },
            "Company_Name": {
              "value": "test company",
              "isEditableByEndUser": true
            }
        });
      
        //Set invisible prechat field
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
            "Customer_ID" : "123456"
        });
    });

            embeddedservice_bootstrap.init(
                '00DcT000000CEfH',
                'General_Support_Chat_with_Bot',
                'https://buildertrend--kspartial.sandbox.my.site.com/ESWGeneralSupportChatw1729287295651',
                {
                    scrt2URL: 'https://buildertrend--kspartial.sandbox.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };
    
    //Passing Web Context to Prechat - END
</script>
<script type='text/javascript' src='https://buildertrend--kspartial.sandbox.my.site.com/ESWGeneralSupportChatw1729287295651/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</body>
</html>
                                        
