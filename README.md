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

## 3. PostgreSQL: Time and Temporal Data
### 2 Range Types
```
select numrange(1,10,'[]');
select numrange '(1,)';
select daterange '[today,infinity)';
```
## 8. Managing Time Related Configuration
### 2 Configuration Options
```
database = alter database
role = alter role
session = ser/show pg_settings
transaction = set local
```
```
set time zone value
set timezone = value
```

Settings
```
TimeZone
DateStyle
IntervalStyle
lc_time
timezone_abbreviations
log_timezone
```
#### 04:27
```
set datastyle = sql.dmy;
```
### 4 IANA Time Zone Database
#### 00:52
```
select * from pg_timezone_names;
```
update time zone definitions
```
--with-system-tzdata
--with-system-tzdata=/usr/share/zoneinfo
```
