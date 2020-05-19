To reproduce:
```
composer install
vendor/bin/phpunit tests/BarTest.php
vendor/bin/phpunit tests/FooTest.php
```

Output of `vendor/bin/phpunit tests/BarTest.php`:

```
PHPUnit 9.1.4 by Sebastian Bergmann and contributors.

.                                                                   1 / 1 (100%)

Time: 00:00.024, Memory: 4.00 MB

OK (1 test, 1 assertion)
```

Output of `vendor/bin/phpunit tests/FooTest.php`:

```
PHPUnit 9.1.4 by Sebastian Bergmann and contributors.

W                                                                   1 / 1 (100%)

Time: 00:00.026, Memory: 6.00 MB

There was 1 warning:

1) Warning
No tests found in class "App\Tests\ParentFooTest".

WARNINGS!
Tests: 1, Assertions: 0, Warnings: 1.
```
