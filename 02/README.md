# Default of Arr::get()

```php
$result['amount'] = 0;
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = '0';
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = null;
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = ' ';
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = 1;
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = -1;
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = '-1';
echo Arr::get($result, 'amount', 'a') . "\n";

$result['amount'] = 0.2;
echo Arr::get($result, 'amount', 'a') . "\n";
```

## Result
```
0
0

 
1
-1
-1
0.2
```
