*{
    margin:0;
    padding:0;
    box-sizing: border-box;
}
body{
    background: #f4f4f4;
}

#container{
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}
header{
    background: #000;
    color:#fff;
    padding: 20px;
}

header nav ul{
    list-style: none;
    padding: 0;
             /*top,bottom E right e left*/
    margin: 10px 0;
    display: flex;
}

header nav ul li a{
    color:#fff;
    text-transform: uppercase;
    padding: 5px 10px;

}
header nav ul li a:hover{
    text-decoration: underline 5px greenyellow;
}

#conteudo{
    display: grid;
    grid-template-columns: 1fr 200px;
}

main{
    display: flex;
    flex-wrap: wrap;
}
.produto{
    width: 200px;
    height: 400px;
    margin: 10px;
    padding: 20px;
    border: 1px solid #ddd;
    background-image:linear-gradient(#021b2b,#784ba0,#6a1d49) ;
    color:#fff;
    border-radius: 30px;
}

.produto img{
    max-width: 100%;
    height: auto;
    margin-bottom: 10px;
}

.preco{
    font-weight: 800;
    margin-top: 50px;
    color:aqua;
    font-size: 1.7rem;
}
button{
    background: aquamarine;
    margin-top: 30px;
    padding: 15px 45px;
    border-radius: 20px;
    cursor: pointer;
}
button:hover{
    background: #021b2b;
    color:#fff;
}
aside{
    width: 200px;
    background: #f8f8f8;
    padding: 20px 0;
}

footer{
    background: #021b2b;
    color:#fff;
    padding: 20px 0;
    margin-top: auto;
}
.footer-content{
    display: flex;
    justify-content: space-around;
    max-width: 100%;
    margin: 0 auto;
}
.footer-content h3{
    margin-bottom: 30px;
}
.footer-content ul{
    list-style: none;
    padding: 0;
}
.footer-content li{
    margin-bottom: 5px;
}
.footer-content a{
    color:#fff;
    text-decoration: none;
}
/* responsividade */

@media(max-width:768px){
    header nav ul{
        display: flex;
        flex-direction: column;
        gap:1rem;
        align-items: center;
    }
    header nav ul li{
        margin: 0;
    }
    #conteudo{
        grid-template-columns: 1fr;
    }
    aside{
        display: none;
        
    }
