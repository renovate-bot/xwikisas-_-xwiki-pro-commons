# xwiki-macro-quick-action

This module adds a way to quickly create a quick action plugin by simply requiring
`xwiki-macro-quick-action` and calling the `registerMacroQuickAction` method.

## Usage

```js
require([''], function (qa) {
  qa.registerMacroQuickAction("expand", {})
})
```

### `registerMacroQuickAction(name, options)`

This method accepts only 2 parameters:

| Parameter | Type   | Description |
|-----------|--------|-------------|
| `name`    | String | The name of the macro. |
| `options` | Object | A map with multiple fields that can affect the final rendering. |

### `options` fields

| Field           | Description | Default |
|-----------------|-------------|---------|
| `language`      | Which translation to be used by the quick action. | Current language of the user |
| `defaultContent`| The placeholder content. | `Type your content here` |
| `xwikiCommand`  | Which command to be executed. | `xwiki-macro-insert` |
| `icon`          | Which icon to be used in the quick action select window. | `fa fa-cubes` |
| `parameters`    | Values for the other parameters of the macro. | — |

## Example

```js
require([''], function (qa) {
  qa.registerMacroQuickAction("expand", {})
})
```