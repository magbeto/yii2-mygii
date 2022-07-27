Yii2 Gii model plus base model
=====================

This generator generates two ActiveRecord class for the specified database table. An empty one you can extend and a Base one which is the same as the original model generator.

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

run

```
php composer require magbeto/yii2-mygii
```

## Usage

```php
//Add this into common/config/main-local.php
    'bootstrap' => 'gii',
    'modules' => [
        'gii' => [
            'class' => 'yii\gii\Module',
            'generators' => [
                'doubleModel' => [
                    'class' => 'magbeto\mygii\generators\model\Generator',
                ],
            ],
        ],
    ],
```
