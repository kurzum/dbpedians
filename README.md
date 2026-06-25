# DBpedians

In development at https://kurzum.github.io/dbpedians/ later moved to https://dbpedians.dbpedia.org

The KG about DBpedians (people and orgs)

### What this github project does

## Join dbpedians.dbpedia.org - basics
1. Get your DBpedia-normalized person URI
DBpedia mints a normalized DBpedian URI using the DBpedia keycloak account name as a stable local slug, following the pattern `https://dbpedians.dbpedia.org/id/${keycloak-name}#me` .
Normally, this is the login of your keycloak. This should also be the username of the forum and other things. 
2. Create your own FOAF profile. Doing so on github.io works, but it can also be any file on any server. See below for more guidance on the FOAF profile and requirements.  
3. Add the owl:sameAs link to the DBpedian URI to your ID in the FOAF profile. Example:    
```
   "@id": "https://kurzum.github.io/profile.jsonld#me",
   "owl:sameAs": "https://dbpedians.dbpedia.org/id/kurzum#me",
``` 
4. Add your URL to the list for crawling   

## Guidelines for FOAF profile
1. Json-LD, Turtle
2. required triples
3. parsing
4. links 
5. limits 

## TODO
* dbpedians.dbpedia.org.  CNAME  dbpedia.github.io.
* enable https
