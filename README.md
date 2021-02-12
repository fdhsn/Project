@import url('https://fonts.googleapis.com/css2?family=Pangolin&display=swap');
*{
    margin: 0;
    padding: 0;
    font-family:  Calibri, 'Trebuchet MS', sans-serif;
    scroll-behavior: smooth;
}
.heading{
    width: 70%;
    margin: 10px auto;
}
.heading p{
    text-align: center;
    font-size: 25px;
}
.graph{
    width: 500px;
    height: 500px;
    position: relative;
    margin: 20px auto;

}
.x-axis{
    background-color: pink;
    width: 500px;
    height: 5px;
    position: absolute;
    top: 250px;
}
.y-axis{
    background-color: pink;
    width: 5px;
    height: 500px;
    position: absolute;
    left: 250px;
}
.y-axis p:nth-child(1), 
.y-axis p:nth-child(2){
    padding-left: 10px;
    font-size: 20px;
}
.y-axis p:nth-child(2){
    position: absolute;
    bottom: 0px;
}
.pos1,
.pos2,
.pos3,
.pos4{
    font-size: 20px;
    position: absolute;
    
}
.pos1{
    left: 150px;
}
.pos2{
    right: 180px;
}
.pos3{
    top: 180px;
}
.pos4{
    right: 0px;
    top: 180px;
}
.x-axis p:nth-child(1),
.x-axis p:nth-child(2){
    padding-top: 10px;
    font-size: 20px;
}
.x-axis p:nth-child(2){
    position: absolute;
    right: 0px;
    top: 0px;
}
.line{
    height: 450px;
    width: 450px;
    position: absolute;
    left: 22px;
    top: 15px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.degree{
    background-color: cyan;
    position: relative;
    height: 20px;
    width: 20px;
    border: 3px solid gray;
    border-radius: 50%;
    z-index: 99;
    left: 225px;
    top: 0px;
    transition: all 1s ease-in-out;
}
.deg-p{
    display: none;
}
.deinput{
    width: 38%;
    margin: auto;
    position: relative;
    display: none;
    animation: uptodown .5s ease-in-out;
}

@keyframes uptodown{
    from{
       top: -74px; 
    }
    to{
        top: 0px;
    }
}
#input{
    margin-top: 20px;
    border: none;
    border-bottom: 2px solid gray;
    outline: none;
    font-size: 20px;
    padding: 10px;
    transition: all .5s ease-in-out;
}
.label{
    position: absolute;
    font-size: 1.5rem;
    top: 34px;
    color: maroon;
    transition: all .5s ease-in-out;
}

#submit{
    font-size: 18px;
    border: 2px solid maroon;
    background-color: gold;
    padding: 10px;
    margin: 0px 10px;
    transition: all 0.5s ease-in-out;
    margin-top: 20px;
}
#submit:hover{
    background-color: red;
    color: white;
    cursor: pointer;
}
#submit:disabled{
    border: 2px solid cyan;
}
#submit:disabled:hover{
    background-color: white;
    color: grey;
    cursor: no-drop;
}
.quadrant p{
    text-align: center;
    font-size: 3rem;
}
.line1{
    text-align: center;
    font-size: 2.5rem;
    margin: 15px 0px;
    font-family: 'Pangolin', cursive;
}
.buttons{
    width: 40%;
    margin: auto;
}
.btn-tri{
    width: 27%;
    margin: auto;
    padding: 20px 10px;
    font-size: 2rem;
    background-color: white;
    border: 2px solid red;
    margin: 10px 20px;
    transition: all .5s ease-in-out;
}
.btn-tri:hover{
    background-color: red;
    color: white;
    cursor: pointer;
}
.btn-tri2{
    width: 100%;
    margin: auto;
    padding: 10px 5px;
    font-size: 1.5rem;
    background-color: white;
    border: 2px solid red;
    margin: 30px 20px;
    transition: all .5s ease-in-out;
    text-align: center;
}
.btn-tri2:hover{
    background-color: red;
    color: white;
    cursor: pointer;
}
.btn-tri:disabled{
    border: 2px solid cyan;
}
.btn-tri:disabled:hover{
    background-color: maroon;
    color: grey;
    cursor: no-drop;
}
.wrong{
    margin-bottom: 20px;
    color: red;
    display: none;
}
.footer{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    background-color: black;
}
.footer p{
    color: white;
    font-size: 19px;
    padding: 20px;
}

/* Responsive */

@media only screen and (max-width: 1000px){
    .buttons{
        width: 100%;
    }
}
