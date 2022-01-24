# Web Page for Paint Application

## AIM:

To design a static website for Paint Application using HTML5 canvas.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML,CSS and canvas.

### Step 3:

Write javascript to capture move events.

### Step 4:

Perform the drawing operation based on the user input.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

```
    } else if (shape == 3){
        ctx.rect(e.offsetX, e.offsetY, 70, 35);
        ctx.strokeStyle = choose;
        ctx.linewidth = 5;
    } else if (shape == 4){
        ctx.moveTo(e.offsetX, e.offsetY);
        ctx.lineTo(e.offsetX, e.offsetY-(s/2));
        ctx.strokeStyle = choose;
        ctx.linewidth = 5;
    }
​
    ctx.stroke();
}
​
function circleclicked() {
    shape=0;
}
​
function squareclicked() {
    shape=1;
}
​
function triangleclicked() {
    shape=2;
}
​
function rectclicked() {
    shape=3;
}
​
function lineclicked() {
    shape=4;
}
    </script>
​
​
</head>
<body>
    <h1>Paint Application</h1>
    <div class="container">
        <div class="content">
            <canvas id="myCanvas" width="1050" height="650"></canvas>
        </div>
        <br/>
        <center>
            <input type="button" class="newshape" id="circle" value="Circle">
            <input type="button" class="newshape" id="square" value="Square">
            <input type="button" class="newshape" id="triangle" value="Triangle">
            <input type="button" class="newshape" id="rectangle" value="Rectangle">
            <input type="button" class="newshape" id="line" value="Line">
        </center>
        <br/>
        <center>
            <button onclick="change_color(this)" id="cypher" style="background: white;"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(49, 231, 255);"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(46, 112, 255);"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(213, 76, 255);"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(153, 0, 255);"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(54, 0, 124);"></button>
            <button onclick="change_color(this)" id="cypher" style="background: rgb(0, 0, 0);"></button>
        </center>
    </div>
    <br/>
    <center>
    <div class="footer">Developed by Nivetha M</div>
    </center>
    <script type="text/javascript">
        var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
shape=0;
let choose="#000000";
let t=50;
let s=120;
ctx.beginPath();
ctx.stroke();
c.addEventListener("click", myClickEvent);
document
.getElementById("circle")
.addEventListener("click", circleclicked);
document
.getElementById("square")
.addEventListener("click", squareclicked);
document
.getElementById("triangle")
.addEventListener("click", triangleclicked);
document
.getElementById("rectangle")
.addEventListener("click", rectclicked);
document
.getElementById("line")
.addEventListener("click", lineclicked);
    </script>
    
</body>
</html>
```

## OUTPUT:

![GitHub Logo](.//n1.png)

## Result:

Thus a website is designed and validated for paint application using HTML5 canvas.
