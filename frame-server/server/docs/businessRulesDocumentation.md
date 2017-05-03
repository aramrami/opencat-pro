<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [businessRules](#businessrules)
    -   [setProfileVariables](#setprofilevariables)
    -   [getDemographicFilterQuery](#getdemographicfilterquery)
    -   [constructAvailableSectionArray](#constructavailablesectionarray)

## businessRules

Transform user demographic data to rules hash. Must be custom-defined for each project

### setProfileVariables

This function constructs a json object which consists of profile data.
Must be custom defined for each project.

**Parameters**

-   `server`  
-   `userid`  
-   `callback`  

Returns **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** The profile data object.

### getDemographicFilterQuery

This function constructs a match query to be supplied to mongo.
This will be used to filter questions relevant to the user's demographics.
Must be custom defined for each project.

**Parameters**

-   `server`  
-   `userid`  
-   `surveyId`  
-   `callback`  

Returns **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** The demographic filter query.

### constructAvailableSectionArray

This function constructs an array of relevant sections to be included in the survey.
This is based on the user's demographics.
Must be custom defined for each project.

**Parameters**

-   `server`  
-   `userData`  
-   `callback`  

Returns **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)>** The array of sections for that user.