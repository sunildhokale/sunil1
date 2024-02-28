# sunil1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>netflix</title>
    <style>
        body{
            margin: 0;
        }
        #grid{
            height: 100vh;
            background-color: crimson;
            display: grid;
            grid-template-columns: 1fr 1fr 1fr 1fr;
            gap: 10px;
            transition: 3s;
        }
        :where(.one,.two,.three,.four){
            background-color: navajowhite;
            transition: 3s;
        }
        :where(.one,.two ,.three,.four):hover{
        background-color: rgb(108, 70, 231);    
        }
        /* #grid .left:hover{
            background-color: blue;
            grid-template-columns: 2fr 0.5gr 0.5 fr; */
        } 
        #grid:has(.one:hover){
            grid-template-columns: 2fr 0.5fr 0.5fr 0.5fr;
        }
        #grid:has(.two:hover){
            grid-template-columns: 0.5fr 2fr 0.5fr 0.5fr;
        }
        #grid:has(.three:hover){
            grid-template-columns: 0.5fr 0.5fr  2fr 0.5fr;
        }
        #grid:has(.four:hover){
            grid-template-columns: 0.5fr 0.5fr 0.5fr 2fr;
        }
    </style>
</head>
<body>
    <div id="grid">
        <div class="one"></div>
        <div class="two"></div>
        <div class="three"></div>
        <div class="four"></div>
    </div>
    <div class="main">
        <div class="one"></div>
    </div>
</body>
</html>
