#Separated Pager for Yii2

Yii2 LinkPager displays a few pages before and after the current page and first and last pages

![sample](https://raw.githubusercontent.com/maddog043/files/master/separatedpager/separatedpager.png)

##Installation

###Install the extension

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist maddog043/yii2-separatedpager "*"
```

or add

```
"maddog043/yii2-separatedpager": "*"
```

to the require section of your `composer.json` file.

##Usage

Simply add the `LinkPager` to page

```php
use maddog043\separatedpager\LinkPager;

...

LinkPager::widget([
    'pagination' => $pages,
    'maxButtonCount' => 1,
]);
```

`$pages` is yii\data\Pagination

`maxButtonCount` is count button before and after the current page

`separator` is separator for pages

`separatorClass` is class for separator symbol
