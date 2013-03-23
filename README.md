Primary computer:

**Linux**

```bash
cd ~/Dropbox
ln -s ~/.config/sublime-text-2/Packages sublime-text-2-settings
```

**Mac**

```bash
cd ~/Dropbox
ln -s ~/'Library/Application Support/Sublime Text 2' sublime-text-2-settings
```

**Windows**

```bat
cd %HOMEPATH%\Dropbox
mklink /D sublime-text-2-settings "AppData\Roaming\Sublime Text 2\Packages"
```

Others:

**Linux**

```bash
cd ~/.config/sublime-text-2
rm -R Packages
ln -s ~/Dropbox/sublime-text-2-settings Packages
```

**Mac**

```bash
cd ~/'Library/Application Support/Sublime Text 2'
rm -R Packages
ln -s ~/Dropbox/sublime-text-2-settings Packages
```

**Windows**

```bat
cd "%HOMEPATH%\AppData\Roaming\Sublime Text 2"
rd /S /Q Packages
mklink /D Packages %HOMEPATH%\Dropbox\sublime-text-2-settings
```
