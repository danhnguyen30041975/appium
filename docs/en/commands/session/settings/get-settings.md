# Retrieve Device Settings

Retrieve the current settings on the device
## Example Usage

```java
// Java
Map<String, Object> settings = driver.getSettings();

```

```python
# Not supported
```

```javascript
// Javascript
// webdriver.io example
let settings = driver.settings();



// wd example
await driver.settings();

```

```ruby
# Not supported
```

```php
// Not supported
```

```csharp
// Not supported
```



## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients

|Language|Support|Documentation|
|--------|-------|-------------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |  [appium.github.io](http://appium.github.io/java-client/io/appium/java_client/HasSettings.html#getSettings--)  |
|[Python](https://github.com/appium/python-client/releases/latest)| None |  |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |  [webdriver.io](http://webdriver.io/api/mobile/settings.html)  |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |  [github.com](https://github.com/admc/wd/blob/master/lib/commands.js#L3018)  |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| None |  |
|[PHP](https://github.com/appium/php-client/releases/latest)| None |  |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| None |  |

## HTTP API Specifications

### Endpoint

`GET /wd/hub/session/:session_id/appium/settings`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|

### JSON Parameters

None

### Response

a JSON hash of all the currently specified settings, see [Settings API](/docs/en/advanced-concepts/settings.md). (`array<object>`)

## See Also

* [JSONWP Specification](https://github.com/appium/appium-base-driver/blob/master/lib/mjsonwp/routes.js#L454)