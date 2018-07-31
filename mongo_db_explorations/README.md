# Mongo DB
in mongo db equivalent term,
<table>
<th><tr><td>RDBMS</td><td>Mongodb</td></tr></th>
<tr>
<td>database</td>
<td>database</td>
</tr>
<tr>
<td>table</td>
<td>collection</td>
</tr>
<tr>
<td>row</td>
<td>document</td>
</tr>
</table>
## Basic commands in mongo shell
* to show all dbs,
```
show dbs
```
* use or specify a db to use for operations
```
use <dbname>
```
* creating a collection by default and entering a document.
```
db.collection_name.insertOne({ajsonentry:'test entry'})
```
* to get all the documents in collection
```
db.collection_name.find()
```
* to find a specific document
```
db.collection_name.find({ parameter: 'value to search' })
```
* updateone 
```
db.collection_name.updateOne({toupdatename:'value'})
```
* to delete after search
```
db.collection_name.deleteOne({item:'to ensure delete only one match'})
or
db.collection_name.remove({ itemnametosearchfor: 'your search term' })
```
* to delete all (remember to put {}, without {} no item will be deleted)
```
db.collection_name.remove({})
```
