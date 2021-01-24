## My Voucher store

### Tests

### testing via CURL

#### CRUD
##### Create
add client
```bash
curl -X POST http://localhost:9999/api/clients -H 'content-type: application/json' -d '{"firstname": "Michał", "lastname": "Kanclerz", "address": {"street": "rakowicka", "zip": "31-222", "city": "krakow"}}'
```

##### Read
get single client
```bash
curl http://localhost:9999/api/clients/3 
```

get list
```bash
curl http://localhost:9999/api/clients 
```

##### Update
update by id
```bash
curl -X POST http://localhost:9999/api/clients/4 -H 'content-type: application/json' -d '{"firstname": "Michał", "lastname": "Brzeczyszczykiewicz", "address": {"street": "nibylandia", "zip": "31-222", "city": "whatever"}}'
```
##### Delete
delete by id
```bash
curl -X DELETE http://localhost:9999/api/clients/1 
```


