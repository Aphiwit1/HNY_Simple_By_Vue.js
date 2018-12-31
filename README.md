# HNY_Simple_By_Vue.js
Using basic Vue.js Happy New Year 2019

ใช้ Basic Vue.js โดยใช้ V-model binding ค่าขึ้นมาแสดงพร้อมจัด CSS ให้สวยงาม มี code ตัวอย่างจาก https://codepen.io/anon/pen/KbyoJa

ตัวอย่าง Code 

<html>
   <head>
      <title>Welcom to first VueJS</title>
   </head>

 
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
