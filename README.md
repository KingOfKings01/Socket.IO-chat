# Socket.IO-chat

To use the Socket.IO we need two things.

First connection to the server
To connect to the server I used http connection from node
import { createServer } from 'node:http';

Second connection add into the index.html file

For this we need to use the socket.io library CMD

<script src="/socket.io/socket.io.js"></script>

Both need to be configured and now every time page loads we get a new connection

#Note
If you're behind a reverse proxy such as apache or nginx please take a look at the documentation for it.

If you're hosting your app in a folder that is not the root of your website (e.g., https://example.com/chatapp) then you also need to specify the path in both the server and the client.

We can add disconnect event as well in the connection configuration.

Then if you refresh a tab several times you can see it in action. user connected and disconnected

