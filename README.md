# pspsqltimetemporaldata
```
update zones set name = $1, geometry = $2
where zone_id = $3 and updated_at < $4
```
Avoid Client Time
```
select * from zones
where updated_at < now();
select now();
```


## 8. Managing Time Related Configuration
### 2 Configuration Options
