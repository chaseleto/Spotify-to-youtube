# Spotify-to-youtube
Creates a YouTube playlist from an existing Spotify library.
This currently only works from likes.
testing readme line
testing 2

----------------------------------- SETUP AUTHENTICATION -------------------------------------------------
Youtube: 
Open a new tab
Open the developer tools (Ctrl-Shift-I) and select the “Network” tab
Go to https://music.youtube.com and ensure you are logged in
Find an authenticated POST request. The simplest way is to filter by /browse using the search bar of the developer tools. If you don’t see the request, try scrolling down a bit or clicking on the library button in the top bar.
Firefox
Verify that the request looks like this: Status 200, Method POST, Domain music.youtube.com, File browse?...
Copy the request headers (right click > copy > copy request headers)
Chromium (Chrome/Edge)
Verify that the request looks like this: Status 200, Type xhr, Name browse?...
Click on the Name of any matching request. In the “Headers” tab, scroll to the section “Request headers” and copy the entire Cookie. Paste this into the headers_auth.json file along with your user-agent information.

Spotify:
Create a developer account on https://developer.spotify.com/ and create a new program, find your client ID and Secret key and paste those into Config.py. Navigate to program settings on the spotify website and add the redirect URI that is in the config file or create your own (must match)
