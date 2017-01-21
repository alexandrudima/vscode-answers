### To find out what a keybinding does:

1. Open `Preferences` > `Keyboard Shortcuts`
2. Click on `Define Keybinding`
3. Press your desired key combination
(e.g. doing it for <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>1</kbd>):
![image](https://cloud.githubusercontent.com/assets/5047891/22168002/1df3bb24-df6a-11e6-93f8-0842e8f37b3d.png)
4. Take note of the string shown inside the textbox (highlighted in purple above)
5. Search for that string in the default keybindings and you shall find what it is bound to.

### To remove a keybinding:

1. Identify the keybinding you would like to remove (e.g:)
```json
{ "key": "ctrl+shift+1",          "command": "editor.action.replaceOne",
                                     "when": "editorFocus && findWidgetVisible" },
```
2.a. Completely free up the keybinding. This will remove all the commands bound to `"ctrl+shift+1"`. Write the following rule:
```json
{ "key": "ctrl+shift+1" }
```
2.b. Completely remove a command. This will remove all keybindings associated with `"editor.action.replaceOne"`. Write the following rule:
```json
{ "command": "-editor.action.replaceOne" }
```
2.c. Remove that specific keybinding. Write the following rule:
```json
{ "key": "ctrl+shift+1", "command": "-editor.action.replaceOne" },
```

> Tip: Remember, in VS Code you can modify each and every keybinding to your liking, you are the sole master of your keyboard.