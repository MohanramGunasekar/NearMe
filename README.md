# Ex04 Places Around Me
## Date: 12-04-2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    *{ margin: 0;}
</style>
<script>
    function coordinate(event) {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("text1").value = x;
        document.getElementById("text2").value = y;

    }
</script>

<body>
    <IMG src="maps.png" width="1000" height="500"
    usemap="#MapNew" onmousemove="coordinate(event)">
      <MAP name="MapNew">
        <AREA shape="RECT" coords="624,148,736,209" href="https://www.ucla.edu/" title="University of California,Los Angeles">
        <AREA shape="RECT" coords="760,215,856,277" href="https://www.usc.edu/" title="University of Southern California">
        <AREA shape="RECT" coords="182,45,292,65" href="https://www.calstate.edu/" title="California State University">
      </MAP>
      <br>
    X-coordinate
    <input type="text" id="text1">
    <br>
    <br>
    Y-coordinate
    <input type="text" id="text2">
</body>
</html>
```

## OUTPUT



![Screenshot 2024-04-27 111715](https://github.com/MohanramGunasekar/NearMe/assets/139841812/0a0bd904-d6dc-4e3d-a7fe-32241497dd56)




## RESULT
The program for implementing image maps using HTML is executed successfully.
