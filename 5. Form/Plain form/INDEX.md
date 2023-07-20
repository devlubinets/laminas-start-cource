# Plain form

Add simple form with url helper in your template for view (example.phtml)

Get url for action
```php
<?php $url = $this->url(Module::ROUTE_NAME_MODULE . '/' . Module::ROUTE_NAME_ACTIONS,['action' => 'doExample',]); ?>
```

Example of form
```html
<form action="<?php echo $url; ?>" method="POST">
    <!--For the first step-->
    <div>
        <label for="name">Enter your name: </label>
        <input type="text" name="name" id="name" required>
    </div>
    <!--For the second step-->
    <div>
        <label for="email">Enter your email: </label>
        <input type="email" name="email" id="email" required>
    </div>
    <div>
        <input type="submit" value="Apply!">
    </div>
</form>
```