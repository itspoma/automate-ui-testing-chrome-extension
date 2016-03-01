# Notes

match: https://www.google.com.ua/
```
page.contains('input[name=q]');
page.not.contains('button[type=submit]');
page.contains('Україна');

$('input[name=q]').val('test');
$('input[type=submit][name=btnK]').click();
page.redirectTo(['search', '&q=aaa']);
```

output:
```
contains element "input[name=q]" PASS
not contains element "button[type=submit]" PASS
contains text "Україна" PASS
redirectTo "search" PASS
redirectTo "&q=aaa" PASS
```
