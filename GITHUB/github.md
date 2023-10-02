# Error-solve
#### 1. (github)
```js
    $ git push -u origin main
        remote: Repository not found.
        fatal: repository 'https://github.com/sarwar-asik/Ready-Baend1.git/' not found 
```
#### 1. solve 

```bash
    git credential-manager uninstall
    git credential-manager install
    git remote remove origin
```