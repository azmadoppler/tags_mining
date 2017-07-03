# tags_mining
**Description** : using twitter API to get user's interest by reverse engineering
# TODO
Added the counting method.
## Requirement
* Node.js 
* Google Map API
* Twitter API key
* Unzipped program OR Git
## How to insert API Key
In the first file for tags_mining.js will need Twitter API key. You will need to insert all of the key here 
```javascript
var T = new Twit({
  consumer_key: '',
  consumer_secret: '',
  access_token: '',
  access_token_secret: ''
});//insert your key in bracket
```
In the first file for tags_googleAPI.js will need Google API key. You will need to insert it here
```javascript
var googleMapsClient = require('@google/maps').createClient({
  key: ''//insert your key in bracket
});
```
## How to use the script
0. Download the file or Clone
1. You should run this command in Command Line to check your node installation -> node --version
2. tags_mining.js will search the twitter for all the keyword with location. You can change the search query item by changing variable called searchParameter (default = takoyaki) 
3. to run tags_mining.js simply open command line in that directory and type -> node tags_mining.js 
4. tags_mining will output the file with text file named user_with_tag.txt
5. After that use the tags_googleAPI.js to change the location from the text file into the real world location
6. to run tags_googleAPI.js simply open command line in that directory and type -> node tags_googleAPI.js
7. output will be in the file named tags_and_location.txt
