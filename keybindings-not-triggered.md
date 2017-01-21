There are a number of reasons why certain keybindings would not reach VS Code. e.g.: the OS binds OS functionality to them, other installed sofware "captures and steals" them, etc.

It is your responsibility to manage **your system** and identify what sofware / OS setting causes this behaviour. If we don't receive a keybinding, there is nothing we can do about it.

### To find out if a keybinding arrives in VS Code:

1. Open `Preferences` > `Keyboard Shortcuts`
2. Click on `Define Keybinding`
3. Press your desired key combination
(e.g. doing it for <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>1</kbd>):
![image](https://cloud.githubusercontent.com/assets/5047891/22168002/1df3bb24-df6a-11e6-93f8-0842e8f37b3d.png)
4. If the key combination does not reflect what you press or shows "unknown", it means VS Code is not receiving these key down events.


### Rebinding a command to a different keybinding
1. Identify the keybinding you would like to rebind (e.g:)
```json
{ "key": "ctrl+shift+1",          "command": "editor.action.replaceOne",
                                     "when": "editorFocus && findWidgetVisible" },
```
2. Copy paste it to your `keybindings.json` with a different `"key"` that does make its way to VS Code:
```json
{ "key": "ctrl+shift+2",          "command": "editor.action.replaceOne",
                                     "when": "editorFocus && findWidgetVisible" },
```
