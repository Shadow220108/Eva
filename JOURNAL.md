<div align="center">
  <h1>Eva</h1>
  <h3>By Shadow</h3>
  <h3>Total Time Spent : 12.1 Hours </h3>
</div>

--- 

### Journal #1 Starting with the project 
Time spent : 1.2 hours   

  
Starting my first project for Expedition Ireland, I wanted to make something whimsical and something which I can gift my friend! While looking for different projects 
I found the tutorial on PCB hacker cards and thought it would be perfect, then I started experimenting and playing around the design which I want.  
I used excalidraw to come up with a sample  
  

<div align="center">
  
| design|
| --- |
| <img width="501" height="457" alt="image" src="https://github.com/user-attachments/assets/06e56a28-6684-41db-a3a7-628374f2581b" /> |

</div>


  I am planning to have LEDs on the stars and have all the circuitry on the back :D  


--- 

### Journal #2 Schematics design!  
Time spent : 1 hour   

  
I started with the schematics following the tutorial on jam hacker card, since this is my first time using EasyEDA, it was quite confusing to figure out, none the less
the tutorial was great and guided me through most of the stuff 
  

<div align="center">
  
| EasyEDA Schematics|
| --- |
| <img width="493" height="493" alt="image" src="https://github.com/user-attachments/assets/cb146d87-804a-44e7-af96-e254830ee8cf" /> |

</div>



--- 

### Journal #3  Going back to KiCAD!  
Time spent : 2.2 hour   

  
After being done with the schematics, I started with the PCB and since I was used to KiCAD, it really confused me and took a bit of time to figure out the shortcuts, 
then I decided to switch back to KiCAD, since I am already familiar with it and it would be a bit easy for me to get the project done in KiCAD
  

<div align="center">
  
| KiCAD Schematics |
| --- |
| <img width="680" height="437" alt="Screenshot 2026-09-30 160704" src="https://github.com/user-attachments/assets/86502bad-0248-49f0-ad77-6d602fee69d5" />  |

</div>

I started the schematics in KiCAD from scratch, starting with importing the footprints for the nfc card, I used easyeda2kicad library ( this is a great library to get anything 
in KiCAD from lcsc or EasyEDA ) 

I wired up everything the same way as it was in the tutorial, in additional I added 4 testpoints for the hacker card to be customizable through I2C communication in future! 

--- 

### Journal #4  Footprints Time!  
Time spent : 1.6 hour   

  
Since I used easyeda2kicad library, it already came with the footprint for the NFC tag, and since I am going to use PCBA for the assembly, I used 0603 for the passives! Main hurdle 
was to find a suitable footprint for the antenna! I tried looking around trying to make my own but then found out its not reliable and not a recommended way! After that after researching for a bit 
I found an online NFC antenna generator! 
  

<div align="center">
  
| NFC Generator |
| --- |
| <img src="https://github.com/user-attachments/assets/a1703431-c934-473b-8e0e-b2d62cdae100" /> |

</div>
At starting I did not understand most of the stuff which I was doing, and what parameters I am messing with, after researching a bit more about NFC I got to know some stuff and came up with a circular 
antenna to match my design, I exported it as KiCAD footprint and them imported to my PCB :D   

--- 


### Journal #5  PCB Routing!  
Time spent : 1 hour   

After importing the footprint, I placed all the components and started routing everything! The antenna had a 5x5mm clearance zone which prevented me to place anything near it! Since I want my board to be pretty
compact, I got rid of the clearance zone and routed everything!  

<div align="center">
  
| PCB |
| --- |
| <img width="900" height="657" alt="Screenshot 2026-09-29 171643" src="https://github.com/user-attachments/assets/c8f5ebfd-ecaf-4645-97da-3355b180f6a3" /> |

| PCB Routed |
| --- |
| <img width="702" height="732" alt="Screenshot 2026-09-29 180015" src="https://github.com/user-attachments/assets/bc556ad1-aa77-49a9-bfcf-d123a1debb59" />  |

</div>

--- 

### Journal #6  Changes in design!  
Time spent : 1 hour   

  
Changes in plan I decided to switch from a circle shape to a heart shape to make it look more pretty and cute! I imported a heart geometry as the edge cut, scaled it to size, placed the components
again and routed everything

<div align="center">
  
| Heart Shaped PCB |
| --- |
| <img width="523" height="441" alt="Screenshot 2026-09-29 182527" src="https://github.com/user-attachments/assets/34b60f30-a919-44de-9236-5c6578b07ae1" /> |

This did not take long since I already routed it once :D

</div>

--- 
### Journal #7 Editing the footprints of the test points! 
Time spent : 0.8 hour   

The test points which I added for further I2C communication allowing me to flash the NFC chip without using an active NFC reader. had a square footprint, which works well
but does not match the design and has unnecessary stuff

<div align="center">
  
| Old Footprint |
| --- |
| <img width="560" height="340" alt="Screenshot 2026-09-29 185625" src="https://github.com/user-attachments/assets/9a0033ef-5a04-4989-ae87-3ae0beb7b144" /> |


I decided to edit the footprints myself and have them in a circular shape, for this I used the KiCAD's default footprint editor and changed the shape and dimensions! I also 
went ahead and added my own silkscreen text to go with footprint for me to identify the test points individually!  
| New Footprint |
| --- |
| <img width="453" height="370" alt="Screenshot 2026-09-30 021622" src="https://github.com/user-attachments/assets/39474da4-f812-49c3-8626-ea436b01ac14" />|
</div>  

--- 
### Journal #8 Adding a keyring! 
Time spent : 0.3 hour   

This heart shaped PCB missed a hole for keychains, so I decided to add one, I came up with a simple design in Canva imported it in KiCAD and used a mounting hole to have it as a hole :D
<div align="center">
  
| Keyring |
| --- |
|<img width="366" height="298" alt="Screenshot 2026-09-30 162351" src="https://github.com/user-attachments/assets/0d5598fe-ba73-4534-b6b1-1046b19604fa" /> |
| <img width="430" height="360" alt="Screenshot 2026-09-30 164302" src="https://github.com/user-attachments/assets/56363e95-9561-4930-8ac5-51bc9b4fd2df" /> |
</div>

### Journal #9 Doing Art! 
Time spent : 2.3 hour   

Here comes my fav part in designing the PCBs adding art to them! Since I want this to be as whimsical as possible, I went around made some custom designs, used pinterest for 
some and added as much of art as I could on my PCB. I also made a spinning render for my PCB which I will have in the readme :D 
<div align="center">
  
| Render |
| --- |
| <img width="513" height="401" alt="Screenshot 2026-09-30 164040" src="https://github.com/user-attachments/assets/d3fc2342-aec2-476b-b743-5945d02e2340" /> |
| <img width="398" height="411" alt="Screenshot 2026-09-30 164053" src="https://github.com/user-attachments/assets/32637b47-b2e6-4b9f-b081-3a180802ff97" /> |
</div>

### Journal #10 BOM and Github! 
Time spent : 0.7 hour   

Finishing up with the project, I uploaded the files to JLCPCB to get a quote, and started writing the readme and organising files to upload to the Github, this would be the final
journal and if you are reading by here, thank you :D
<div align="center">
  
| Readme |
| --- |
| <img width="1521" height="732" alt="Screenshot 2026-10-14 131947" src="https://github.com/user-attachments/assets/510941a6-f0b9-4bee-9728-ba1a142b9eb1" /> |

</div>
