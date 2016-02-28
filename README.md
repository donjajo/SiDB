# php_DB
Simple PHP MySQL Database Framework

**SyDB** is a Simple PHP MySQL Database framework with ease of use

## Using SyDB
Include **db.Class.php** to your project and set database details in $db_data object in line 10 to 15
```php
// Load database data
self::$db_data = array(
	'host' => 'localhost',
	'user' => 'root',
	'password' => '',
	'name' => ''
	);
 ```
 ###Inserting Data
 Using the `insert()` method which accepts 2 arguments and returns the last insert ID
- Table name
- Arrays of values to insert with column name as keys
```php
Db::insert( 'table', array( 'column1' => 'value1', 'column2' => 'value2' ) );
```

### Updating Data
```php
Db::update( 'table', array( 'column1' => 'new_value', 'column2' => 'new_value' ), array( 'column3' => 'value' ) );
```
This accepts 3 arguments:
- Table name
- Array of columns to modify
- Array of columns to match

### Deleting Data
```php
Db::delete( 'table', array( 'column' => 'value' ) );
```
This deletes from table where `column` = `value`


