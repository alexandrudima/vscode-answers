### Scrolling with the trackpad is not smooth

VS Code is built on top of Chromium. At this point it is Chromium v53. There are a number of issues that have been already fixed in newer versions of Chromium. We will benefit from these fixes once we adopt a newer version of Electron, which we do quite frequently.

### What you can do

Download Chromium v53 and see if scrolling with the trackpad is smooth when you browse the internet.

Download the latest version of Chromium and see if scrolling with the trackpad is smooth.

If it is not, then consider creating an issue against Chromium.

### Known workarounds

For example, my trackpad (on a Surface Book) works correctly after "restoring" and then maximizing back the VS Code window (Possibly related #13612).

There are no code change we can do on our side to workaround these issues.
