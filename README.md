# condition-noop

[Semantic Release](https://github.com/semantic-release/semantic-release) uses [condition-travis](https://github.com/semantic-release/condition-travis) as its default plugin, making it seemingly impossible to run on any other CI (unless using a custom plugin for that CI).

Bizarre but true.

This plugin can be used to disable "verify-conditions" altogether:

**package.json**
```json
{
  "release": {
    "verifyConditions": "condition-noop"
  }
}
```

## License
MIT
