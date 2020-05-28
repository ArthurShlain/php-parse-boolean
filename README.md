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
BooleanHelper::anyValueToBoolean('positive', false, ['positive', 'plus'], ['negative', 'minus']);`

// true


`
BooleanHelper::anyValueToBoolean('minus', false, ['positive', 'plus'], ['negative', 'minus']);`

// false

