# Ex04 Places Around Me
## Date: 07.04.2024

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
### imagemap.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jai Pradhiksha</title>
</head>
<script>
    function coord(event) {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("txt1").value = x;
        document.getElementById("txt2").value = y;
    }
</script>

<body>
    <img src="entertainmentmap.png" width="1000px" usemap="#MapNew" onmousemove="coord(event)">
    <MAP name="MapNew">
        <AREA shape="RECT" coords="39,122,180,156" href="http://www.madrasraceclub.com/" title="Madras Race Club">
        <AREA shape="RECT" coords="64,364,200,400" href="https://www.phoenixmarketcity.com/chennai/brand/Funcity/1491"
            title="Phoenix Fun City">
        <AREA shape="RECT" coords="356,178,497,220"
            href="https://www.tripadvisor.in/Attraction_Review-g304556-d325388-Reviews-Guindy_Snake_Park-Chennai_Madras_Chennai_District_Tamil_Nadu.html"
            title="Chennai Snake Park">
        <AREA shape="RECT" coords="306,76,452,114" href="https://tnstc.gov.in/bm-birla-planetarium.html" title="BM Birla Planetarium">
        <AREA shape="RECT" coords="574,211,703,243" href="http://www.kartwheel.in/" title="Kartwheel - Kids Play & Party zone">
        <AREA shape="RECT" coords="600,437,707,469" href="https://www.thecompanycheck.com/org/magic-carpet-fun-zone/e64faac62a"
            title="Magic Carpet Fun zone">
        <AREA shape="RECT" coords="803,190,980,240" href="https://nassaa.in/" title="Nassaa Uth Hub">
    </MAP>
    <br>
    X coord : <input type="text" name="" id="txt1"> <br>
    Y coord : <input type="text" name="" id="txt2">
</body>

</html>
```

## OUTPUT
![image](https://github.com/Jai-Pradhiksha/NearMe/assets/100289733/19190f82-ccb9-4f23-8dd5-8106f5115c0f)




## RESULT
The program for implementing image maps using HTML is executed successfully.
