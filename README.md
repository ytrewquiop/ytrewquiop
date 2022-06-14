<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>stackoverflow</title>
  <style>
    :root{
      --black:rgba(28, 219, 219, 0.045);
      --blue:rgb(18, 83, 235);
    }
    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    .con{
      width: 100vw;
      height:100vh;
      background: url('https://source.unsplash.com/random/300×300') no-repeat scroll center center;
      background-size: 100% 100%;
    }
    .navbar{
     width: 100%;
     height: auto;
     display: flex;
     flex-flow: row nowrap;
     justify-content: center;
     align-items: center;
     background-color: aliceblue;
     position: relative;
     position: sticky;
    }
   .lines{
    width: clamp(15%,2.5rem,25%);
    height:1.2px;
    background: black;
    margin: 0.2rem auto;
   }
   .nav-pro{
    width: auto;
    height: auto;
    padding: 0.2rem;
   }
   .line-col{
    width: 100%;
    height: 2px;
    background: rgb(233, 164, 36);
   }
   .second-pro{
    width: auto;
    display: flex;
    font-size: 11px;
   }
   .om{
    text-decoration: none;
    color: rgb(70, 65, 65);
    text-align: center;
    margin: 0 0.5rem;
    position: relative;
    transition: color 1s ease-in; 
   }
   .third-pro{
    display: flex;
    flex-direction: row;
    width: auto;
    font-size: 11px;
   }
   p,h4{
    display: inline;
   }
   .four-pro{
    width: clamp(15%,23%,25%);
   }
   input{
    width: 100%;
    border-radius: 2px;
    aspect-ratio: 30/1;
    background: rgb(165, 148, 148);
    outline: none;
    border: 0.5px solid rgb(0, 149, 255);
    
   }
   input::placeholder{
    color: rgb(240, 236, 236);
    font-size: 9px;
    margin-left: 25px;
   }
   button{
   color: aliceblue;
   background-color: var(--blue);
   height: 2em;
   font-size: 9px;
   padding: 0 0.4rem;
   border: none;
   margin: 0 3px;
   border-radius: 2px;
   }
   button:nth-child(1){
   color: var(--blue);
   background-color: aliceblue;
   border: 0.5px solid rgb(95, 86, 223);
   }
   @media screen and (max-width:720px){
    .third-pro,.four-pro{
      display: none;
    }
    .five-pro{
      overflow-x: auto;
      scroll-behavior: smooth;
    }
   }
  .om:hover{
   color: red;
  }
  .om::after{
    content: "";
    display: block;
    width: 0;
    height: 1px;
    position: absolute;
    background: rgb(70, 65, 65);
    left: 2%;
    bottom: 1%;
    transition: width 1s ease-in;
  }
  .om:hover::after{
    width: 100%;
  }
  input[type="search"]::-webkit-search-decoration,
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-results-button,
input[type="search"]::-webkit-search-results-decoration { display: none; }
  



*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.container{
  background-color: lightcoral;
  border: 1px solid greenyellow;
  /* margin: 10px 0; */
  padding: 25px;
  width: 100vw;
  height: auto;
  box-sizing: border-box;
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(150px,1fr));
  grid-template-rows: repeat(auto-fit,auto);
  /* grid-auto-rows: 1fr; */
  /* grid-column-gap: 20px;
  grid-row-gap: 100px; */
  grid-gap: 10px 20px;

}
.box{
  background-color: cornflowerblue;
  border: 1px solid blueviolet;
  transition: all 3s;
  /* background-image: linear-gradient(to to right, orange) ; */
  /* margin: 10px 2px; */
}
.box img{
  width: 100%;
  height: auto;
}
.box:hover{
  transform: scale(1.3) skew(2deg);
  background-color: orchid;
  box-shadow: 2px 2px 20px 10px black;
  /* background-image: url('./image/temple.jpg')  linear-gradient(to to right,pink orange,cyan); */

}
p:hover::selection{
  background-color: aqua;
  color: aliceblue;
}
/* .p-i-div:hover{
  visibility: hidden;
} */
#box-8{
  /* grid-column: 2/3;
  grid-row: 1/2; */
}
/* #box-2{
  grid-column: 2/3;
  grid-row: 3/4;
} */
.container-2{
  background-color: black;
  width: 100vw;
  height: 40rem    +    1rem;
  padding: 3rem 1rem;
}
#item-1 h3,h3{
  color: rgb(97, 96, 96);
  font-size: 14px;
}
.al{
  text-decoration: none;
  color: aliceblue;
  font-size: clamp(0.5rem,0.7rem,1rem);
}
.al:hover{
  text-decoration: underline;
}
.container-2{
  display: flex;
  /* grid-template-columns: repeat(auto-fit,minmax(80px,1fr));
  grid-template-rows: repeat(1,1fr);
  grid-auto-rows: 1fr;
  flex-direction: row; */
  flex-flow: row wrap;
  justify-content: space-around;
  align-content: space-around;
}
i{
  margin-right: 2px;
}
.p-2{
  font-size: clamp(0.5rem,0.7rem,1rem);
  line-height: clamp(1rem,1.2rem,2rem);
  color: aliceblue;
}
#item-5{
  border-left: 1px solid white;
  height: auto;
  padding-left: 1rem;
}
.item{
  margin: 1rem 0;
}
@media screen  and (max-width:384px){
  .p-2{
    margin-top: 6px;
  }


}
@media screen  and (max-width:400px){
  .container{
    grid-template-columns: 1fr;
  }


}
 

