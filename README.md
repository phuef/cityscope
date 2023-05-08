# CityIO_Flask

A lightweight version of cityIO for locally testing CityScope tables.

The initial state of the table is established from a local json file. GET, POST and DELETE requests can be made following the main [cityIO](https://cityscope.media.mit.edu/backend/API) structure: 

To run, first install requests, flask, and flask_cors in a clean environment:
```
pip install flask flask_cors
```

Then call cityio_lite.py with the table names as arguments:
```
python cityio_lite.py table_name_1 table_name_2
```

Each table is initialised from the corresponding json file stored in the 'base' directory. Note that the table names must be the same as the json file names, minus the `_base.json` extension.


## Develpment 
For development, you may update the `json` file. You must than restart the server AND the CityScopeJS client, so that the changes are reflected.