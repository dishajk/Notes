# To install fonts

1. Get the .ttf file
2. `mv` the .ttf file to `~\.local\share\fonts`
3. `fc-cache -f -v` to clear font cache
4. `fc-list | grep "Font name"` to verify whether the font is installed
5. Restart system if the font is not showing in the app.
