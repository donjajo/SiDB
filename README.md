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
 Using the insert() method which accepts 2 arguments, 
 	* The table name
    * Array of values and column names as keys