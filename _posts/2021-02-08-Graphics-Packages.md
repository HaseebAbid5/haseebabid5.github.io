---
layout: post
title: Graphics Packages
subtitle: Prototype or Final?
tags: [Pokemon Clone, Graphics, Art, PS1, PlayStation 1, Packages]
comments: true
---

The post for today will be a short one going over the graphical packages I am using for this game. A lot of people may have some reservations about using graphic assets in a final full game, but I am much more open to the idea. I am a programmer. I have dabbled with a couple of 3D modeling software, pixel art software, texturing software, and have even tried my hand at 3D and 2D animation. I am not good at any of these things. I am also not at a place in my life where I would want to dedicate hundreds, if not thousands, of hours trying to perfect my hand at these skills. I just want to develop a game. I have often heard the term "play to your strengths" and my strength is programming. Not to mention the double standard where if an artist just uses a script or system developed by someone else, they don't have to think twice about it. I would argue rightfully so, but that should also mean that there should be no shame on people using art from others in their product, as long as they have permission of course. 

For the purposes of this Pokemon Clone title I am currently developing, I have used a number of graphical packages to kickstart my development. I do plan on using these assets in the final version of the game, unless I can secure some funding to hire an artist which is a path I would highly prefer to go down instead. But, at least for now, I am very happy with the results I can get with what I have.

## Low-Poly Ultimate Pack

For the roads, trees, buildings, and most environmental assets I am using the [Low Poly Ultimate Pack by polyperfect](https://assetstore.unity.com/packages/3d/props/low-poly-ultimate-pack-54733).

![LowPolyUltimatePack](https://assetstorev1-prd-cdn.unity3d.com/key-image/4b30d9fd-3db5-41c4-adce-15710ec40ba5.webp){: .mx-auto.d-block :}

This package is of a very good value. For just $50 you can have access to graphics for a large variety of environments. It includes everything from buildings, nature assets, props, and even people. It does also include materials, and combines the model + material to have prefabs for every object within the package. The low-poly style plus the use of a texture atlas instead of separate texture for each colour makes this package very optimized as well right out of the box. The low-poly style also works really well with my PlayStation 1 art style target.

## Cute Low-Poly Animals Super Pack

[This is the package](https://assetstore.unity.com/packages/3d/characters/animals/cute-low-poly-animals-super-pack-118520) that I will be using as a base for creating my "Pokemon". Again, the low-poly models work great with my PS1 target, and for $10 getting a ton of rigged and animated animals is just a really good deal. 

![Low-PolyCuteAnimals](https://assetstorev1-prd-cdn.unity3d.com/key-image/df75bb67-10d0-4244-bd75-b5d956cd5815.webp){: .mx-auto.d-block :}

I will however have to modify these animals and make them probably not-so-cute in order to create higher level evolutions as is so common in Pokemon. I have already designed one such character. Again, as a programmer, creating art is a difficult task for me. However, I was able to successfully scale, re-texture, and add cool effects to one of these animals to create a cool looking evolution. 

![PokemonAnimalEvolution](\assets\img\PokemonAnimalEvolution.gif){: .mx-auto.d-block :}
<div align="center"><i>Base hedgehog model from package (small) VS modified evolution (big)</i></div>


## FREE Stylized PBR Texture Pack

This is a completely free high quality texture pack including the bitmap texture with normal maps. The package includes textures for grass, dirt, wood, rocks, and just general ground-type textures that I will probably end up using in every scene in my game. 

![FreeStylizedTextures](https://assetstorev1-prd-cdn.unity3d.com/package-screenshot/531df1ff-96ce-45b2-94d5-08dc367f3a08.webp){: .mx-auto.d-block :}

Not much more to be said about [this package by Lumo-Art 3D](https://assetstore.unity.com/packages/2d/textures-materials/free-stylized-pbr-textures-pack-111778). It's high quality and it's free. Perfect.

## FREE Skybox Extended Shader

This is the final asset that I am going to highlight in this article. This free, animated, and beautiful [skybox by BOXPHOBIC](https://assetstore.unity.com/packages/vfx/shaders/free-skybox-extended-shader-107400) is perfect for any game with a stylized art style. 

![BOXPHOBICSkybox](https://assetstorev1-prd-cdn.unity3d.com/package-screenshot/3e783a21-bce1-469e-81b7-2f14e46777a2.webp){: .mx-auto.d-block :}

Similar to the texture pack above, there is not much more to be said. Oh, except that the clouds animate which is a super nice touch. But yea, another perfect free asset.

## Will They Blend?

As you can see, I am using a large variety of graphical assets from entirely different artists with some of them even having major clashes in art style. An example would be the free texture pack, which includes high resolution and highly detailed textures, coming to odds with the low-poly and single coloured textures from the polyperfect Ultimate Pack. The way to blend these different art styles, for the purposes of this game, is to compress the hell out of them until they all have this pixelated feel to them. Some of this was [covered in the previous post](https://haseebabid5.github.io/2021-02-05-Graphics/) and I will be going more in-depth in a future post about optimization. Stay tuned!
