<h1 align="center">HolbertonBnB V2.0</h1>
<p align="center">An AirBnB clone.</p>

<p align="center">
  <img src="https://github.com/adonis7ejeda/AirBnB_clone_v2/blob/master/assets/hbnb_logo.png"
	    alt="HolbertonBnB logo">
</p>


[![lisence](https://img.shields.io/github/license/adonis7ejeda/AirBnB_clone_v2?style=plastic)](https://github.com/adonis7ejeda/AirBnB_clone_v2/blob/master/LICENSE)
[![Twitter Adonis](https://img.shields.io/twitter/follow/Adonis7ejeda?label=AdonisTejeda&style=social)](https://twitter.com/Adonis7ejeda)
[![Twitter Carlos](https://img.shields.io/twitter/follow/cbarros27?label=CarlosBarros&style=social)](https://twitter.com/cbarros27)


## Description :house:

In this project we learned how to build a database engine with the SQLAlchemy Python library. 

<p align="center">
  <img src="https://github.com/adonis7ejeda/AirBnB_clone_v2/blob/master/assets/hbnb_step2.png"
	    alt="HolbertonBnB logo">
</p>


### Classes :cl:

HolbertonBnB supports the following classes:

* BaseModel
* User
* State
* City
* Amenity
* Place
* Review

## Storage :baggage_claim:

The above classes are handled by one of either two abstracted storage engines,
depending on the call - [FileStorage](./models/engine/file_storage.py) or
[DBStorage](./models/engine/db_storage.py).

### FileStorage

The default mode.

In `FileStorage` mode, every time the backend is initialized, HolbertonBnB
instantiates an instance of `FileStorage` called `storage`. The `storage`
object is loaded/re-loaded from any class instances stored in the JSON file
`file.json`. As class instances are created, updated, or deleted, the
`storage` object is used to register corresponding changes in the `file.json`.

### DBStorage

Run by setting the environmental variables `HBNB_TYPE_STORAGE=db`.

In `DBStorage` mode, every time the backend is initialized, HolbertonBnB
instantiates an instance of `DBStorage` called `storage`. The `storage` object
is loaded/re-loaded from the MySQL database specified in the environmental variable
`HBNB_MYSQL_DB`, using the user `HBNB_MYSQL_USER`, password `HBNB_MYSQL_PWD`, and
host `HBNB_MYSQL_HOST`. As class instances are created, updated, or deleted, the
`storage` object is used to register changes in the corresponding MySQL database.
Connection and querying is achieved using SQLAlchemy.

## Testing :straight_ruler:

Unittests for the HolbertonBnB project are defined in the [tests](./tests)
folder. To run the entire test suite simultaneously, execute the following command:

```
$ python3 unittest -m discover tests
```

Alternatively, you can specify a single test file to run at a time:

```
$ python3 unittest -m tests/test_console.py
```

## Authors :black_nib:
* **Ashley Baker,** 
* **kah tchek mekapeu d'avilla** <[mekapeu](https://github.com/mekapeu)>