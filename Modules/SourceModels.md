



## Default Magento Admin Source Models

##### Example Path
`app/code/Gil/Mageziner/etc/adminhtml/system.xml`

##### Example field markup

```
 <field id="specificcountry" translate="label" type="multiselect" sortOrder="140" showInDefault="1" showInWebsite="1" showInStore="0">
    <label>Payment From Specific Countries</label>
    <source_model>Magento\Directory\Model\Config\Source\Country</source_model>
</field>
```

### List of Out of Box Source Models

Many of the default Source Models can be found inside ` /vendor/Magento/<module>/Model/Config/Source/`. An example would be 

| Type | Source Model | Description |
| :--- | :--- | :--- |
| select | Magento\Config\Model\Config\Source\Enabledisable | Yes or No Select. Used for enable or disable values. Saved as 0 or 1 in database. |
| select | Magento\Config\Model\Config\Source\Yesnocustom | Same as Yes/No with a  Custom option |
| select | Magento\AdminNotification\Model\Config\Source\Frequency | that is used in notifications and enables us to select frequency \(every 1, 2, 6, 12, 24 hours\) |
| select | Magento\Catalog\Model\Config\Source\TimeFormat | that enables us to set the time format (12h / 24h) |
| select | Magento\Cron\Model\Config\Source\Frequency | that enables us to choose from `Daily/Weekly/Monthly` (in the database it’s saved as D/W/M respectively) |
| select | Magento\GoogleAdwords\Model\Config\Source\Language | that enables saving a 2-letter code of a given language in the ISO 639-1 format \(e.g. en\) |
| select | Magento\Config\Model\Config\Source\Locale | that acts similarly to the above one, but it pertains a locale code \(e.g. en\_US\) |
| allowspecific | Magento\Payment\Model\Config\Source\Allspecificcountries | List of Countries |
| multiselect | Magento\Directory\Model\Config\Source\Country | List all countries and select applicable ones | 
| obscure | Magento\Config\Model\Config\Backend\Encrypted | Saved value is show with *. Useful for API keys or Passwords. Encrypted on backend |
| text | n/a | Simple text field entry. No source model needed.
| multiselect | Magento\Customer\Model\Config\Source\Group | Select customer groups
