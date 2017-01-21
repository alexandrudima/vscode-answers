If you are sensitive to get things pixel-perfect (like me), I can recommend not to use `window.zoomLevel`. We do everything correct on our side, paint the `<div>s` at integer coordinates, etc. But by setting `window.zoomLevel` to `-2` I think Chromium interprets that as `80%` and begins multiplying all our nice integers with `0.8`. This causes the nice integers to become floats and it is inevitable that they get rounding errors.

I recommend to stick with customizing `fontSize` and `lineHeight`. I wonder what makes you want to change `window.zoomLevel` to begin with?
