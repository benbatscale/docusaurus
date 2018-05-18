---
id    : lidar
title : LiDAR Best Practices
---

## Dynamic Tracks (Moving Objects)
1. Find the **Best Frame** where object is **clearest** and **densest**.   
    a. *Activate GROUND.*  
    b. *Include all LiDAR points inside cuboid and tighten.*

2. Check for **Missing Frames** & **Complete Pathway**   
    a. *Add a frame for **first** and **last** frame the object appears in.*    
    b. *Add any necessary frames for anything in between.*  

3. Use **Interpolation**  
    a. *Always include **first**, **last**, and **densest** frame.*    
    b. *Delete unnecessary frames, leaving only important ones for general pathway.*   
    c. *If pathway is curved, start by using frames by 5ths. (1, 6, 11, 16, 21, 26, etc.)*   

4. **Correct Bottom of Cuboid** (z-index)  
    a. *Activate GROUND.*    
    b. *Go through each frame and adjust z-Index to sit right on top of GROUND.*  
    c. *Check Top, Back & Side Views in each frame.*

5. **Directional Heading**  
    a. *Use TOP DOWN VIEW.*  
    b. *Create a smooth pathway by going through each frame correcting directional heading.*  
    c. *Add as many frames needed to ensure pathway is smooth and correct.*  

6. **Double Check**   
    a. *Go through steps 1 - 5 again.*  
    b. *Use Top Down View*  
    c. *Make adjustments for directional heading of each frame, using wasd and arrow keys.*   
    d. *The goal is for each cuboid to line up end to end with the one before and after it.* 

7. **Final Check**  
    a. *Use Overhead View.*  
    b. *Confirm that cuboid is aligned properly and facing in the direction it is moving.*  

## Quick Method for No Label Zone
1. *Delete No Label Zone.* 
2. *Draw a new box but DO NOT MARK stationary.*  
3. *Edit as necessary.*  
4. *When editing is finished, MARK stationary.*  
