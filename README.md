<!DOCTYPE html>
<html>
<head>
 <title>To-do-list</title>
<link href="style.css">
</head>
<body>
    <style>
        *{
            padding: 0;
            margin: 0;
            box-sizing: border-box;
        }
        body{
            height: 100vh;
            background: linear-gradient(pink,rgb(179, 90, 238));
        }
        .app{
            font-family: 'Courier New', Courier, monospace;
            width: 100vw; 
            position: absolute;
            left: 0;
            right: 0;
            top: 40px;
        }
        .container{
            padding: 20px;
            background-color: #ffff;
            box-shadow: 10;
        }
        #wrapper{
            position: relative;
            display: grid;
            grid-template-columns: 400px 100px;
            gap: 10px;
        }
        #wrapper input{
            width: 100%;
            background-color: transparent;
            color: black;
            font-size: 15px;
            border: none;
            border-bottom: 2px solid  rgb(220, 154, 233);
            padding: 10px;
        }
        #wrapper input:focus{
            outline: none;
            border-color: rgb(193, 133, 243); 
        }
        #wrapper button{
            position: relative;
            border-radius: 1px;
            border-style: solid;
            font-weight: 500;
            font-size: 15px;
            border: none;
            outline: none;
            color: #ffff;
            cursor: pointer;
            background-color: rgb(179, 90, 238);
        }
        #error{
            text-align: center;
            background-color: #ffff;
            color: red;
            margin-top: 10px;
            padding: 15px;
            border-radius: 1px solid;
            display: none;
        }
    </style>
    <div class="app">
     <div class="container">
       <div id="wrapper">
         <input type="text" placeholder="Task to be done...">
         <button id="add-btn">Add</button>
       </div>
       <div id="tasks">
         <p id="pending_task">You have <span  class=" count_value">0</span> task (s) to complete..</p>
       </div>
         <p id="error" >Input cannot be empty</p>
     </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
<scrip>
  const addbtn = document.querySelector("add-btn");
const newtask = document.querySelector("#wrapper input");
const taskcontainer = document.querySelector("tasks");
const error = document.getElementById("error");
const countValue = document.querySelector("count-value");

let taskCount = 0;

const displayCount = (taskCount) =>(
    countValue.innerText = taskcount;
);
const addTask = ()  => (
    count taskName = newTaskInput.value.trim()
    error.style.display= "none";
    if(!taskname){
        
    }
)
</scrip>
