# FOLLOW THE BLACK RABBIT
>December 27, 2022
Ref: https://hacktoria.com/collaborations/follow-the-black-rabbit/

After reading the Prologue and the briefing I downloaded the flag file and the starting information.
I took my notepad++ and saved the first note

> *password sample for flagfile*: name-of-coffee-beans-name-of-thief
> *sample password*: midnight-og-coffee-beans-jimmy

Ready to follow the rabbit!

* 1st layer: I spent my time lurking around to find useful information. At the 1st layer I found a recipe and a black-bunny text file - both of them seems to hide a lot of information. I decided to take a note and move to a little hole to the 2nd layer viewing the "suspects" and "unknown-backup" directories.

Under the "suspects folder" [R1] I found 6 interesting images about the suspected thief and another *txt* file without useful information. So I decided to move to the next hole checking the "unknown backup". 
I moved my attention to the */etc* folder containing 4 files named in some way *password*. One of them - "P455W0RD" - is filled with the following text:

> name-of-structure-contry-city

> use password for vault

Move on to the next directory - */home/UNTITLED*
I can see a new directory and a zip file both named *vault*. 

The zip file was encrypted, so I decided to search around a way to unzip it (Rememeber the note taken before few rows above. It seems we need to find a structure in some place :) )

So I moved under the /root folder and I found an interesting password.png file. 

![](https://user-images.githubusercontent.com/121463483/209887729-cd21599b-0b3d-49fc-bbfb-cc394c46ba56.png)

Using Google Lens and Google Images I quickly found the result, so I moved to Google Maps and verified the results. 

GREAT! 

I used the template and decided to move for the first attempts (upper and lower case):
* KÖLNER-DOM-DEUTSCHLAND-KÖLN
* kölner-dom-deutschland-köln

No Success. I wanted to cry but... we know that we should keep calm and be patient.

I moved again around ang went back to the *vault* folder. 

Two files without encryption:
* black-bunny-organization-card.jpeg
* secret

In the first file I found an email address blackbunny****@*****.\*\*\* with the message: "Text us with the secret!"

At the end of the "secret" file the information to be texted: 
> secret: blackrabbits4life-operation-coffee 

I sent the mail and the day after I received an email with the new instructions

## Day 2

Let me show you the email I got back

![](https://user-images.githubusercontent.com/121463483/209889055-25827328-e75d-48e4-aa5c-179849a5dfba.png)

The email says:

> G00d afternoon,
to retrieve the coffee-beans you have deposited, please proof that you are ****** by answering the following question:

![](https://user-images.githubusercontent.com/121463483/209887646-f13f28af-986d-4031-a18e-22956d92456c.png)

The-coordinates is the password for the beans in this vault: https://drive.google.com/file/d/158EIYAW1IJvYfNkFxUA92yeBGVN_jPbF/view?usp=sharing

I tried with Google Lens, Google Images and Yandex, without success. After that I used Bing and I got a clue.

![](https://user-images.githubusercontent.com/121463483/209888398-db616d06-fece-4453-a6e8-b011351e1bdb.png)

I opened the link: https://www.californiabeaches.com/map/best-beaches-youll-never-see-california/

finding the "Red White & Blue Beach". 

Using Google Earth Pro I did the match between the map and the image. The coordinates of the red cross are mine! But what kind of format I should use to unlock the beans vault?

I tried (mistakenly) the following two without success:
> 36°58'46.16"N 122° 8'50.69"O

> 36.9794896177, -122.14741415

So I moved back to the information I previously got. Well, awesome trick Mr.Midnight (https://twitter.com/MrMidnight53). If you want to hide something, paint it red.

I decided to use *"The-coordinates"* as password to unzip the beans.zip file downloaded from Google Drive

Thumbs Up! I got it. 

![](https://user-images.githubusercontent.com/121463483/209889574-90ce7586-1602-4bb6-8ac0-6df34853321d.png)

Now we need to complete the password to unlock the flagfile. We need to know who is the thief.

Going back to Step [R1] I moved back to the "suspect" directory. I took the 6 names of the images and I moved to a bruteforce attack using lowercase chars.

And the winner is... Jeff!

**Solution**

So, using the password: 

> *california-gold-coffee-beans-jeff* 

I was able to unlock the flag archive achieving the Contract Card!

Thank you Hacktoria & Mr.Midnight for a beautiful trip following the rabbit


