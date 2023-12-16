### Error to create jango project in my windows 

#### My error for ` django-admin startproject yourprojectname `

##### My Error 
```js
 django-admin startproject Ordain_Jango
django-admin : The term 'django-admin' is not recognized as the name of a cmdlet, function, script
file, or operable program. Check the spelling of the name, or if a path was included, verify that
the path is correct and try again.
At line:1 char:1
+ django-admin startproject Ordain_Jango
+ ~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (django-admin:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException


```

### solve the error 

follow https://bobbyhadz.com/blog/django-admin-is-not-recognized-as-internal-or-external-command

```bash 
# 👇️ create virtual environment
python -m venv venv

# 👇️ activate on Windows (cmd.exe)
venv\Scripts\activate.bat

# 👇️ activate on Windows (PowerShell)
venv\Scripts\Activate.ps1

```

