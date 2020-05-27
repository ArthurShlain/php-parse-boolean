# php-parse-boolean
Parse any scalar value to boolean

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
BooleanHelper::anyValueToBoolean('a', false, ['a'], ['b']);`

// true


`
BooleanHelper::anyValueToBoolean('b', false, ['a'], ['b']);`

// false

