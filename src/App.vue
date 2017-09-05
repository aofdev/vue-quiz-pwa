<template>
  <div id="app">
   <nav class="navbar   navbar-default navbar-fixed-top">
    <div class="container-fluid">
        <h1 id="headText" style="font-size:2.7em;font-family: 'Oswald', sans-serif;" class="animated zoomIn"><b>Vue</b></h1>
    </div>
</nav>
<div class="wrapper">
<div id="header">
    <br><br>
<h1 id="text" class="animated fadeInLeft">The Super Quiz</h1>
</div>
<br>
</div>
    <main>
      <router-view></router-view>
    </main>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
body {
  margin: 0;
   background-color: #eeeeee;
            font-family: 'Kanit', sans-serif;
            text-align: center;
}



main {
  text-align: center;
  margin-top: 40px;
}
      .wrapper {
            min-height: 100%;
            height: auto !important;
            height: 100%;
            margin: 0 auto -4em;
        }

   .navbar-default {
            border-color:transparent;
            box-shadow:0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23);
            min-height: 64px;
            margin-bottom: -10px;
        }


        ul, ol {
            margin-top:0;
            margin-bottom:11.5px;
        }

        .navbar-default .navbar-nav > li > a {
            color:black;
        }.navbar-default .navbar-nav > li > a:hover {
             color: #fff;
         }

           #header{
            background-color: darkorange;
            height: 250px;
        }
      
      

        #text{
            font-size: 5em;
            margin-top: 80px;
            color: white;
            text-shadow: 0 1px 0 #ccc,
            0 2px 0 #c9c9c9,
            0 3px 0 #bbb,
            0 4px 0 #b9b9b9,
            0 5px 0 #aaa,
            0 6px 1px rgba(0,0,0,.1),
            0 0 5px rgba(0,0,0,.1),
            0 1px 3px rgba(0,0,0,.3),
            0 3px 5px rgba(0,0,0,.2),
            0 5px 10px rgba(0,0,0,.25),
            0 10px 10px rgba(0,0,0,.2),
            0 20px 20px rgba(0,0,0,.15);

        }
        #headText{
            color: orange;
        }


        @media screen and (max-width: 767px) {
            #text {
                font-size: 2.7em;
            }
            #show{
                font-size: 30px;
            }
        }


        @media (min-width: 768px) and (max-width: 991px) {
            #text {
                font-size: 3.7em;
            }
            #show{
                font-size: 35px;
            }
        }


        @media (min-width: 992px) and (max-width: 1199px) {
            #text {
                font-size: 4.5em;
            }
            #show{
                font-size: 40px;
            }
        }

        @media screen and (min-width: 1200px) {
            #text {
                font-size: 5em;
            }
            #show{
                font-size: 45px;
            }
        }
</style>
