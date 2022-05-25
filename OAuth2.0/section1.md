Section 1
==========

### A Brief History of OAuth   

In the past, each services used different tools for authentication of third party apps. However, they had one same goal -> <b>[Applications to access data from third party apps without the users sharing their password]</b> <br>

Mechanisms of tools were similar. So the developers started to work out together to solve the problem => the result : OAuth<br>

### How OAuth Improves Application Security
* One of the most common ways applications handle authentication is with a simple username and password prompt within the app. -> e.g.) [Exchange the password for a session cookie]<br>

* OAuth improves the security of a system by reducing the number of places users enter passwords and give you much more flexibility in the future<br>

### OAuth vs OpenId Connect
* OAuth and OpenId Connect are often used together but they are different things.<br>

#### OAuth (Accessing APIs)
* Designed for application to get access to APIs. The application doesn't need to know who the user is that's using.  <br>

* Think of 'Hotel Service'. <br>
(1) Once the person at the front-desk check out my identification : <b>Authorization Server</b><br>
(2) They hand out these key cards : <b>Access tokens</b><br>
(3) With those key cards, I can access to hotel resources : <b>The resource </b><br>

* They do not care who the person is, who's using the card. They just check whether the key cards are valid for the door. <br>

* But what if, the app wants to know about identification?  In this case, OpenID connect is needed.<br>

#### OpenId Connect (Identifying Users)
* Takes OAuth as a foundation and it adds in user identity information on top<br>
* Extension of OAuth and that extension providers a mechanism where the OAuth Server can actually communicate data about the user back to the application.<br>
* OAuth issues access tokens to apps, OpenID connect issues ID tokens to apps.ID token is a statement about the user.<br>