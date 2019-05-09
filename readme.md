# Cache Management API

With help of artifacts present in this repository, we can manage (Get/Create/Update/Delete) the API Gateway default and custom caches content. Here is the list of operations supported by API :

![Available API Methods]( https://github.com/Axway-API-Management-Plus/master/cache-management/src/lib/images/APIMethods.PNG )

Response of GET /caches and GET /caches/{name} also list number of cached entities in caches

**Usage:** 

1. Import *cache-management.xml* in policy studio project.
2. Add all 3 policies of container "Cache Management" as routing policies in Policy Studio --> Server Settings --> API Manager --> Routing Policies
3. Deploy the configuration
4. Import *cache-management-api-export.dat* in API Manager.  //password is changeme
5. Test the endpoints, you can use postman collection *Cache-Management.postman_collection.json*

**Warning :** Internal caches contain data such as HTTP session information and irresponsible cache manipulation may lead to unpexted failures. So be careful!!
