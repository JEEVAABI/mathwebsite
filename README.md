# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mathematical Calculations</title>
    <style>
    * {
        box-sizing: border-box;
        font-family: Arial, Helvetica, sans-serif;
      }
      body {
        background-color:rgb(133, 125, 245);
      }
      .container {
        width: 1080px;
        margin-left: auto;
        margin-right: auto;
      }
      .content {
        display: block;
        width: 100%;
        background-color: #d8f192;
        min-height: 500px;
        margin-top: 150px;
      }
      .content2{
          display: block;
          width: 100%;
          background-color: #94b33e;
          min-height: 500px;
          margin-top: 150px;
          margin-bottom: 150px;
      }
      h1{
          text-align: center;
          padding-top: 50px;
          color: rgb(36, 23, 23);
          font-style: bold;
      }
      .formelement{
          text-align: center;
          font-size:xx-large;
          margin-top: 5px;
          margin-bottom: 5px;
      
      }
      .auth{
          text-align: center;
          color:black;
          font-family: Georgia, 'Times New Roman', Times, serif;
          font-size:xx-large;
      }
    </style>
    
</head>
<body>
    <h1>Mathematical Calculations</h1>
    <div class="container">
        <div class="content">
            <h1>VOLUME OF CYLINDER</h1>
                  <form>
                      <div class=formelement>
                          <lable for="radedit">Radius=</lable>
                          <input type="text" id="radedit" value=" "/>Meters
                      </div><br>
                      <div class=formelement>
                          <lable for="htedit">Height=</lable>
                          <input type="text" id="htedit" value=" "/>Meters
                      </div><br>
                      <div class=formelement>
                          <input type="button" value="Calculate Volume" id="calbutton"/>
                      </div><br>
                      <div class=formelement>
                          <lable for="volumeedit">Volume=</lable>
                          <input type="text" id="volumeedit" readonly="0"/>Meter<sup>3</sup>
                      </div><br>
                      <div class=formelement>
                      Formula is = pi*Radius^2*Height
                      </div>
                  </form>
        </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton");
            button.addEventListener("click",function(){
                var radtext,httext,volumetext;
                var radval,htval,volumeval;
                radtext=document.querySelector("#radedit");
                httext=document.querySelector("#htedit");
                volumetext=document.querySelector("#volumeedit");
                if (Number(radtext.value)&& Number(httext.value)) {
                    radval= parseInt(radtext.value);
                    htval= parseInt(httext.value);
                }
                else{
                    alert("The number entered is incorrect, which is only to be positive numeric values..!!...")

                }

                radval=parseInt(radtext.value);
                htval=parseInt(httext.value);
                volumeval=22/7*radval*radval*htval;
                volumetext.value=volumeval;
            });
        </script>

        
        <div class="content2">
            <h1>VOLUME OF CONE</h1>
            <form>
                <div class="formelement">
                    <lable for="radiusedit">Radius=</lable>
                    <input type="text" id="radiusedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                    <lable for="heightedit">Height=</lable>
                    <input type="text" id="heightedit" value=" "/>Merers
                </div><br>
                <div class="formelement">
                    <input type="button" value="Calculate Volume" id="calbutton1"/>
                </div><br>
                <div class="formelement">
                    <lable for="voledit">Volume=</lable>
                    <input type="text" id="voledit" readonly="0"/>Meter<sup>3</sup>
                </div><br>
                <div class="formelement">
                Formula is:V=π*Radius^2*Height/3
                </div><br>
            </form>
        </div>
        
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton1");
            button.addEventListener("click",function(){
                var radiustext,heighttext,voltext;
                var radiusval,heightval,volval;
                radiustext=document.querySelector("#radiusedit");
                heighttext=document.querySelector("#heightedit");
                voltext=document.querySelector("#voledit");
                if (Number(radiustext.value)&& Number(heighttext.value)) {
                    radval= parseInt(radiustext.value);
                    htval= parseInt(heighttext.value);
                }
                else{
                    alert("The number entered is incorrect, which is only to be positive numeric values..!!...")

                }

                radiusval=parseInt(radiustext.value);
                heightval=parseInt(heighttext.value);
                volval=22/7*radiusval*radiusval*heightval/3;
                voltext.value=volval;
            });
        </script>
        <footer> <p class="auth">Developed By : A.JEEVA ABISHAKE 21500568</p></footer>
    </div>          
    
</body>
</html>
```

## OUTPUT:
### Page Outcome:
![output](output1.png)

### Page showing alert message to user:
![output](error.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.