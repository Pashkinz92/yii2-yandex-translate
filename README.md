Translate content using YandexTranslateAPI
==========================================
Translate content using YandexTranslateAPI

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist pashkinz92/yii2-yandex-translate "*"
```

or add

```
"pashkinz92/yii2-yandex-translate": "*"
```

to the require section of your `composer.json` file.


Usage
-----

```
    'components' => [
         ...
         'translate' => [
             'class' => \pashkinz92\yii2-yandex-translate\Translation::className(),
             'key' => 'yandexTranslateApiKey',
         ],
         ...
     ]
```

Once the extension is installed, simply use it in your code by  :

```
 
     $lang =  Yii::$app->translate->detect('Hello !');
     echo '<pre>';
     var_dump($lang);
     echo '</pre>';
```