# Chat example with websockets in go - from gobwas
# These are the examples from gobwas/ws - only fixed
- removed the git sub-repositories and replaced them with packages and go modules
- fixed errors in the javascript part to allow using version 2.0 of mithril js. The original example is downloading the 
  library from the site directly. Now it points to the 2.0 version.
- removed the Makefile

# Running
- in one terminal:
  ```
  cd src/chat
  go run .
  ```
- in another terminal
  ```
  cd src/proxy && go build && cd ../..
  ./src/proxy/proxy 
  ```
- with the browser load http://localhost:8888/

The original README can be found at https://github.com/gobwas/ws-examples
