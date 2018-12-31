# HNY_Simple_By_Vue.js
Using basic Vue.js Happy New Year 2019

ใช้ Basic Vue.js โดยใช้ V-model binding ค่าขึ้นมาแสดงพร้อมจัด CSS ให้สวยงาม มี code ตัวอย่างจาก https://codepen.io/anon/pen/KbyoJa

ตัวอย่าง Code 

<html>
   <head>
      <title>Welcom to first VueJS</title>
      <script type = "text/javascript" src = "https://cdnjs.cloudflare.com/ajax/libs/vue/2.2.1/vue.js"></script>
      <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css" integrity="sha384-GJzZqFGwb1QTTN6wy59ffF1BuGJpLSa9DkKMp0DgiMDm4iYMj70gZWKYbI706tWS" crossorigin="anonymous">
      <link href="https://fonts.googleapis.com/css?family=Kanit" rel="stylesheet">

      <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js" integrity="sha384-wHAiFfRlMFy6i5SRaxvfOCifBUQy1xHdJ/yoi7FRNXMRBu5WHdZYu1hA6ZOblgut" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/js/bootstrap.min.js" integrity="sha384-B0UglyR+jN6CkvvICOB2joaf5I4l3gm9GU6Hc1og6Ls7i6U/mkkaduKaBhlAXv9k" crossorigin="anonymous"></script>
   </head>

   <style>
     body{
       background-color: #1d5464;
       padding: 100px;
       font-family: 'Kanit', sans-serif;
     }

     h4{
       
      color: white;
    text-align: center;
    margin: 0 0 35px 0;
    font-weight: 400;
    font-size: 24px;
     }
     h1{
      background: -webkit-linear-gradient(#fff, #999);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    text-align: center;
    margin: 0 0 5px 0;
    font-weight: 900;
    font-size: 4rem;
    color: #fff;
     }

     .content{
       padding: 40px 80px 40px 80px;
       background-color: aliceblue;
       border-radius: 10px;
       max-width: 800px;
       text-align: center;
       margin-left: 151px;
     }
     .show{
       text-align: center;
       
     }

     .form-group{
       margin-bottom: 100px;
     }
   </style>
   <body>
      <div id = "intro" class="container">
        <div class="show mb-4">
            <h1>{{text}}</h1>
            <h6>By Aphiwit</h6>
        </div>
       
          <div class="form-group content center">
              <div class="input-group">
                <input type="text" class="form-control p-4" :maxlength="max" v-model="text"/>
                <div class="input-group-text px-3" v-text="max - text.length">
                </div>
              </div>
          </div>
      </div>
      <script type = "text/javascript">
         var vue_det = new Vue({
            el: '#intro',
            data: {
              max : 19,
              text : 'Happy New Year 2019',
            }
         });
      </script>
   </body>
</html>
