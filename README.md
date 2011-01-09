

## SDKs

### NodeJS

<pre>
sdk = require('account-hub-sdk')
sdk.init({
    account_authkey: [...]
});

// when the Bitcoin button is pressed:
sdk.request(invoice, ...callback...);
</pre>

where
<pre>
invoice = {
    title: "XXXL Coffee, 4 timbits",
    amount: "7.58 CAD"
}
</pre>
if there's an error, your callback will be called with e.g.
<pre>
{
    error: {
        name: "AuthError",
        message "The authkey you provided does not currently have any access permissions."
    }
}
</pre>
otherwise, if/when the invoice is paid, your callback will be called with
<pre>
{paid: true}
</pre>

### Python

TODO

### Ruby

TODO

