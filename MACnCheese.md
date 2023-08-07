## Deconstruct CTF 2023
Category : OSINT<br>
Points : 500<br>
Flag : `dsc{30:89:D3:2E:04:22}`<br>
Description : `Well mr.ramen told me to get some information about the cctv camera in some market but neither did he gave me clear instructions for the market nor did he gave me clarity on what was the information needed. He just gave me a link and said trust me you can do find it :/`

For this challenge, the author talks about a cctv camera and also about a market.<br>
He also provides a github link here : https://github.com/Mayhul-Jindal/.<br>
From this github link on this repo : https://github.com/Mayhul-Jindal/buriOS.<br>
We can find in /img subfolder a commit which says : "added this here by mistake lol" then by downloading the [image here](https://raw.githubusercontent.com/Mayhul-Jindal/buriOS/4d6492a87256049955d71c5ca9b19f71bb4e2f1d/img/Screenshot%202022-07-10%20004259.png)<br>
We can see it's a cctv camera by simply doing google reverse image search, we find the exact camera live on youtube [here](https://www.youtube.com/watch?v=wuC8wRvXock).<br>
Now we know that the camera is it Kyoto at the Nishiki Market so by simply using google map, we [find it](https://www.google.fr/maps/place/Nishiki+Market/@35.0049247,135.7648196,17z/data=!4m6!3m5!1s0x6001089ccd8ccb4f:0xb69ea31001ec6c9c!8m2!3d35.0050258!4d135.764723!16s%2Fm%2F03d6_6p?entry=ttu)<br>
Then by searching in the different streets and watching the picture we find back the camera at [this location](https://www.google.fr/maps/@35.0049961,135.7649165,3a,75y,63.9h,107.68t/data=!3m6!1e1!3m4!1sjmCcyLcWAsZ9nk05PI-wKg!2e0!7i16384!8i8192?entry=ttu)<br>
So finally we spot on the map : ![here](https://ibb.co/zbLsR76) and we have exact latitude and longititude so we go on [Wigle](https://wigle.net/) create an account, enter latitude and longitude and get the MAC address of the webcam on the [map](https://ibb.co/QJLvVcV) which is `30:89:D3:2E:04:22 -> GlocalNet_0UTSJD`.<br>
