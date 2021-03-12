# landing-pad-dataset-generator

The dataset generator allows to easily and acurately make a dataset for landing pad localisation. The software proposes **images and ```.csv``` file of the observer's position**. The dataset can then be used under supervised learning for accurate pose estimation.

## How to install

To run the software, it is first needed to install Blender from their [download page](https://www.blender.org/download/)

The `.blend` file has to be run from the terminal to enable python script. The following command lines ensure firstly to get to the current folder, secondly to execute the *blender* file.

```
cd ~/landing-pad-dataset-generator
blender dataset-generator.blend
```

Finally, the script can be run in two ways: by clicking the *Play button* or by pressing the keys *Alt + P*.

## How to tune the environment

Follows a non exhaustive list of the parameters that can be adjusted to suits the project,
- **Image size**: changing parameters *width* and *height*
- **Dataset size**: this is the total number of generated images
- **Boundary position of the camera**: it suits the camera parameters to ensure visibility of the landing pad
- **Image format**: by default this is encoded in ```.PNG```
- **Observer's position**: It is composed of location of the *Camera* and rotation of the *Plane* under boundaries conditions
- **Background**: linked as *child* of the landing pad, a photo realistic background can be added. For instance [Quixel](https://quixel.com/) assets can be used with appropriate [plugin](https://quixel.com/plugins/)
- **Landing pad image**: by replacing ```landing-pad.png``` the landing pad texture can be modified
