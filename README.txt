Switched to grasshopper after having some basic issues in openframeworks. 

I tried some different plugins, but couldn't successfully get katakana characters in openframeworks. 

Recreating this poster is relatively simple. Each letter is repeated along a for loop. The center of each character is roughly the center of the character's bounding box. 

Three transformations occur as part of the for loop. 

Firstly, the characters are translated in the y axis, creating the trail effect below the title characters. 

Secondly, the characters undulate according to a sine wave function. Two options could create this effect. Either the characters could rotate about the y axis, or the  characters could scale non-uniformly about the x axis. I wanted to try the rotation since I hadn't done anything 3D in openframeworks, but I was finding that when I added ofRotateDeg(...) into a for loop, my debugging window would crash. 

Finally, the characters were scaling from full size at the top of the page, to zero at the bottom. 


In grasshopper, I mapped these three functions to one slider, and played with the frequency of the sine wave until I matched the original poster. 

