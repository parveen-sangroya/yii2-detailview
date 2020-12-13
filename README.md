yii-detailview
==============
Enhanced the DetailView widget of yii2 framework using bootstrap classes

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist sangroya/yii2-detailview "*"
```

or add

```
"sangroya/yii2-detailview": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?=  echo \sangroya\DetailView::widget([
*     'model' => $model,
*     'attributes' => [
          ['group'=>true,'label'=>'Personal Detail']
*         'title',               // title attribute (in plain text)
*         'description:html',    // description attribute in HTML
*         [                      // the owner name of the model
*             'label' => 'Owner',
*             'value' => $model->owner->name,
*         ],
*         'created_at:datetime', // creation date formatted as datetime
*     ],
        'header'=>false //by default it's true and set the header on the top
* ]); ?>```
