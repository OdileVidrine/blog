---
layout: post
title: "I miss when AI images were weird"
---
I remember the first time I was amazed by neural network created images. I saw an article in January 2021
from OpenAI, showing these images DALL-E made from the text prompt "an armchair in the shape of an avocado."

| DALL-E example A | DALL-E example B |
| --- | --- |
| ![an AI generated image of an avocado chair]({{ site.baseurl }}/assets/images/avocado_2.png) | ![an AI generated image of an avocado chair]({{ site.baseurl }}/assets/images/avocado_3.png) |

Since then AI has evolved at a rate my human brain can't fully comprehend. AI-generated images are now impossible to
distinguish from other types of images with a cursory glance.

I understand why this is happening. It's the most logical way to improve the product. But I think something
interesting is being lost forever as AI models improve.

Here is an image I found on an archived 4chan thread from August 29, 2022, where the user prompted
Stable Diffusion to create "special agent dale cooper visiting my cats." 
(Disclaimer- I do not endorse anything that happens on 4chan. However, I must praise the people at https://desuarchive.org for their dedication to providing an easily searchable archive)
The result is unsettling. This is what Nano Banana creates on February 9, 2026, with the same prompt.

| Stable Diffusion (August 29, 2022) | Nano Banana (February 9, 2026) |
| --- | --- |
| ![an AI generated image of dale cooper with cats]({{ site.baseurl }}/assets/images/dale_cooper_2022.png) | ![an AI generated image of dale cooper with cats]({{ site.baseurl }}/assets/images/dale_cooper_2026.png) |

Aside from the "TNiN PPAEX" text visible, all the AI weirdness has been scrubbed from the image. Dale and his cats are no longer lumpy and smeared with the wrong number of legs.

Here is another example from the same archived 4chan thread from August 29, 2022, using the prompt 
"Full-body illustration of the Goddess Athena, golden armor, white robe, flowing blonde hair, detailed gentle motherly face, digital illustration, manga, アニメ, pixiv fanbox, intricate art by Ilya Kuvshinov, Alberto Vargas"
I do think GFPGAN Face Correction was used on this image, but her eyes are still uncanny.

| Stable Diffusion (August 29, 2022) | Nano Banana (February 9, 2026) |
| --- | --- |
| ![an AI generated image of athena]({{ site.baseurl }}/assets/images/athena_2022.png) | ![an AI generated image of athena]({{ site.baseurl }}/assets/images/athena_2026.png) |

I think the era of six-fingered hands, smeary eyes, and smudgy faces is gone forever. And because it happened so fast,
and the creepy era of AI generated images was seen as a flaw that needed to be fixed, no one archived the crappy stuff.

I miss it. So I wanted to bring it back to life. I also liked the idea of exploring AI technology in a way that is ethical,
as the ethics behind current models are debatable at best.
It started with 170 pictures of my cat.
![a black and white cat]({{ site.baseurl }}/assets/images/lucinatorpants.jpeg)
This shows an example from each epoch as the AI attempted to generate photos of the only thing it knew, my cat.
![a grid of ai generated images resembling a black and white cat]({{ site.baseurl }}/assets/images/epoch_grid170.png)
Later I modified the training datat to contain 300 pictures of my cat, and ran the code again.
![a grid of ai generated images resembling a black and white cat]({{ site.baseurl }}/assets/images/epoch_grid_300.png)

Considering how many images in a row look the same, I think there is overfitting happening. I plan to do more testing with
larger sets of photos.

My code is at https://github.com/OdileVidrine/Lucinator. If you want to use this repo to make your own image generator, create a folder called example_data with your images, run resize_image.py to shrink and crop images,
run train.py to generate the images, and optionally run make_epoch_grid.py to create the result grid.

