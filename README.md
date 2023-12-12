# calculator
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Calculator</title>

    <style>
    #box{
    height:400px;width:200px;
    border:1px solid black;
    margin:40px; 
    position:relative;   
    left:150px;
}

#inp{
    height:50px;width:190px;
    margin:2px;
    border:1px solid black; 
    border-radius:12px;
    
}
marquee{
    position:relative;
    top:15px;
    font-size: 50px;
    font-family: 'New Times Roman';
}
.btn{
   height:50px;width:50px;
   border:1px solid black;
   margin:2px;
   display:inline-block;
   flex-wrap: wrap; 
   border-radius:5px;
}
    </style>
  </head>
<body>
<marquee>Calculator</marquee>
<div id="box">
    <input type="text" id="inp">
    <div>
       <button class="btn" onclick="val=''; document.querySelector('#inp').value=val;">C</button>
       <button class="btn" onclick="val=val+ '1'; document.querySelector('#inp').value=val;" >1</button>
       <button class="btn" onclick="val=val+ '2'; document.querySelector('#inp').value=val;">2</button>
       <button class="btn" onclick="val=val+'+'; document.querySelector('#inp').value=val;">+</button>
       <button class="btn" onclick="val=val+ '3'; document.querySelector('#inp').value=val;">3</button>
       <button class="btn" onclick="val=val+ '4'; document.querySelector('#inp').value=val;">4</button>
       <button class="btn" onclick="val=val+ '-'; document.querySelector('#inp').value=val;">-</button>
       <button class="btn" onclick="val=val+ '5'; document.querySelector('#inp').value=val;">5</button>
       <button class="btn" onclick="val=val+ '6'; document.querySelector('#inp').value=val;">6</button>
       <button class="btn" onclick="val=val+ '*'; document.querySelector('#inp').value=val;" >*</button>
       <button class="btn" onclick="val=val+ '7'; document.querySelector('#inp').value=val;">7</button>
       <button class="btn" onclick="val=val+ '8'; document.querySelector('#inp').value=val;">8</button>
       <button class="btn" onclick="val=val+ '/'; document.querySelector('#inp').value=val;">/</button>
       <button class="btn" onclick="let r = eval(val); document.querySelector('#inp').value=r;">=</button>
       <button class="btn" onclick="val=val+ '9'; document.querySelector('#inp').value=val;">9</button>
       <button class="btn" onclick="val=val+ '0'; document.querySelector('#inp').value=val;">0</button>
       <button class="btn" onclick="val=val+ '.'; document.querySelector('#inp').value=val;">.</button>
       
    </div>
</div>

<script>
    let val='';
    document.querySelector('#inp').value=val;
</script>
</body>
</html>
