index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div class="card">
        <ul class="ul">


            <li>
                <i class='bx bx-drink'></i>
            </li>
            <li>
                <i class='bx bx-film'></i>
            </li>
            <li>
                <i class='bx bx-sore-alt'></i>
            </li>
            <li>
                <i class='bx bx map'></i>
            </li>
            

        </ul>
        <a class="https://compragamer.net/pga/imagenes_publicadas/compragamer_Imganen_general_26074_Placa_de_Video_Zotac_GeForce_RTX_3090_24GB_GDDR6X_Trinity_OC_a2c94661-grn.jpg">
    <img src="https://compragamer.net/pga/imagenes_publicadas/compragamer_Imganen_general_26074_Placa_de_Video_Zotac_GeForce_RTX_3090_24GB_GDDR6X_Trinity_OC_a2c94661-grn.jpg" alt="">
        </a>
    <div class="con-text"></div>
    <h2> imagen </h2>
    <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eos nesciunt natus molestiae explicabo voluptas dolore necessitatibus, rerum illo ducimus ex sit nulla fugit, ullam aliquid maiores ea. Quia, magni architecto?
    </p>
    <button> Contactar </button>
    </div>
    </div>
</body>
<link href="stilos.css" rel="stylesheet" type="text/css">
</html>

css

.card {
    width: 300px;
    height: 400px;
    background: #000;
    border-radius: 30px;
    overflow: hidden;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: all .25s ease;
    backface-visibility: hidden;

}
.card:hover {

    transform: scale(.9);

}
.card:hover:after{

height: 200px;
}
.card:hover .con-text p { 
    margin-bottom:0px ;
    opacity: 1;
}
.card:hover img{
    transform: scale(1.25);
}
.card:hover .ul{
    transform: translate(0);
    opacity: 1;
}
.card:after{
    width: 100%;
    content:'';
    left: 0px;
    bottom: 0px;
    height: 150px;
    position:absolute;
    background: linear-gradient(100deg, rgba(0,0,0,0) 0%, rgba(0,0,0,1)100%);
    z-index: 20;
    transition: all .25s ease;
}
.card img{
    height: 100%;
    z-index: 10;
    transition: all .25s ease;
}
.card .con-text{
    z-index: 30;
    position:absolute;
    bottom: 0px;
    color:#fff;
    padding: 20px;
    padding-bottom: 30px;
}
.card .con-text p{
    font-size: .8rem;
    opacity: 0;
    margin-bottom: -170px;
    transition: all .25s ease;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    flex-direction: column;

}
.card .con-text p button{
    padding: 7px 17px;
    border-radius: 12px ;
    background: transparent;
    border: 2px solid #fff;
    color: #fff; 
    margin-top: 10px;
    margin-left: auto;
    cursor: pointer;
    transition: all .25s ease;
    font-family: poppins;
    font-size: .75rem;
    outline: none;

}
.card .con-text p button:hover {
    background: #fff;
    color:#000;
}
.ul{
    position: absolute;
    right: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    z-index: 40;
    border-radius: 14px;
    border-left:0px ;
    padding-top: 8px;
    padding-bottom: 8px;
    top: 0px;
    transform: translate(100%);
    transition: all .25s ease;
}
.ul li{
    background: #fff;
    list-style: none;
    width: 40px;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 7;
    transition: all .25s ease;
    backface-visibility: hidden;

}
.ul li:last-child{
    border-radius: 0px 0px 12px 12px;
}
.ul li:first-child {
    border-radius: 12px 12px 0px 0px;
}
.ul li:hover{
    opacity: 1;
    transform: translate(-7px, -4px);
    border-radius: 6px;

}
.ul li i{
    font-size: 1,4rem;
    color: #000;
}
