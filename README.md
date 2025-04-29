# Ex03 Time Table
## Date:29/04/2025

## AIM
To write a html webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create a static folder and inert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html.

### STEP 4
Add header row using ```<th>``` tag.

### STEP 5
Add your timetable using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
timetable.html
```
<!DOCTYPE html>
<html lang="eng">
<head>
    

    <link rel="stylesheet" href="styling.css">
    <title>Prime Batch Table</title>
</head>
<body align="center">
    <img src="logo.png" alt="Image" class="img">
    <table class="t1">
        <caption class="TT" style="font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;">Prime Batch TT</caption>
        <thead>
            <tr class="Ch">
                <th style="background-color: pink;">DAY</th>
                <th>8AM-10AM</th>
                <th>10AM-12PM</th>
                <th>LUNCH(12PM-1PM)</th>
                <th>1PM-3PM</th>
            </tr>
        </thead>
        <tbody>
                <tr >
                    <th>MONDAY</td>
                    <td>Python Programming</td>
                    <td>Assesent Hour</td>
                    <td class ="lunch" rowspan="5" style="background-color: antiquewhite;">
                        L <br> 
                        U <br>
                        N <br>
                        C <br>
                        H
                    </td>
                    <td>Machine Learning</td>
                </tr>
                <tr >
                    <th>TUESDAY</td>
                    <td>Module Completion</td>
                    <td>Data Science</td>
                    <td>Advance C Programming</td>
                </tr>
                <tr >
                    <th>WEDNESDAY</td>
                    <td>Task Completion</td>
                    <td>Data Science</td>
                    <th style="background-color: cyan;">Mentor Meet</td>
                </tr>
                <tr >
                    <th>THURSDAY</td>
                    <td>Assesment Hour</td>
                    <td>Advance C Programming</td>
                    <td>Machine Learning</td>
                </tr>
                <tr >
                    <th>FRIDAY</td>
                    <td>Data Science</td>
                    <td>Python Programming</td>
                    <td>Module Completion</td>
                </tr>
                <tr>
                    <th>SATURDAY</td>
                    <th colspan="4" style="background-color: rgb(210, 166, 227) ; font-size: large;">Module Assesment Completion</th>
                </tr>
        </tbody>

    </table>
    
</body>
</html>

```
styling.css
```
body {
    display: flex;
    flex-direction: column;
    justify-content: center; 
    align-items: center;  
    height: 100vh; 
    margin: 0; 
    padding-top: 4px;
    background: url('image.png') no-repeat center center fixed; 
    background-size: 50%; 
}

body::before {
    content: ""; 
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: inherit; 
    filter: blur(10px); 
    z-index: -1; 
}

.TT{
    color : rgb(0, 0, 0);
    caption-side:top;
    text-align:center;
    font-weight:bold;
    font-size: 40px;
    font-family: 'Arial', sans-serif;
    transition: transform 0.4s ease-in-out,color 0.4s ease-in-out;
}

.TT:hover{
    transform: scale(1.1);
    color: rgb(38, 0, 255);
}

.t1{
    margin: auto;
    width:80%;
    text-align:center;
    border: 5px solid black;
    transition: transform 1s ease-in-out;
}

.t1:hover{
    transform: scale(1.1);
}

.t1 th,.t1 td{
    border: 2px solid black;
    padding : 15px;
    position: relative;
}

.t1 th{
    background-color: rgb(178, 255, 255);
    font-size: medium;
    transition-duration: .4s;
}
.Ch th{
    background-color: rgb(255, 172, 242) ;
}

.t1 td{
    
    background-color: rgb(245, 203, 203);
    
}

.lunch{
    font-weight: 700;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    font-size: x-large;
}



.t1 td:hover{
    background-color: rgb(238,248,238); 
    transform: scale(0.90); 
    transition: background-color 0.4s ease-in-out, transform 0.4s ease-in-out; 
}

.t1 th:hover {
    background-color: rgb(94, 238, 94); 
    transform: scale(0.90); 
    transition: background-color 0.4s ease-in-out, transform 0.4s ease-in-out; 
}

.img {
    display: block; 
    margin-bottom: 5px; 
    width: auto; 
    max-width: 70%; 
    transition: transform 1s ease-in-out;
}

.img:hover {
    transform: scale(1.1); 
}

```

## OUTPUT
![alt text](<Screenshot (6).png>)

## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
