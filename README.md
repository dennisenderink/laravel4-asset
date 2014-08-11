A port of Laravel 3's Asset class. Made to work with Laravel 4.


## Usage

### Composer Side

add `"dennisenderink/asset": "dev-master"` to the `require` section of your `composer.json` so that it should look something the code below.

```composer
...
...
...
"require": {
	...
	...
	...
	"dennisenderink/asset": "dev-master"
},
...
...
...
```

### Laravel Side

add the following code to the `providers` section of the `app/config/app.php` file

```php
'Dennisenderink\Asset\AssetServiceProvider',
```

so that it'll look something like the following

```php
'providers' => array(

	...
	...
	...
	'Dennisenderink\Asset\AssetServiceProvider',

),
```

and add the following code to the `aliases` section of the `app/config/app.php` file

```php
'Asset' => 'Dennisenderink\Asset\Facades\Asset'
```

so that it'll look something like the following

```php
'aliases' => array(

	...
	...
	...
	'Asset'       => 'Dennisenderink\Asset\Facades\Asset',

),
```