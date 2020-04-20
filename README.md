This is an example plugin repository that references all example plugins.

Adding the following to your orca.yml config will load and start the latest RandomWaitPlugin example plugin during app startup.
```
spinnaker:
  extensibility:
    plugins:
      Armory.DatadogEventListener:
        enabled: true
        extensions:
          armory.dataDogEventListener:
            enabled: true
            config:
              apiKey: 'key'
    repositories:
      example-repo:
        url: https://raw.githubusercontent.com/armory-plugins/pluginRepository/master/repositories.json
```
