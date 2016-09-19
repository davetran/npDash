# npDash

## Usage
npDash.html and assembly.json need to be in the same directory to operate.

###Firefox
npDash can be run locally from Firefox.

###Chrome ( and other webkit browsers?)
Chrome disables loading of local files (assembly.json) for security reasons.
One option to get around this is to start chrome with the "--allow-file-access-from-files" flags but poses a security risk.
Another option is to host a local-server using node.js or python:

#### Python 2.x
Go to the directory were npDash.html is located and run: 
```
python -m SimpleHTTPServer
```
#### Python 3.x
Go to the directory were npDash.html is located and run: 
```
python -m http-server
```
#### Node.js
Install the http-server package using npm:
```
npm install http-server -g
```
Go to the directory were npDash.html is located and run: 
```
http-server
```
