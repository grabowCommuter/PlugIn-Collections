
##How to create a Collection of PlugIns?

###Collections

You can define your own collection of PlugIns, e.g. "The top-ten for California". A collection of PlugIns is just a simple list of PlugIns. Each PlugIn is identified by its `moduleId`-value, e.g. `grabowCommuter/Speedometer`. (The `moduleId` is always equal to the fullname of the gitHub-repro. For more information about PlugIns look [here](https://github.com/grabowCommuter/PlugIn-Developer)).

### Create a collection

To create a collection, you have to define a JSON-Array according to the following structure:
`[ { "modueId": "<fullname of repro>" }, ... }`

An example of an collection:
   
       [
            	{ "moduleId":"grabowCommuter/Speedometer" },
            	{ "moduleId":"grabowCommuter/Speedometer2" },
            	{ "moduleId":"grabowCommuter/GoogleSatView" }
       ]

###Publish a collection

To publish a collection of PlugIns the following steps must be executed:

1. Create a new repository on github.

2. Put the string `(com.grabow.commuter.collection)` somewhere into the description of the repro. ACom will search for repros containing this string in the description. 

3. Save the collection in the master-branch of your repro under the name `collection.js`. Check the path to your Collection-file - it should be similar to the following example: `https://raw.githubusercontent.com/grabowCommuter/TestCollection/master/collection.js`

5. Your done.

----
####Hint: 
- If you search and load the collection via ACom, be aware that it takes some time (minutes) until the repro is published or updated on github.
- Android does cache downloaded files. If you reload your (even modified) collection, Android might take the cached version. To check, which version is loaded select the „Edit PlugIn“ button and check the content.
- Use the `README.md` file to explain what your collection is good for and for which region it is best suited for (e.g. USA, Asia, Europe, Germany, etc.). 
- Use the repro description to explain your collection in short. Only the first 120 characters of the description will be shown in ACom. Don't forget to add the string `(com.grabow.commuter.collection)`.


----




> Written with [StackEdit](https://stackedit.io/).