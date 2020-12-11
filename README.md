# php-parse-boolean
Parse any scalar value to boolean. Useful when you need to parse boolean columns of spreadsheet file.

## Usage

```php
BooleanHelper::anyValueToBoolean(0);
// false
```

```php
BooleanHelper::anyValueToBoolean(1);
// true
```

```php
BooleanHelper::anyValueToBoolean('-');
// false
```


```php
BooleanHelper::anyValueToBoolean('+');
// true
```


```php
BooleanHelper::anyValueToBoolean('imNotInRules', 'default');
// 'default'
```

```php
$positives = ['positive', 'plus'];
$negatives = ['negative', 'minus'];
BooleanHelper::anyValueToBoolean('positive', false, $positives, $negatives);
// true
```


```php
$positives = ['positive', 'plus'];
$negatives = ['negative', 'minus'];
BooleanHelper::anyValueToBoolean('minus', false, $positives, $negatives);
// false
```


