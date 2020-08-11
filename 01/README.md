# boolean of Arr::get()

```php
$result['amount'] = 0;
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = '0';
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = null;
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = ' ';
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = 1;
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = -1;
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = '-1';
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = 0.2;
echo Arr::get($result, 'amount') ? "true\n" : "false\n";

$result['amount'] = [];
echo Arr::get($result, 'amount') ? "true\n" : "false\n";
```

## Result
```
false
false
false
true
true
true
true
true
false
```
