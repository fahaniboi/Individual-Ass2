# Individual-Ass2
 
![Rep is Public and has Unity Gitignore](https://user-images.githubusercontent.com/72412425/228298465-f1440dee-8c0d-4024-9bbc-33e494c2d588.png)
The Repository has been published as public and it has a unity gitignore. 


![Empty ](https://user-images.githubusercontent.com/72412425/228298993-353dbb24-393d-4eb1-a782-61e01483ab64.png)
Created an empty 3D Unity Project 

![Build Release](https://user-images.githubusercontent.com/72412425/228300350-f2225b47-5c7f-40d6-bde9-ec849bfc669b.png)
The Build has been created and Released in GitHub

Forward Rendering is the usual type of rendering technique that most engines use. Forward rendering starts with supplying the graphics card to the geometry which then gets projected and broken down to vertices, then it gets transformed or split into fragments, which then gets rendered and then passed onto the screen.

Deffered Rendering is when the rendering is deffered a little bit until all of the geometries have been passed down the pipe. The final image is then made by applying the shading at the end. 


My student number ends with an odd number. 
![Toon Water](https://user-images.githubusercontent.com/72412425/228310081-d6eace47-15e9-4a92-8758-325ec72d3053.png)
Added the Toon shader to the Water shader to make a toon like water. Added a low poly boat mesh that i found on the asset store to act like that boat that is shown in the pdf. The water shader I used was from the lecture as well as the Toon shader. I combined both shaders to have a Toon like Water shader which i then added to a plane object. 

I combined the two shaders by copying the LightingToonRamp function from the ToonRamp shader we made in class and pasted it into the water shader that was also made in class. I then added a custom made toon texture and applied it to the disignated texture spot in the material.

![Screenshot 2023-03-29 103650](https://user-images.githubusercontent.com/72412425/228573793-555e9d95-e3fc-430e-aaa1-d611abcbeb9c.png)

The code takes an input image (RenderTexture Source) and generates a series of lower resolution versions of it. The variable "integerRange" specifies the amount by whihc the resolution is reduced at each step, and specifies how many steps are needed. It then applies a "Blit" operation, which is a type of image processing operation, to copy the input image to the currentDestination. The resulting tecture is then used as the input to the next iteration of the downsampling process. The code uses an array of RenderTextures "Textures" to store the results and then a new RenderTexture "currentDestination" is created to store the downscaled image. If the height scales beloew 2 pixels the downsampling process is stopped. After the downsampling is complete, the code generates a series of higher-resolution vaersions of the image. It does this by applying a "Blit" operation to each texture in the "textures" array, copying the results to the hnext higher resolution texture in the array. The highest resolution texture is copied to the ouput imageimage, the RenderTexture destination using another Blit operation. 
 

