
### Mastering line wrapping

There are two important settings in VS Code that control line wrapping.

* `editor.wrappingColumn` (300 by default)
* and `editor.wordWrap` (false by default)

It is important to understand the need for two distinct settings and how to tweak them to suit your use-case:

Examples (with explanations):

| `wordWrap` | `wrappingColumn` | Explanation |
|---|---|---|
| false | 300 | Lines will wrap at <code>300</code> |
| false | 0 | Lines will wrap at <code>viewport_column</code> |
| false | -1 | Lines will never wrap. |
| true | 300 | Lines will wrap at <code>min(viewport_column, 300)</code> |
| true | 0 | Lines will wrap at <code>viewport_column</code> |
| true | -1 | Lines will never wrap. |
