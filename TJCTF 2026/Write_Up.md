# TJ CTF 2026

Date: May 9, 2026

# TJCTF Challenge

## Misc Challenge

### Challenge 1

![image](https://hackmd.io/_uploads/SkEFeQU1fl.png)

- This is in my opinion is a very fun challenge
- **Investigation:**
    - We have here is an MP4 file that have bird dancing
        
        ![image](https://hackmd.io/_uploads/B1k1bmL1zg.png)
        
    - In the birb.mp4 file, we can see that there is a lot of dancing moves
        
        ![image](https://hackmd.io/_uploads/SJwZZXUJfl.png)
        
    - I think this is the `dancing man cipher`
- **Solution:**
    - I will divide the birb.mp4 file into frames using **`ffmpeg`** and then decrypt it using **`d.code`** tool
        
        ![image](https://hackmd.io/_uploads/BkXgMmUJfl.png)
        
        ![image](https://hackmd.io/_uploads/SJjxG7I1fx.png)
        
    - After having divided the frames, I arrange it into text
        
        ![image](https://hackmd.io/_uploads/BycLfQLJGg.png)
        
    - Decrypt the cipher and we receive
    
    Flag: **`tjctf{da_birb_got_some_movez}`**
        
        ![image](https://hackmd.io/_uploads/HkutGm8yGe.png)
        

### Challenge 2

![image](https://hackmd.io/_uploads/BJH4XmU1fl.png)

- **Investigation**
    - We are loaded into a game
        
        ![image](https://hackmd.io/_uploads/H1sOmXUkzx.png)
        
    - Controls:
        - Move left and right (<- and ->)
        - Jump (space)
- Solution
    - Play the game
    - Reach and pass the wall, is the flag
        
        ![image](https://hackmd.io/_uploads/HJcp7mUJGl.png)
        
    - After getting over the wall blocking you, we have the flag
    
    Flag: **`tjctf{PAST_THE_WALL}`**
        
        ![Screenshot 2026-05-17 000319](https://hackmd.io/_uploads/Byj1VmLyfe.png)
        

## OSINT

![image](https://hackmd.io/_uploads/SyFR-zv1zx.png)

- **Investigation**
    - This challenge uses your OSINT abilities
    - It is like Geoguessr game
    - There are 9 locations that need to be explored
- **Solution**
    - The locations that we find:
        - 1/9: Beer Park, Las Vegas ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=36.111926&lng=-115.172599&z=18&slat=36.112558&slng=-115.172816&sh=84.984&sp=2.302&sz=1&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 2/9: Prospect Mountain, Lake George ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=43.423896&lng=-73.745718&z=18&slat=43.423459&slng=-73.746045&sh=189.214&sp=2.697&sz=1&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 3/9: Thomas Jefferson High School for Science and Technology in Northern Virginia ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=38.818138&lng=-77.167975&z=16&slat=38.818138&slng=-77.168013&sh=299.811&sp=-11.81&sz=0.327&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 4/9: Costco Wholesale, West Ox rd ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=38.849554&lng=-77.371937&z=16&slat=38.849738&slng=-77.371099&sh=10.803&sp=-32.041&sz=0.327&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 5/9: Horne's Ferry (Official) ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=44.13547&lng=-76.353993&z=16&slat=44.135586&slng=-76.354357&sh=248.287&sp=-0.888&sz=0.327&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 6/9: Palmyra Atoll National Wildlife Reef ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=5.88514&lng=-162.066421&z=16&slat=5.884583&slng=-162.060638&sh=-87.952&sp=-27.407&sz=0.327&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 7/9: Le Portail, Den Den, Tunisia ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=36.821974&lng=10.104141&z=18&slat=36.821974&slng=10.104141&sh=349.138&sp=0&sz=1&gm=0&panel=msbi&mi=1&be=0&pc=1))
        - 8/9: RN8, Madagascar ([Link](https://www.google.com/maps/@-20.1493558,44.5014063,2a,75y,70.26h,78.12t/data=!3m10!1e1!3m8!1sVPeWsd1M6cKa7w12GJzwLg!2e0!6shttps:%2F%2Fstreetviewpixels-pa.googleapis.com%2Fv1%2Fthumbnail%3Fcb_client%3Dmaps_sv.tactile%26w%3D900%26h%3D600%26pitch%3D11.882465029771993%26panoid%3DVPeWsd1M6cKa7w12GJzwLg%26yaw%3D70.2628586882619!7i13312!8i6656!9m2!1b1!2i38?entry=ttu&g_ep=EgoyMDI2MDUxMy4wIKXMDSoASAFQAw%3D%3D%5C))
        - 9/9: Kawahigashi Park, Uji, Kyoto, Japan ([Link](https://data.mapchannels.com/dualmaps9/map.htm?lat=34.894023&lng=135.810683&z=11&slat=34.893956&slng=135.81081&sh=1.836&sp=-7.97&sz=1&gm=0&panel=msbi&mi=1&be=0&pc=1))
    - After having founded all the locations above, the game will end and you will receive the flag
        
        ![image](https://hackmd.io/_uploads/BJFF4zDJzx.png)
        

Flag: **`tjctf{y0u_ar3_a_g30gu3ssr_g0d!}`**
