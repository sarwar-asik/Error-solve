# Error-solve

#### 1. (github)
    $ git push -u origin main
        remote: Repository not found.
        fatal: repository 'https://github.com/sarwar-asik/Ready-Baend1.git/' not found 
#### 1. solve 
    git credential-manager uninstall
    git credential-manager install
    git remote remove origin
