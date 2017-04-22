# Translating in Magento 2

## Template Translations

[http://devdocs.magento.com/guides/v2.0/frontend-dev-guide/translations/translate\_theory.html](http://devdocs.magento.com/guides/v2.0/frontend-dev-guide/translations/translate_theory.html "Official Documentation")

##### **Regular Translation**

```phtml
<h3><?php echo __('Really Interesting Title') ?></h3>
```

##### Translation with Variable

```phtml
 <h3><?php echo sprintf(__('¿Que pasa %s?'), $user_firstname) ?></h3>
```

## Javascript Translations

Use `$.mage.__('Reschedule')` when translating strings in Javascript.

###### EXAMPLE

```js
alerter({
    title: $.mage.__('Reschedule'),
    content: form,
    buttons: [],
});
```



