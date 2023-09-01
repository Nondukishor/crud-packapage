## Requirements
    Laravel >=8.0.0
    PHP >= 7.4.0
## Installation
```
composer require nipu/curdpackage --dev
```
# after install run this command
```
php artisan vendor:publish --provider="Nipu\CurdPackage\CrudGeneratorServiceProvider"
```

And since, we're using laravelcollective/html as dependency you should add its service provider in the config/app.php file. 
check docs
https://laravelcollective.com/docs

```
'providers' => [

    Collective\Html\HtmlServiceProvider::class,
],

'aliases' => [
    'Form' => Collective\Html\FormFacade::class,
    'HTML' => Collective\Html\HtmlFacade::class,
],
```
