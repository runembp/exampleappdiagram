Exercise 04:

title Sequence Diagram - New Note MOOC.js

Browser->Server: HTTP POST - Posts the new note
Browser->Server: HTTP GET - Requests /notes/ url
Server->Browser: Sends the HTML
Browser->Server: HTTP GET - Requests the css content
Server->Browser: Sends the main.css
Browser->Server: HTTP GET - Requests the javascript content
Server->Browser: Sends the main.js
Browser->Server: HTTP GET - Requests the json content 
note over Browser:
browser executes the Javascript code to handle the incoming JSON Data
end note

Server->Browser: Sends the data.json
Browser->Server: HTTP GET - Requests the favicon
Server->Browser: Sends the favicon.ico

https://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgU2VxdWVuY2UgRGlhZ3JhbSAtIE5ldyBOb3RlIE1PT0MuanMKCkJyb3dzZXItPlNlcnZlcjogSFRUUCBQT1NUIC0gUG9zdHMgdGhlIG5ldyBub3RlABkXR0VUIC0gUmVxdWVzdHMgL25vdGVzLyB1cmwKAFIGLT4AYgc6IFNlbmQATwZIVE1MACsmdGhlIGNzcyBjb250ZW50ADkcbWFpbi5jc3MALypqYXZhc2NyaXB0ADcpagAzLHNvbgCBMQggCm5vdGUgb3ZlciAAggkICmIAgn0GIGV4ZWN1dGUAgmsGSgCBCQxkZSB0byBoYW5kbGUAgwoFaW5jb21pbmcgSlNPTiBEYXRhCmVuZACDHAYAglYcZGF0YS5qc29uAIJNKmZhdmljb24AgywcABwHLmljbwoKCg&s=default



Exercise 05:

title MOOC Spa Diagram

B->S: HTTP GET the spa url
S->B: Returns the HTML

B->S: HTTP GET the CSS
S->B: Returns the main.css

B->S: HTTP GET the javascript
S->B: Returns the spa.js

note over B
Handles the js code and fetches the JSON data to add to 
the ul and il
end note

B->S: HTTP GET the JSON data
S->B: Returns the data.json

B->S: HTTP GET the favicon
S->B: Returns the favicon.ico

https://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgTU9PQyBTcGEgRGlhZ3JhbQoKQi0-UzogSFRUUCBHRVQgdGhlIHNwYSB1cmwKUy0-QjogUmV0dXJucwAVBUhUTUwAHhVDU1MAHBNtYWluLmNzcwBRFWphdmFzY3JpcHQAVhNzcGEuanMKCm5vdGUgb3ZlciBCCkhhbmRsZQCBAwZqcyBjb2RlIGFuZCBmZXRjaAARB0pTT04gZGF0YSB0byBhZGQgdG8gCnRoZSB1bAAnBWlsCmVuZCBub3RlAIFmFQA3CQCBahNkYXRhLmpzb24AgiAVZmF2aWNvbgCCIhMAEwcuaWNv&s=default

Exercise 06:

title New note created on Mooc SPA

B->S: HTTP POST 201 - Sends new note

note over B 
Javascripts Pushes the new note to the list of notes
end note

https://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgTmV3IG5vdGUgY3JlYXRlZCBvbiBNb29jIFNQQQoKQi0-UzogSFRUUCBQT1NUIDIwMSAtIFNlbmRzIG4AMwcKCgA7BW92ZXIgQiAKSmF2YXNjcmlwdHMgUHVzaGVzIHRoZQAlCSB0bwALBWxpc3Qgb2YAdwVzCmVuZACBAQU&s=default
