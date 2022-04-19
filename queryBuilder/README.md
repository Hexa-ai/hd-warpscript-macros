# Query builder

This library simplifies the use of several GTS Warp10 as a table of a SQL base.

## Prerequisite

Each GTS represents a column of the table. In order for the GTS records to be considered as the row of a table, the timestamps must be aligned.

## Example

```

$rangeDtStart $rangeDtEnd '~mA.Code|mA.Evenement|mA.ModeDeMarche' $readToken @queryBuilder/select

'mA.Evenement' 1 '==' @queryBuilder/where 
'mA.ModeDeMarche' 6 '==' @queryBuilder/andWhere 
'mA.Code' '%27055F%27' '==' @queryBuilder/andWhere
@queryBuilder/all
```

## Functions currently available

* @queryBuilder/select
* @queryBuilder/where
* @queryBuilder/andWhere
* @queryBuilder/orWhere
* @queryBuilder/and
* @queryBuilder/or
* @queryBuilder/all
* @queryBuilder/count



