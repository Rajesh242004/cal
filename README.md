## program 

```
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
    <style>
        input{
            margin-top: 20px;
            border-radius: 8px;
        }

        button{
            width: 50px;
            border-radius: 8px;
            margin-bottom: 20px;
            margin-left: 20px;
            margin-right: 20px;
        }

    </style>
</head>
<body style="padding-top: 150px; background-image: url('cal.jpg');">
    <div style="background-image: url('cal3.jpg');" class="card col-4 mx-auto ">
        <div class="card-header bg-success text-white text-center">
            <h1>CALCULATOR</h1>
        </div>
        <div class="card-body">
            <center>
                First Number :<input type="text" name="num1" id="n1" onmouseenter="Mousein1()" onmouseleave="Mouseleave1()"> <br> <br>
                Second Number:<input type="text" name="num2" id="n2" onmouseenter="Mousein2()" onmouseleave="Mouseleave2()"> <br> <br>
            
                <button class="btn btn-primary" id="add" onclick="Add()">+</button> 
                <button class="btn btn-danger" id="sub" onclick="Sub()">-</button> <br>
                <button class="btn btn-success" id="mul" onclick="Mul()">*</button> 
                <button class="btn btn-warning" id="div" onclick="Div()">/</button> <br>
        
                <p id="out">
                </p>
                </center>
        </div>
        
    </div>


    <script>
        function Mousein1(){
            document.getElementById("n1").style.background="lightgreen";
        }
        function Mousein2(){
            document.getElementById("n2").style.background="grey";
        }
        function Mouseleave1(){
            document.getElementById("n1").style.background="white";
        }
        function Mouseleave2(){
            document.getElementById("n2").style.background="white";
        }

        function Add(){
            num1=parseInt(document.getElementById('n1').value);
            num2=parseInt(document.getElementById('n2').value);
            out=document.getElementById('out');

            out.innerHTML=num1+num2;
        }
        function Sub(){
            num1=parseInt(document.getElementById('n1').value);
            num2=parseInt(document.getElementById('n2').value);
            out=document.getElementById('out');

            out.innerHTML=num1-num2;
        }
        function Mul(){
            num1=parseInt(document.getElementById('n1').value);
            num2=parseInt(document.getElementById('n2').value);
            out=document.getElementById('out');

            out.innerHTML=num1*num2;
        }
        function Div(){
            num1=parseInt(document.getElementById('n1').value);
            num2=parseInt(document.getElementById('n2').value);
            out=document.getElementById('out');

            out.innerHTML=num1/num2;
        }

    </script>
</body>
</html>
```
