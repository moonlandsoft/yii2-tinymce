moonlandsoft/yii2-tinymce
=========================
The TinyMCE Extension for yii framework

[![Latest Stable Version](https://poser.pugx.org/moonlandsoft/yii2-tinymce/v/stable)](https://packagist.org/packages/moonlandsoft/yii2-tinymce) [![Total Downloads](https://poser.pugx.org/moonlandsoft/yii2-tinymce/downloads)](https://packagist.org/packages/moonlandsoft/yii2-tinymce) [![Latest Unstable Version](https://poser.pugx.org/moonlandsoft/yii2-tinymce/v/unstable)](https://packagist.org/packages/moonlandsoft/yii2-tinymce) [![License](https://poser.pugx.org/moonlandsoft/yii2-tinymce/license)](https://packagist.org/packages/moonlandsoft/yii2-tinymce)

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist moonlandsoft/yii2-tinymce "*"
```

or add

```
"moonlandsoft/yii2-tinymce": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
use moonland\tinymce\TinyMCE;

echo TinyMCE::widget(['name' => 'text-content']);

$form->field($model, 'attribute')->widget(TinyMCE::className());

//toggle to tinyMCE or to textarea

echo TinyMCE::widget(['name' => 'text-content', 'toggle' => ['active' => true]]);

$form->field($model, 'attribute')->widget(TinyMCE::className(), [
	'toggle' => [
		'active' => true,
	]
]);
```
