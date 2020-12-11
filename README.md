# php-parse-boolean
Parse any scalar value to boolean. Useful when you need to parse boolean columns of spreadsheet file.

Just copy `anyValueToBoolean` function to your Helpers class

## Usage

`
BooleanHelper::anyValueToBoolean(0);`

// false


`
BooleanHelper::anyValueToBoolean(1);`

// true


`
BooleanHelper::anyValueToBoolean('-');`

// false


`
BooleanHelper::anyValueToBoolean('+');`

// true


`
BooleanHelper::anyValueToBoolean('this string not in rules', 'this is default value');`

// 'this is default value'


`
$positives = ['positive', 'plus'];

$negatives = ['negative', 'minus'];

BooleanHelper::anyValueToBoolean('positive', false, $positives, $negatives);`

// true


`
$positives = ['positive', 'plus'];

$negatives = ['negative', 'minus'];

BooleanHelper::anyValueToBoolean('minus', false, $positives, $negatives);`

// false

