# Grey Dark Theme
A lower contrast dark grey theme for Visual Studio 2026

Based on https://github.com/gluks/vs-theme-grey-dark
Based on [Dark 2019 theme](https://github.com/madskristensen/DarkTheme2019)

## Font
This theme is designed to be used with the `Consolas` font. You can change the font in 

`Tools -> Options -> Environment -> Fonts and Colors`

## Examples

![](img/example.png)

### C#

![](img/csharp.png)

### JSON

![](img/json.png)

### XML / XAML

![](img/xaml.png)

## License

[MIT License](LICENSE)

## SSMS / SQL Server Management Studio 22

Can also install it in SSMS / SQL Server Management Studio 22.

Example on my system:

Close SSMS / SQL Server Management Studio 22.

Base path: C:\Program Files\Microsoft SQL Server Management Studio 22\Release\Common7\IDE\Extensions

Create folder: C:\Program Files\Microsoft SQL Server Management Studio 22\Release\Common7\IDE\Extensions\GreyDark2026

You need two files, CustomTheme.pkgdef and CustomTheme2026.pkgdef.
You can compile this project and get them from the \bin-folder, or download the VS extension here: https://marketplace.visualstudio.com/items?itemName=ContosoCorporation.GreyDarkTheme2026

The downloaded file in named GreyDarkTheme2026.vsix. Unpack the file (it is a zip-file) with eg. 7-Zip. Among the unpacked files should be CustomTheme.pkgdef and CustomTheme2026.pkgdef.

Put files CustomTheme.pkgdef and CustomTheme2026.pkgdef into the GreyDark2026-folder.

Delete file: C:\Program Files\Microsoft SQL Server Management Studio 22\Release\Common7\IDE\Extensions\extensions.configurationchanged
Create a new and empty file with same name.
VS uses the timestamp of this file to tell if it need to rebuild its internal guts.

Start SSMS / SQL Server Management Studio 22.

If it worked, you should see Tools->Themes->Grey Dark 2026. Select it.

You may need to restart SSMS / SQL Server Management Studio 22 one more time after selecting it.
