# form-element

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
