<html>
  <body>
  <script type='text/javascript'>
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
          
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
                                        
