# Storage-Method
Local Storage vs Session Storage vs Cookie vs Session

mechanism
expired
storage
support
apply
size
type
example

localStorage, sessionStorage, and cookies are all client storage solutions.
mechanisms 
storage specific to an individual browser on an individual computer/device.
sessions will need to involve your application server side most likely using a database, but possibly XML or a text/CSV file.

In terms of capabilities, cookies, sessionStorage, and localStorage only allow you to store strings

localStorage and sessionStorage are perfect for persisting non-sensitive data needed within client scripts between pages (for example: preferences, scores in games).

Cookies an be trivially tampered with by the user, and data can also be read from them in plain text 
As cookies are used for authentication purposes and persistence of user data, all cookies valid for a page are sent from the browser to the server for every request to the same domain
 If you are not using SSL, cookie information can also be intercepted in transit, especially on an open wifi.

On the positive side cookies can have a degree of protection applied from security risks like Cross-Site Scripting (XSS)/Script injection by setting an HTTP only flag which means modern (supporting) browsers will prevent access to the cookies and values from JavaScript (this will also prevent your own, legitimate, JavaScript from accessing them).
Typically cookies are used to store identifying tokens for authentication, session, and advertising tracking.

session data usually relies on a cookie token to identify the user for repeat visits (although rarely URL parameters may be used for the same purpose)
As session data is completely controlled by your application (server side) it is the best place for anything sensitive or secure in nature.



## ToDo
- Simple Vue SPA for this illustration.
- Display a table that compare all the example.
