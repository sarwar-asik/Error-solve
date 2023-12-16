### Error for cloning a private repository

#### Error

```bash
┌──(sarwar㉿ashik)-[~/…/Ashik/WEB/JOB/Champ_coder]
└─$ git clone https://github.com/Champ-Coders/redirect-blood-donation-campain-server.git
Cloning into 'redirect-blood-donation-campain-server'...
Username for 'https://github.com': sarwar-asik
Password for 'https://sarwar-asik@github.com':


remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Champ-Coders/redirect-blood-donation-campain-server.git/'

```

##### Solve set config in your device

```bash

git config --
```

### If error again . You have generate token from
https://github.com/settings/tokens

```bash
git clone https://sarwar-asik:<YOUR-PAT>@github.com/sampod76/kartick_education_server.git

examples:
 git clone https://sarwar-asik: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@github.com/sampod76/kartick_education_server.git

```