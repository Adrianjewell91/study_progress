Technical Specifications for Theorizer MVP:

1. A ruby on rails backend with authentication for users using the A/a authentication paradigm, built in the style of A/a.
    1. An auth endpoint for authenticating a user. /session and /users
    3. An endpoint for serving the static files. /home
    4. An CRUD endpoint for logging queries. (Two schema options, a separate table for queries, and a foreign key for the user, probably better so we can store dates).  /query
2. A ML service - API hosted separately /analysis - This can also his the auth endpoint to authenticate a request, and pass it as an orchestrator. But I feel like there's a better way to do it. 
    1. Build the ML Model and run it locally, probably in python with flask. 
        1. Run a small server with one endpoint, and then when the endpoint is hit, authenticate the request and then make the analysis.
        2. Cache the analysis and also cache the session tokens last used - Could I do a performance test with this and measure the results, using a cache and not using a cache for this section?
            1. Make 1000 requests and measure the time using the caches, and not using them (no cache, just auth cache, and just request cache, and then both), and see the time, and report the results, that would be interesting.
    2. Put the ML API on a cloud server and host the API endpoint.
    3. Authenticate it so that only an authorized user can make the request, and when the request is made, the api sends a message to the app to store a query count. 
        1. The session token cookie has to be passed to the ML api endpoint, and the ML service has to pull the session token from it. 
        2. Encryption of the cookie? 
    4. ML endpoint can store an LRU cache of the last five recently used session tokens. 
3. A frontend served from the RoR instance:
    1. Do I use React or Web components or straight vanilla javascript? That depends. I will definitely be bundling, but I want it to work on all browsers (IE, Chrome, Safari, Firefox). Will have to test it. 
        1. Pros: React - industry standard right now, 
        2. Web Components: the future.
        3. Vanilla: I can just do it the way I want with no extra stuff, and have it be backward compatible, and if I use vanilla, what style should I use? God, there is too much to do here. 
    2. An authentication page to log in or sign up. 
    3. An homepage with a piano and music staff, on which you can add notes. 
    4. The staff and piano are linked together, so when I click a note, it gets added to the staff and vice versa. Perhaps this is possible only to a certain extent.
    5. Mobile-first: what does this mean? 
        1. The piano scales accordingly: how will I do this? At full screen the piano is a full width, and at certain widths the piano stops scaling and becomes scrollable, and then disappears.
            1. Phone 214px?: only staff. 
            2. Ipad 760px, scrollable piano.
            3. Large ipad: 900 px scrollable
            4. Screen 1200px: full piano.
        2.  Should the piano key change size? No, they should take up a definitive amount of space, because piano keys don’t change size, or maybe have two sizes. 
    6. Then an ‘analyze button’.
    7. Design will be similar to the current one. 
4. Tests for all aspects of the project and some kind of test analyzer that shows the whole thing is tested. Use what David Boldow is using. 
5. Set up a CI/CD pipeline through Jenkins for both the service and the web app equivalent to what I did at WSI, so I can test it using automate test scripting, and deploy from GitHub branches to the server. This will be all on AWS or something similar I guess. 

TDD:

Tests suites for controller functions:
	- When I look up a user, the query will return a ORM object that includes the user and the number of queries they have made, and their session token, and their password hash.
	- When I add user, I must include a username, and a password in their entries.
	- When I add a user, the number of queries made is set to zero. 
	- When I authenticate a user successfully, the return value will be the session token.
	- When I logout a user, a request must be sent to the ML service to remove that session token from the cache. 
	- When I fail to authenticate a user with username and password, an error will be returned. 
	- When a query is stored, it stores the correct date, and increments total number of queries for that user by one (tests the functionality of the table). 
Tests for Routes:
	- When I make a request to add a user, it should work when valid and fail when invalid payload.
	- When I request a session token, it should work when valid and fail when invalid. 
	- When I record a query same. 
	- When I request the home page, I should get the login page when user is not authenticated, and the homepage, when user is authenticated.
Tests for the ML service functions:
	- When I make the request, the first thing the service will do is authenticate the user. 
	- When I pass a valid session token the service will call the analysis function. 
	- When I pass an invalid token the service will throw an error. 
	- When the analysis function is called, the function will first check the cache before making a query.
	- After a period of a few minutes, a session token must be removed from the cache for security purposes.
	- When the analysis function is called, and the cache does not store the query, it will make an analysis.
	- When the analysis is made, it should work correctly (make twenty tests perhaps.)
ML Service Routes:
	- When I make the call with correct credentials, the request should succeed, and fail when the credentials are invalid (invalid payload or invalid credentials).
Tests for the frontend functions:
	- Requests: When I make a request to the ML service, it should include a payload that is valid and also the session information. 
	- Requests: When I make a request for authentication, it should include both the username and password of the user as the payload.
	- When the page loads, there should be three major sections: the staff, the keyboard, and the analysis section (visual test).
	- Tests for the keyboard: the keyboard should have 88 keys, and each one should work (one click for selection, one click for de-selection).
	- Refresh the page and whatever was selected should load back up (store configuration in local storage or similar). 
	- Clicking on the analyze button should initialize an API request. 

