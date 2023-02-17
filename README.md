# Tela-simples
Meu primeiro projeto - Criei essa tela simples somente para conhecer o HTML e CSS.
Prometo melhora-la futuramente

HTML

<!DOCTYPE html> 
<html lang="pt-br"> 
  <head> <meta charset="UTF-8"> 
  <meta http-equiv="X-UA-Compatible" content="IE=edge"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <link rel="stylesheet" href="CSS/STYLES.CSS"> 
  <title>Menu responsivo</title> 
  </head> 
  <body>
     <header> 
        <nav class="nav-bar"> 
            <div class="logo"> 
                <h1>Logo</h1>
             </div> 
             <div class="nav-list"> 
                <ul> 
                    <li class="nav-item"><a href="#" class="nav-link">Inicio</a></li> 
                    <li class="nav-item"><a href="#" class="nav-link">Projetos</a></li> 
                    <li class="nav-item"><a href="#" class="nav-link">Sobre</a></li> </ul> 
                </div>
                 <div class="login-button"> <button><a href="#">Entrar</a></button> </div>
                <div class="mobile-menu-icon">
                    <button onclick="menuShow()"><img class="icon" src="ASSETS/IMG"></button>
                </div>
                  </nav> 
                 <div class="mobile-menu-icon">
                    <ul>
                      <li class="nav-item"><a href="#" class="nav-link">Inicio</a></li> 
                      <li class="nav-item"><a href="#" class="nav-link">Projetos</a></li> 
                      <li class="nav-item"><a href="#" class="nav-link">Sobre</a></li>
                      <div class="login-button"> <button><a href="#">Entrar</a></button> </div>
                    </ul>
                </div>
                 
                 </div>
                </header> 
            </body> 
            <script src="CSS/script.js"></script>
            </html>
            
            CSS
            
            *{ 
padding: 0;
margin: 0;
font-family: sans-serif;
} 
header { 
background-color: #24252a; 
box-shadow: 0px 3px 10px #464646; 
} 
.nav-bar{ 
display: flex; 
justify-content: space-between;
padding: 1.5rem 6rem;
}
.logo{ 
display: flex; 
align-items: center;
} .logo h1 { 
 color: #fff;
}
.nav-list {
display: flex;
align-items: center;
}
.nav-list ul{
display: flex;
justify-content: center;
list-style: none;
} 
.nav-item{
margin: 0 15px; 
} 
.nav-link{
text-decoration: none;
font-size: 1.15rem; 
color: #fff; 
-weight: 400; 
} 
.login-button button { 
text-decoration: none; 
background-color: #0187a7; 
font-size: 1.15rem; 
color: #fff; 
padding: 10px 15px; 
border-radius: 15px; 
} 
.login-button button a{ 
text-decoration: none;
color: #fff; 
font-weight: 500; 
font-size: 1.1rem;
 }
 .mobile-menu-icon{
    display: none;
 }
 @media screen and (max-width: 730px){
 
 .nav-bar{
        padding: 1.5rem 4rem;
 }
 .nav-item{
    display: none;
 }
 .login-button{
    display: none;
 }
 .mobile-menu-icon{
   display: block;
 }
 .mobile-menu-icon button{
   background-color: transparent;
   border: none;
   cursor: pointer;
 }
 .mobile-menu ul {
   display: flex;
   flex-direction: column;
   text-align: center;
   padding-bottom: 1rem;
 }
 .mobile-menu .nav-item{
   display: block;

 }
 .mobile-menu .login-button{
   width: 100%;
 }
   .open{
      display: block;
   }
 
 
 }
