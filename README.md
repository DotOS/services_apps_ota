# Documentation
# DEPRECATED
## Moved to https://github.com/DotOS/official_devices
### json example :

```
{
  "response":[
    {
      "datetime":1612459475,
      "filename":"dotOS-R-v5.0.0-davinci-OFFICIAL-20210204-1724.zip",
      "id":"817af9b5b8eab6151c22456634c24dfe",
      "romtype":"OFFICIAL",
      "size":1666374431,
      "url":"https://url/update.zip",
      "version":"v5.0.0",
      "changelog":[
        {
          "miscTitle":"",       (Can be left empty)
          "miscSummary":"", 
          "settingsTitle":"",   (Can be left emtpy)
          "settingsSummary":"",
          "securityTitle":"",   (Can be left emtpy)
          "securitySummary":"",
          "systemTitle":"",     (Can be left emtpy)
          "systemSummary":""
        }
      ]
    }
  ]
}
```

## Conditions
* Changelog summary for each category should **NOT** be left empty if it has a title
    * **Example**
     ```
     "miscTitle":"Test Title",
     "miscSummary":"",
     ```
     
* If you don't have any changes for a category, just leave both entries empty
* For the ID entry it's recommended to be used the md5 hash generated after a successful build
* Use the datetime timestamp that is generated after a successful build
