# npDash

## Requirements
npDash.html and assembly.json need to be in the same directory to operate.

## npDash in Firefox
npDash can be run locally from Firefox:

- Open npDash.html via the browser.  

## npDash in Chrome ( and other webkit browsers?)
Chrome disables loading of local files (assembly.json) for security reasons.
One option to get around this is to start chrome with the "--allow-file-access-from-files" flags but poses a security risk.
Another option is to host a local-server using node.js or python as follows:

- **Option 1**: Python 2.x
    Go to the directory were npDash.html is located and run: 
    ```
    python -m SimpleHTTPServer
    ```
    **Notes**: Using the Python servers may require the use of browser hard refreshes (ctrl+F5) to clear the cache. This is generally not required for non-development purposes.

-  **Option 2**: Python 3.x
    Go to the directory were npDash.html is located and run: 
    ```
    python -m http-server
    ```
    **Notes**: Using the Python servers may require the use of browser hard refreshes (ctrl+F5) to clear the cache. This is generally not required for non-development purposes.

-  **Option 3**: Node.js (Preferred)
    
    This method is preferred due to the extra arguments that can be passed to control server behaviour.

    Install the http-server package using npm:
    ```
    npm install http-server -g
    ```
    Go to the directory were npDash.html is located and run: 
    ```
    http-server -c-1
    ```

    The -c-1 flag tells the localhost server to not cache files.
