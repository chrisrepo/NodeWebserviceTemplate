# NodeWebserviceTemplate
Template for a node rest web service

## How to use
1. Have node.js and mongodb installed
2. Copy this project to a local directory
3. Open 3 command prompts

With the first command prompt, start your mongodb server instance  
Mac:  
```$ mongod```
Windows:  
```$ mongod.exe```

With the next command prompt, start your node service (make sure you're cd'd to the directory with index.js)  
```$ node index.js```

With the last command prompt, test the service with this statement
(note that curl commands aren't built into windows machines so extra work may be necessary to get them)   
```curl -H "Content-Type: application/json" -X POST -d '{"tile":"Hello World"}' http://localhost:3000/items```  

This will insert a value into the mongo db under a collection called "items". You can add more test values if you'd like. The results will be displayed at this localhosted webpage: http://localhost:3000/items
