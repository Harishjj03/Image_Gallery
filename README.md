# Ex.08 Design of Interactive Image Gallery

# Date : 09-11-2025

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
gallery.html:
<html>
<head>
    <title>Image Gallery</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
</head>

<body>
<div>
    <h1 class="titlebar">Image Gallery</h1>
    <div class="container">

        <div>
            <img src="Ajith.jpg" onclick="openModal(this)">
            <h2>AJITH KUMAR</h2>
        </div>

        <div>
            <img src="shane.avif" onclick="openModal(this)">
            <h2>SHANE NIGAM</h2>
        </div>

        <div>
            <img src="dq.jpg" onclick="openModal(this)">
            <h2>DULQUER SALMAN</h2>
        </div>

        <div>
            <img src="pranav.jpg" onclick="openModal(this)">
            <h2>PRANAV</h2>
        </div>

        <div>
            <img src="sandeep.avif" onclick="openModal(this)">
            <h2>SANDEEP</h2>
        </div>

        <div>
            <img src="kp.jpg" onclick="openModal(this)">
            <h2>KALYANI 
                PRIYADHARSHAN</h2>
        </div>

        <div>
            <img src="RS.webp" onclick="openModal(this)">
            <h2>REVATHY
                 SARMA</h2>
        </div>

        <div>
            <img src="mb.avif" onclick="openModal(this)">
            <h2>MAMITHA BAIJU</h2>
        </div>

        <div>
            <img src="rv.avif" onclick="openModal(this)">
            <h2>RUKMANI VASANTH</h2>
        </div>

        <div>
            <img src="Malavika.jpg" onclick="openModal(this)">
            <h2>MALAVIKA MANOJ</h2>
        </div>

    </div>

    
</div>

<script>
function openModal(imageElement) {
    const imageSrc = imageElement.src;

    const width = 900;
    const height = 600;
    const left = (screen.width / 2) - (width / 2);
    const top = (screen.height / 2) - (height / 2);

    const newWindow = window.open(
        '',
        '_blank',
        `width=${width},height=${height},top=${top},left=${left}`
    );

    newWindow.document.write(`
        <html>
        <body style="margin:0; background:black; display:flex; justify-content:center; align-items:center; height:100vh;">
            <button onclick="window.close()" style="position:absolute; top:10px; right:15px; font-size:24px; color:white; background:none; border:none; cursor:pointer;">×</button>
            <img src="${imageSrc}" style="max-width:90%; max-height:90%;">
        </body>
        </html>
    `);
}
</script>

 
</body>
</html>

style.css:
*{
    margin: 0px;
    padding: 0px;
}

body{
font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
  background-color: darkmagenta;
  font-size: large;


}

.titlebar{
    color: white;
    text-align: center;
    padding: 10px;
    margin-bottom: 30px;
    font-weight: bold;
    letter-spacing: 2px;
    margin-top: 10px;
    
}

.container{
display: flex;

flex-wrap: wrap;
justify-content: space-around;
  display: grid;
  grid-template-columns: repeat(5, 1fr); 
  gap: 20px; 

   padding: 20px 40px; 
  margin: 0 auto; 
  max-width: 1300px; 
}






.container img:hover {
  transform: scale(1.05);
}


 .container img {
  width: 180px;              
  height: 270px;            
  object-fit: cover;       
  background-color: white;   
  border: 3px solid white;
  border-radius: 10px;
  transition: transform 0.3s ease;
  box-sizing: border-box;
  flex-grow: 1;
 
}

.container h2 {
  
  margin-top: 8px;        
  font-size: 14px;
  color: white;            
  font-weight: 900;
  letter-spacing: 0.5px;
   margin-bottom: 20px;
}


 
 


 


```

## OUTPUT
![alt text](<Screenshot 2025-11-09 220901.png>)
![alt text](<Screenshot 2025-11-09 221033.png>)
![alt text](<Screenshot 2025-11-09 221830.png>)


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