.none{
  text-decoration: none;
  scroll-behavior: smooth;
}

.fixed{
  height: 50px;
  width: 50px;
  border-radius: 50%;
  background: blueviolet;
  position: absolute;
  bottom: 5px;
  right: 5px;
  scroll-behavior: smooth;
}
.fixed::after{
  content: "";
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: black;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  clip-path: polygon(52% 26%, 52% 57%, 65% 59%, 48% 100%, 26% 60%, 40% 59%, 40% 26%);
  scroll-behavior: smooth;
}
  </style>
</head>
<body>
  <div class="con">
    <div class="line-col"></div>
    <div class="navbar">
      <div class="nav-pro first-pro" style="width: clamp(4rem,4.2rem,5rem);">
        <div class="lines"></div>
        <div class="lines"></div>
        <div class="lines"></div>
      </div>
      <div class="nav-pro second-pro">
        <p style="margin-right: 2px;">STACK</p>
        <h4>OVERFLOW</h4>
      </div>
      <div class="nav-pro third-pro">
        <div><a href="#" class="om">about</a></div>
        <div><a href="#" class="om">products</a></div>
        <div><a href="#" class="om">for team</a></div>
      </div>
      <div class="nav-pro four-pro">
        <input type="search" placeholder="search...">
      </div>
      <div class="nav-pro five-pro" style="display: flex;">
        <button><a href="./signup.html" style="text-decoration: none; color: blue;">Log in </a></button>
        <button><a href="./signup.html" style="text-decoration: none; color: white;">Sign up </a></button>
      </div>
    </div>
    
  </div>
  <!-- <main> -->
    <div class="container">
      <div class="box" id="box-1">

        <p>THIS IS BOX-1</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-2">

        <p>THIS IS BOX-2</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-3">

        <p>THIS IS BOX-3</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-4">

        <p>THIS IS BOX-4</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-5">

        <p>THIS IS BOX-5</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-6">

        <p>THIS IS BOX-6</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-7">

        <p>THIS IS BOX-7</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-8">

        <p>THIS IS BOX-8</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>
      <div class="box" id="box-9">

        <p>THIS IS BOX-9</p>
        <img src="./image/sun.jpg" alt="image of sun" loading="lazy">
        <p class="p-i-div">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos, eveniet?</p>

      </div>

    </div>
  <!-- </main> -->
  <footer>
    <div class="container-2">
      <div class="item" id="item-1">
        <h3>about</h3>

        <div class="a-1">
          <a href="#" class="al"><i class="fa-solid fa-message-middle"></i>contact us</a>
        </div>

        <div class="a-1">
          <a href="#" class="al">about us</a>
        </div>
        <div class="a-1">
          <a href="#" class="al">careers</a>
        </div>
        <div class="a-1">
          <a href="#" class="al">flipkart stories</a>
        </div>
        <div class="a-1">
          <a href="#" class="al">press</a>
        </div>
        <div class="a-1">
          <a href="#" class="al">flipkart wholesale</a>
        </div>
        <div class="a-1">
          <a href="#" class="al">corporate information</a>
        </div>




      </div>
      <div class="item" id="item-2">
        <h3>HELP</h3>
        <div class="a-1"><a href="#" class="al">payments</a></div>
        <div class="a-1"><a href="#" class="al">shipping</a></div>
        <div class="a-1"><a href="#" class="al">cancellation & returns</a></div>
        <div class="a-1"><a href="#" class="al">FAQ</a></div>
        <div class="a-1"><a href="#" class="al">report infrignment</a></div>
      </div>
      <div class="item" id="item-3">
        <h3>POLICY</h3>
        <div class="a-1"><a href="#" class="al">Return policy</a></div>
        <div class="a-1"><a href="#" class="al">Terms of use</a></div>
        <div class="a-1"><a href="#" class="al">Security</a></div>
        <div class="a-1"><a href="#" class="al">Sitemap</a></div>
        <div class="a-1"><a href="#" class="al">EPR compliance</a></div>
      </div>
      <div class="item" id="item-4">
        <h3>SOCIAL</h3>
        <div class="a-1"><a href="#" class="al">Facebook</a></div>
        <div class="a-1"><a href="#" class="al">Twitter</a></div>
        <div class="a-1"><a href="#" class="al">You Tube</a></div>
      </div>
      <div class="item" id="item-5">
        <h3>Mail Us:</h3>
        <p class="p-2">Flipkart Internet Private Limited,</p>
        <p class="p-2">Buildings Alyssa, Begonia &</p>
        <p class="p-2">Clove Embassy Tech Village,</p>
        <p class="p-2">Outer Ring Road, Devarabeesanahalli Village,</p>
        <p class="p-2">Bengaluru, 560103,</p>
        <p class="p-2">Karnataka, India</p>
      </div>
      <div class="item" id="item-6">
        <h3>Registered Office Address</h3>
        <P class="p-2">Flipkart Internet Private Limited,</P>
        <P class="p-2">Buildings Alyssa, Begonia &</P>
        <P class="p-2">Clove Embassy Tech Village,</P>
        <P class="p-2">Outer Ring Road, Devarabeesanahalli Village,</P>
        <P class="p-2">Bengaluru, 560103,</P>
        <P class="p-2">Karnataka, India</P>
        <P class="p-2">CIN : U51109KA2012PTC066107</P>
        <P class="p-2">Telephone: 1800 202 9898</P>
      </div>
    </div>
  </footer>
  <a href="#item-6" class="none"><div class="fixed"></div></a>
</body>
</html>
