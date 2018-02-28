
extcats: tools to organize and query astronomical catalogs
==================================================================

This modules provides classes to import astronomical catalogs into 
a mongo noSql database, and to query this database for positional 
matches.

The preferred way to install the package is to download the tar 
from this Github page, unpack it in your favourite place, and 
run python setup.py install. This will also download some test
data to run the example notebooks. 

Alternatively, the pure python pacakge (witout examples) should be 
installable via pip.

The two main classes are:

    - CatalogPusher: will process the raw files with the catalog sources
    and creates a database.
    
    - CatalogQuery: will perform queries on the catalogs.

See examples and explanations in the notebook folder.

In order to run this tool, you require a local mongo daemon to be running. MongoDb is a database software, and can be found at https://www.mongodb.com/download-center#production, or installed via Homebrew for Mac users (e.g https://treehouse.github.io/installation-guides/mac/mongo-mac.html).

Once you have installed Mongo, you can start a Mongo Daemon by entering the command "mongod" in a terminal. Once this step is complete, the extcats packages can then be run.
