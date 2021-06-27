# PHP MySQLi Base

![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCJNpJE0aWgc1jV1Edz93pmA?style=social)
![GitHub followers](https://img.shields.io/github/followers/awanz?style=social)
[![Chat on Telegram](https://img.shields.io/badge/Chat%20on-Telegram-brightgreen.svg)](https://t.me/awangram)  

## About

PHP Mysqli Base is My library code for make a easy i code php to connect mysql with mysqli.

## Specification

Use PHP version 8 for better deployment.

## Installation

1. Clone This Project
2. You can include file mysqlibase.php to your code with

`include_once('mysqlibase.php');`

3. You can use that!

## Example Code

If you want use this library, first you must make object with example code this.

`$db = new MySQLBase($dbhost, $dbname, $dbuser, $dbpass);`

After you init object you can use with code

`$result = $db->getAll("table_name");`

## Example Fetch Data

> **$result->fetch_all()**

```
Array
(
    [0] => Array
        (
            [0] => Threads_connected
            [1] => 1
        )

)
```
> **$result->fetch_assoc()**
```
Array
(
    [Variable_name] => Threads_connected
    [Value] => 1
)
```
> **$result->fetch_array()**
```
Array
(
    [0] => Threads_connected
    [Variable_name] => Threads_connected
    [1] => 1
    [Value] => 1
)
```
> **$result->fetch_field()**
```
stdClass Object
(
    [name] => Variable_name
    [orgname] => VARIABLE_NAME
    [table] => SESSION_STATUS
    [orgtable] => SESSION_STATUS
    [def] => 
    [db] => information_schema
    [catalog] => def
    [max_length] => 17
    [length] => 256
    [charsetnr] => 45
    [flags] => 1
    [type] => 253
    [decimals] => 0
)
```
> **$result->fetch_field_direct(1)**
```
stdClass Object
(
    [name] => Value
    [orgname] => VARIABLE_VALUE
    [table] => SESSION_STATUS
    [orgtable] => SESSION_STATUS
    [def] => 
    [db] => information_schema
    [catalog] => def
    [max_length] => 1
    [length] => 8192
    [charsetnr] => 45
    [flags] => 1
    [type] => 253
    [decimals] => 0
)
```
> **$result->fetch_fields()**
```
Array
(
    [0] => stdClass Object
        (
            [name] => Variable_name
            [orgname] => VARIABLE_NAME
            [table] => SESSION_STATUS
            [orgtable] => SESSION_STATUS
            [def] => 
            [db] => information_schema
            [catalog] => def
            [max_length] => 17
            [length] => 256
            [charsetnr] => 45
            [flags] => 1
            [type] => 253
            [decimals] => 0
        )

    [1] => stdClass Object
        (
            [name] => Value
            [orgname] => VARIABLE_VALUE
            [table] => SESSION_STATUS
            [orgtable] => SESSION_STATUS
            [def] => 
            [db] => information_schema
            [catalog] => def
            [max_length] => 1
            [length] => 8192
            [charsetnr] => 45
            [flags] => 1
            [type] => 253
            [decimals] => 0
        )
)
```
> **$result->fetch_row()**
```
Array
(
    [0] => Threads_connected
    [1] => 1
)
```
> **$result->fetch_object()**
```
stdClass Object
(
    [Variable_name] => Threads_connected
    [Value] => 1
)
```


## Contribution

Awan

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).