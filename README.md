# contextos-registry

Plugin registry for [ContextOS](https://github.com/guilhermefmotta/ContextOS).

## Add a plugin

Submit a PR adding your entry to `registry.json`.

### Schema

```json
{
  "id": "mcp-yourplugin",
  "name": "Your Plugin",
  "pluginType": "mcp",
  "description": "One sentence.",
  "author": "you",
  "official": false,
  "icon": "🔧",
  "tags": ["tag1", "tag2"],
  "install": {
    "installType": "npx",
    "command": "npx",
    "args": ["-y", "your-mcp-package"],
    "requiredEnv": ["YOUR_API_KEY"]
  }
}
```

`pluginType`: `"mcp"` | `"skill"` | `"agent"`

`installType`: `"npx"` | `"uvx"` | `"binary"`
