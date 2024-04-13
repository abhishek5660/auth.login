# auth.login

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Login Page</title>
    <link rel="stylesheet" href="https://cdn.auth0.com/js/lock/11.34.2/lock.css">
</head>
<body>
    <div id="login-container"></div>
</body>
</html>
    <script src="https://cdn.auth0.com/js/lock/11.34.2/lock.min.js"></script>
    <script>
        var lock = new Auth0Lock('bmbQMzqsbYWkE8EmJgVPWWiEmKGGsStR', 'dev-v53xhmacimboaelt.au.auth0.com', {
            auth: {
                redirectUrl: 'http://127.0.0.1:5500/lostandfound.html',
                responseType: 'token'
            }
        });
        lock.show();
        lock.on("authenticated", function(authResult) {
            // Use authResult.idToken or authResult.accessToken
            // to perform further actions like saving the token
            // or redirecting the user.
        });
    </script>
</body>
</html>
