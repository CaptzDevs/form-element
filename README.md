# form-element

##List of option 
| Key                        | Data Type |
|----------------------------|-----------|
| matchTo                   | string    |
| matchToAll                | string    |
| duplicate                 | string    |
| length                    | number    |
| startWithNumber           | boolean   |
| startWithUpperCase        | boolean   |
| startWithLowerCase        | boolean   |
| startWithSpecialCharecter | boolean   |
| noNumber                  | boolean   |
| noUpperCase               | boolean   |
| noLowerCase               | boolean   |
| noSpecialCharecter        | boolean   |
| containsNumber            | boolean   |
| containsUpperCase         | boolean   |
| containsLowerCase         | boolean   |
| containsSpecialCharecter  | boolean   |
| email                     | boolean   |
| youtubeLink               | boolean   |
| whitespace                | boolean   |
| empty                     | boolean   |
---

## Set validate option
```js
        let username = document.querySelector('#username').validate({matchTo : '#password',matchToAll : '.password-check',duplicate : checkUserRegist},'.validationText')
        let password = document.querySelector('#password').validate({matchTo : '#username'})

```
## Setup
```js
        username.setLang('en')

        username.replaceOptionText({duplicate:"Test No Duplicate"})
```
## Add event
```js
        username.initEvent('keyup',(res)=>{

        console.log(res)


        })


        password.initEvent('keyup',(res)=>{
            
            console.log(username.res)

        })
```
