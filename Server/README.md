# Server

Directory for server app

<p>Server API</p>
<p>
	<ul>
		<li>	
			Establishing Connection:
			<br>Server : "Hello, identify yourself"
			<br>Client : "Hello, @{1}" 1 - Username
			<br>If username is taken add number after username eg. Mike1, Mike2, Mike3  
		</li>
		<li>
			Change username:
			<br>Client : "USERNAME @{1}" 1 - New Username
		</li>
		<li>
			If Username is taken
			<br>Server : "Username @{1} is taken already" 1 - Username
		</li>
		<li>
			If Username is registered
			<br>Server : "Username @{1} is registered, to log in use "LOGIN @USERNAME PASSWORD command"
		</li>
		<li>
			Sending Message Client -> Chatroom:
			<br>Client : "MSG {1}" 1 - Message Content
		</li>
		<li>
			Sending Message Server -> Client:
			<br>Server : "@{1} MSG {2}" 1 - Username who sent msg, 2 - Message Content
		</li>
		<li>
			Changing chatroom:
			<br>Client : "JOIN #{1}" 1 - Chatroom name
			<br>If user is banned from chatroom
			<br>Server: "Sorry, you are banned from #{1} room" – 1 Chatroom name
		</li>
		<li>
			Sending Private messages Client -> Server:
			<br>Client : "PRIVMSG @{1} {2}" 1 - Username to recive priv msg, 2 - Message Content
		</li>
		<li>
			Sending Private messages Server -> Client:
			<br>Server : "@{1} PRIVMSG {2}" 1 - Username who sent private message, 2 - Message Content
		</li>
		<li>
			Create chatroom:
			<br>Client : "CREATEROOM #{1}" 1 - Chatroom name
			<br>If Room is already created
			<br>Server : "Room #{1}, is already created, to join room use "JOIN #RoomName" "
		</li>
		<li>
			Mute/Unmute User:
			<br>Client : "MUTE @{1}" 1 - Username to be mute/unmuted
		</li>
		<li>
			Kick User:
			<br>Client : "KICK @{1}" 1 - Username to be kicked
		</li>
		<li>
			Ban/Unban User:
			<br>Client : "BAN @{1}" 1 - Username to be banned/unbanned
		</li>
		<li>
			Ping request:
			<br>Server : "PING"
			<br>Ping response
			<br>Client : "PONG"
		</li>
		<li>
			Register Account:
			<br>Client : "REGISTER @{1} {2} {3}" 1 - Username to register, 2 - password, 3 - email
		</li>
		<li>
			Log In:
			<br>Client : "LOGIN @{1} {2}" 1 - Username to login, 2 - password
		</li>
	</ul>
</p>
