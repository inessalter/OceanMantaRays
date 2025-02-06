# OceanMantaRays
Project for Ocean Manta Rays


 Ishita Gupta and Ines Salter
Manta Arrival to the Village of Fish
Google Drive Link to Submission
Inspiration
We were reading Playground, which inspired us to think of the ocean as a potential source for this project, reflecting photos under the ocean, showing the biodiversity under water and how the light can illuminate all which we cannot see. Additionally, Ishita has done a lot of freediving and so for her it’s particularly moving to be able to represent the underwater world in blender.

Rendering our Final Image from a different angle and without textures:
We rendered two images without textures, one with the ocean still and one without so that the differences were clear. The last image, which has no textures, still has a blue tone because of the volumetric applied to it.
1. Main Geometry from Scratch
   
 We modeled the corals and manta rays entirely from scratch. The manta rays were carefully sculpted to capture their natural elegance, and the corals were designed with organic shapes to add realism to the underwater environment.
2. UV Mapping and Texturing from Scratch
We created custom textures and materials to enhance the realism of our scene:
● Manta Ray Wave Texture: To simulate water caustics, we manually unwrapped the manta ray for proper UV mapping. The texture was procedurally generated using Blender's Wave Texture nodes and Mapping tools, resulting in a dynamic, caustic-like appearance that integrates seamlessly with the underwater environment.
● Coral Material with BRDF Shading: For the coral, we applied a custom BRDF-based material to simulate realistic light scattering and reflection. Using Blender’s Principled BSDF shader, we incorporated procedural noise textures to add surface detail and variation, making the corals appear more organic and lifelike.
● Fish Textures and BRDF Shading: We manually unwrapped and textured the fish using a custom UV wrap. This wrap was generated with the assistance of ChatGPT (to get the specific images for the textures - which is allowed according to the handout) and applied with precision to ensure the texture fit the geometry seamlessly.
● Water: For the surface of the water, we created a water surface texture. Shading Texture Images:
By combining these techniques, we achieved visually compelling textures that enhance the underwater scene’s depth and realism.
  
   Manta texturing Nodes
Fish Shader Editor 
Corals Shader Editor
 We really tried to create the coral texture with the porous attribute, however because the corals was so fractal, it caused our Blender to crash. However, we wanted to add it here so that you can see our attempt at the coral texture.
Source: https://www.youtube.com/watch?v=A-jTsmo1wok&ab_channel=3derrorist
   
  3. Blender/Cycles Advanced Features
To add depth and realism to our scene, we utilized the following advanced features in Blender Cycles:
● Volumetric Water:The water was created using volumetrics, giving it a realistic sense of depth and atmospheric scattering. This technique allowed us to replicate the natural murkiness and light diffusion commonly seen in underwater environments.
● Realistic Lighting with HDRI:We incorporated a cloudy sky HDRI to create realistic, diffused lighting. This was complemented with additional light sources to illuminate key parts of the scene, such as the manta rays and corals. Strategic lighting highlights areas of interest and adds visual appeal.
 
  Playing with Lighting:

  We also tried with different lighting to see which one represented our image best. We tried many different area lights from many perspectives, and played around with the color of the lights. In the end, what worked best was adding a partly cloudy sky HDRI, which caused realistic cloud lighting.
Work Distribution
● Ishita:
Ishita focused on the 3D modeling of the manta ray and corals, ensuring their shapes were
natural and lifelike. She also worked on the volumetric water to simulate the depth and atmosphere of the underwater environment, which was particularly challenging due to its complex light scattering and rendering requirements. Additionally, Ishita handled the underwater lighting, strategically placing light sources to illuminate key areas of the scene and highlight the textures and geometry.
● Ines:
Ines took charge of the texturing and UV mapping for the scene. She created and applied custom textures, including:
○ The wave-like pattern for the manta ray to simulate caustics and wave shader editor texture properties, for the manta ray.

○ The detailed fish skin texture, ensuring seamless wrapping using custom UV maps. Also, fish positioning, rotations, scaling etc.
○ The coral textures, which incorporated surface variation and shading to enhance realism.Ines’ careful work on UV unwrapping and procedural textures brought the models to life and ensured that the materials aligned perfectly with the geometry.
Sources
Manta Modeling: https://www.youtube.com/watch?v=3AxlR8nSDgU Water Volumetrics: https://www.youtube.com/watch?v=xvgOTeJXKII Inspiration for Corals: https://www.youtube.com/watch?v=zTLty_Mfqnw Partly Cloudy Sky HDRI: Uploaded to Google Drive
Previous Project Proposal:
In our project, we will use ray tracing and volumetric (Blender/Cycles advanced feature) to create a realistic underwater environment. Ray tracing will allow us to accurately simulate how sunlight enters the water, refracts, and reflects off various objects like coral and the manta ray, creating natural highlights and shadows. This technique will enable us to capture realistic caustics—patterns of light on the ocean floor—and the subtle interplay of light as it passes through the water. Additionally, we’ll apply volumetrics to the water material to mimic the slight haze and light scattering seen underwater, adding depth and creating a gradual fading effect as objects move further from the viewer. Together, ray tracing and volumetric will give our scene a lifelike, immersive quality, enhancing the realism of the underwater atmosphere.
Manta ray skin has a slightly smooth and sometimes shiny texture due to its streamlined body for gliding through water. By adjusting specularity and roughness in the shader, we can create a finish that reflects light subtly, mimicking how real skin would look underwater.
Real manta ray skin, like human skin, has slight translucency. Adding subsurface scattering gives a soft look where light penetrates slightly into the surface before reflecting out, which can add a sense of depth and realism.
We will also wrap our Manta Ray with UV mapping to simulate the patterns on its skin and better represent the lighting on it. We will also try to use UV wrappers on the coral surfaces if it looks good.
We will also make a custom coral shader, if time permits!
