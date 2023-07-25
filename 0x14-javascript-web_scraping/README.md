0x14. JavaScript - Web scraping
General
JavaScript programming
SON data
Request and fetch API
Read and write a file using fs module
Environment
OS: ubuntu

IDE: Vim, VS Code

Language: JavaScript

Style guidelines: semistandard Airbnb style

Node.js

Shebang: #!/usr/bin/node

Star Wars api: swapi-api.hbtn.io

install Node 10
$ curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
$ sudo apt-get install -y nodejs
Install semi-standard
$ sudo npm install semistandard --global
Install request module and use it
$ sudo npm install request --global
$ export NODE_PATH=/usr/lib/node_modules
Run the code
reading file and parsing it with Node.js

ralex@ralex-nb:$ cat cisfun
C is super fun!
ralex@ralex-nb:$ ./0-readme.js cisfun
C is super fun!

ralex@ralex-nb:$ ./0-readme.js doesntexist
{ [Error: ENOENT: no such file or directory, open 'doesntexist']
  errno: -2,
  code: 'ENOENT',
  syscall: 'open',
  path: 'doesntexist' }
ralex@ralex-nb:$
write to a file

ralex@ralex-nb:$ ./1-writeme.js my_file.txt "Python is cool"
ralex@ralex-nb:$ cat my_file.txt ; echo ""
Python is cool
ralex@ralex-nb:$
status code of a GET request

ralex@ralex-nb:$ ./2-statuscode.js https://www.xelar.tech
code: 200
ralex@ralex-nb:$ ./2-statuscode.js https://www.xelar.tech/doesntexist
code: 404
ralex@ralex-nb:$
Author:Mesele A.
