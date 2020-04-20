This is an example plugin repository that references all example plugins.

Adding the following to your orca.yml config will load and start the latest RandomWaitPlugin example plugin during app startup.
```
spinnaker:
  extensibility:
    plugins:
      Armory.RandomWaitPlugin:
        enabled: true
        extensions:
          armory.randomWaitStage:
            enabled: true
            config:
              defaultMaxWaitTime: 60
    repositories:
      example-repo:
        url: https://raw.githubusercontent.com/spinnaker-plugin-examples/examplePluginRepository/master/repositories.json
```
