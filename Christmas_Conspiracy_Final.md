


> A Christmas Conspiracy
December 26, 2022
Ref: https://hacktoria.com/collaborations/a-christmas-conspiracy/

After reading the Prologue and the brief I moved my attention to the whatsapp screenshots (and in particular to the last one)

![](https://hacktoria.com/wp-content/uploads/2022/12/convo-4.png)  

I tried few OCR scan tools to automatically read the link without success, so I decided to manually write it down.

The link is: ZTGIS://YHW.XJSHBBQ.CQX/SWD/JG/1Y9AWEOQ4UP2WUT4V6H82/A?DN=0&CLEWC=N1BHW4UVEWTB6NZPGWW9PRL9H

First things I saw:
* semi colon, dot and slash
* ZTGIS really similar to https
* YHW ?-> WWW
* CQX ?-> COM

The encoding is not "static" (Caesar style) but something that can map the same char to different chars. I tried using cyberchef (magic function) without success so I moved to my knowledge and I decided to try with oldest ciphers . So, I said "let me try with Vigenère". After a quick search on google I found this useful site:

> https://asecuritysite.com/coding/vigcalc2

I filled out the fields as below:
* sentence: ZTGIS
* KEY: HTTPS

I clicked on **Analyze** and the Christmas magic showed me the word: **SANTA**

Quickly I fill out the fields with the right values moving first to "santaclaus" as key but I received an error. So I tried to identify the next char to match the ".com". The final working Key was "santaclause" and I found the decoded link: 
> https://www.dropbox.com/scl/fo/1y9ndemf4uv2eqb4v6u82/h?dl=0&rlkey=v1bud4uttwzj6jhptdw9ngl9n

(Just to be honest, I got an error because I tried the uppercase version of the link. After few checks, I moved to fully lowercase and I got the right folder to download)  

I downloaded the folder and after laughing (Thank you Infosec United) I read the plan and tried to geolocalize the image as requested. 


First thing first: **open google maps and move to the coordinates**

Using the coordinates from Step 1 and step 3 I understood where to search: **Antarctic region**. The red roof used for container and buildings of researchers is a good clue. I tried with Google Lens, Google Images and Yandex, without success. I moved to Google earth and Google maps harvesting all around (a lot near Machu Picchu base). 
There are a lot of similar results but not the right one :) 

Any Osint-er should keep calm and be patient

After that I checked on Google for the list of Researchers base and tried searching for them (by name) in Google Maps. Finally, near the places I moved before, I found "Carlini Base" aka Jubany. And it matched.

**Solution**
>https://goo.gl/maps/B8R5NkgaPjK8Z5ba7