/**_ Get All Users _**/
(GET)> https://loginzomato.herokuapp.com/api/auth/users

/**\*\***Register**\***/
(POST)> https://loginzomato.herokuapp.com/api/auth/register
(body) =>{
"name" : "Sudha",
"email" : "sudha@gmail.com",
"password" : "12345678",
"role" : "Admin"

}
/**\*\***Login**\***/
(POST) => https://loginzomato.herokuapp.com/api/auth/login
(body) => {
"email" : "sudha@gmail.com",
"password" : "12345678"
}
(response)=> {auth:true,token:'dgsdg'}

/**\*\***UserInfo**\***/
(GET) => https://loginzomato.herokuapp.com/api/auth/userinfo
(Header) => {'x-access-token':'token value from login'}
