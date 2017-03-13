#Ptt-Alertor
<img align="right" src="https://raw.githubusercontent.com/liam-lai/ptt-alertor/master/logo.jpg">
[![Build Status](https://travis-ci.org/liam-lai/ptt-alertor.svg?branch=master)](https://travis-ci.org/liam-lai/ptt-alertor)
[![codecov](https://codecov.io/gh/liam-lai/ptt-alertor/branch/master/graph/badge.svg)](https://codecov.io/gh/liam-lai/ptt-alertor)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Happy Chinese New Year

## Path

### Board

* /boards/[board name]/articles

### User

* GET /users/[account]

* POST /users

```
{
    "profile":{
        "account": "sample",
        "email":"sample@mail.com" 
    },
    "subscribes":[
        {
            "board":"gossiping",
            "keywords":["問卦","爆卦","公告"]
        },
        {
            "board":"lol",
            "keywords":["閒聊"]
        }
    ]
}
```

* PUT /users/[account]

```
{
    "profile":{
        "account": "sample",
        "email":"sample@mail.com" 
    },
    "subscribes":[]
}
```