# pspsqltimetemporaldata
```
update zones set name = $1, geometry = $2
where zone_id = $3 and updated_at < $4
```
