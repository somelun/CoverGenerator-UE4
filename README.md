# Cover Generator 

The cover generator is a plugin for Unreal Engine 4. 

It analyzes the geometry of a level to find possible cover points. Cover points can then be parsed via the native **Environment Query System (EQS)** to allow AI controlled characters to find spots to hide during a fight or to prepare an ambush.

The system offers different set of information per generated cover such as if it is a crouched or standing cover, if the character can stand to shoot or lean on the side.

# Example video of AI using the cover generator
<a href="http://www.youtube.com/watch?feature=player_embedded&v=igwEAeQFwhM
" target="_blank"><img src="http://img.youtube.com/vi/igwEAeQFwhM/0.jpg" 
alt="Dynamic tactical cover generation coupled with a GOAP AI " width="240" height="180" border="10" /></a>

# How to use the cover generator? 
- Add the plugin to your project

- The cover generator is using the native nav mesh bounds volume of a level to generate the covers, so if you do not already have one in the scene, add a nav mesh bounds volume to your level.

![Add a nav mesh bound volume](https://cloud.githubusercontent.com/assets/6062062/23832918/7c1c2ab4-073e-11e7-9bbe-1860f58f1a65.jpg)

- You can see the generated navigation mesh by pressing 'P' on your keyboard.

![Visualize the navigation mesh](https://cloud.githubusercontent.com/assets/6062062/23832943/cd750854-073e-11e7-8ef6-464449bf18a2.jpg)

- Create a CoverGenerator blueprint and drop it in your level

![Create a CoverGenerator blueprint](https://cloud.githubusercontent.com/assets/6062062/23832877/d51f40e8-073d-11e7-9ba2-04e13065fd29.jpg)

- By default, the cover generator will generate the cover points on begin play. To visualize the generated points, click on the cover generator actor in your scene and tick the option "Debug Draw All Points"

![Display generated cover points](https://cloud.githubusercontent.com/assets/6062062/23832977/5e7e1d54-073f-11e7-848d-9fad46882bfa.jpg
)

- You can see the result on the image below. Blue spheres represent cover points, the lowest ones for crouched covers, the highest ones for standing covers. Arrows are representing from where the character can shoot.


![Simulating level](https://cloud.githubusercontent.com/assets/6062062/23833001/c020b030-073f-11e7-832a-a8a5a8696790.jpg
)


## How to enable the Environment Query System?

See UE4 quick start guide: [https://docs.unrealengine.com/latest/INT/Engine/AI/EnvironmentQuerySystem/QuickStart/2/](https://docs.unrealengine.com/latest/INT/Engine/AI/EnvironmentQuerySystem/QuickStart/2/)





