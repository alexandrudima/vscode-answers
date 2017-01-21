We listen to `mousewheel` events coming in from Chromium. It is Chromium's job to emit `mousewheel` events when using two fingers on the trackpad. Closing here because there is no possible code change we can do in our code to make this work. If you experience issues, please look into reporting them to Chromium.

### To find out what Chromium version VS Code uses:

* Go to `Help` > `About` and look for the Renderer version

![image](https://cloud.githubusercontent.com/assets/5047891/22174828/fd47b564-dfe7-11e6-9a55-a119b4b08c3b.png)

* You can then proceed to install Chromium at the same version and try if your problem reproduces in that version.

### Known workarounds

For example, my trackpad (on a Surface Book) works correctly after "restoring" and then maximizing back the VS Code window (Possibly related #13612).
