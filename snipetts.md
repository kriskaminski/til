# Snippets

usefull snippets from across the web and real life

## List files> 1GB in windows cmd

```cmd
:: If in this folder or subdirectories there is a file with size greater than 1GB print its path
forfiles /s /m * /c "cmd /c if @fsize GEQ 1073741824 echo @path"
:: /s search into subdirectories recursively
:: /m mask Defaults to *.\*
:: /c overwrite default command (cmd /c echo @file)
```
