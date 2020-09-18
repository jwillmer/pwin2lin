# pwin2lin

Convert Putty session from Windows to Linux.

## How To

### Export from Windows

- Open registry editor: `WIN+R` - `regedit`
- Browse to `HKEY_CURRENT_USER\SOFTWARE\SimonTatham\PuTTY`
- Export Putty folder to `putty.reg`

### Convert

- Fix file encoding of `putty.reg` to UTF-8 and Unix(LF)
- Execute script `./pwin2lin.pl putty.reg .putty`
- Investigate if `.putty/sessions` contains your sessions

### Import

- Import `.putty` folder to Linux home directory
- Start putty and enjoy :)


## Original source

https://code.google.com/p/pwin2lin