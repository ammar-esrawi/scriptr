# Project Title
firebase client for scriptr platform

## Current implementation 

Real Time Database

# Getting started
```
var fbModule = require('./newFirebase/Firebase');

var fb=new fbModule.Firebase();
var dbMngr=fb.getDatabaseManager();
var myDb=dbMngr.db("dbName");
var doc=myDb.doc("path.to.document");//the dot represents a level in the json tree

var x=doc.get();
```
# Configuration
```
//The Project Info ,not used in current version
const project={
    name:"Project Name",//not used for now but it will help you distinguish your apps
    type: "service_account",//not used for now
  	project_id: "projectID"//your project id in firepase
};

const access_token="YourToken";

//The database needed data to build the data Uris
const database={
    deafultDatabase:"deafultDB",
    endPointPrefix:"https://",
    endPointSuffix:".firebaseio.com"
    
};

//errors list dont modify
const errorCodeList = {
    "missingParameter" : "MISSING_PARAMETER",
    "invalidAction": "INVALID_ACTION",
    "notFound": "ENTITY_NOT_FOUND"
};
```






