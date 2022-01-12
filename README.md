# reactCatchInternetExplorer
A few lines of code to display a Message if visitor is using old IE.

All you need is the Script-Block in the index.html\
Just copy it into your /public/index.html into the body and customize the message.

```javascript
<script>
    var ieMode = window.document.documentMode;
    if (ieMode) {
        console.log('ieMode: ', ieMode);
        var userMessage = document.createElement('h3');
        userMessage.innerHTML = 'Browser is not supportet.';
        document.body.appendChild(userMessage);
    }
</script>
 ```
    
