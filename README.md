# form-element


""js  
        let username = document.querySelector('#username').validate({matchTo : '#password',matchToAll : '.password-check',duplicate : checkUserRegist},'.validationText')
        let password = document.querySelector('#password').validate({matchTo : '#username'})


        username.setLang('en')

        username.replaceOptionText({duplicate:"Test No Duplicate"})

        username.initEvent('keyup',(res)=>{

        console.log(res)


        })


        password.initEvent('keyup',(res)=>{
            
            console.log(username.res)

        })
"""