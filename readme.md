Background:Take home exercise about implement and test a coumminication protocal.
It includes two part: Speaker and listner. The key of relative is the speed and timing.
The speaker sending the message in dffernernt way. And Listeners estimate the speed of speech by time to get the correct information.

Installation:(perfer to install in global to avoid permission issue)
To install and test the code please follow the following steps:
npm install
Once all requested modules have been installed digit
npm start
The express application start at: http://localhost:3000/

References:
express
socket.io
socket.io-client

Maintainer: Xiufen Luo

Related Efforts: The attached document

Feature contents:Speaker,Listener
Function: Connection，Broadcast，Time speed Calculate,Translation

Useage:
after all enviroment set up and run
node speaker.js

speaker will be set up to ready to listen the prt 3000
if you received the error message: port 3000 already in use,please run
lsof -i :3000
it will show you the PID(port id)
kill -9 PID
And run node speaker.js

speaker will broadcast the message with default length(only one syllables)
or you can run the amont length for message you want(ex. 100)
node speaker.js 100

open new termnial and run
node listener.js
if connected,The connetion message will display on both side and listener will receive the message from speaker.
