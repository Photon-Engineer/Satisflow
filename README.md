# Satisflow

Hello and thank you for your visiting this repo! For the actual tool, go to [photon-engineer.github.io/Satisflow](https://photon-engineer.github.io/Satisflow/). For the source code, see [Satisflow-Dev](https://github.com/Photon-Engineer/Satisflow-Dev).

This goal of this project is to provide a helpful tool for the game [Satisfactory](https://www.satisfactorygame.com/). The tool is a flow-based calculator where you can add nodes and make connections for the purpose of planning out each part. This is tool is designed from the ground up with interactivity in mind. It allows you to save the output as text to be able to reload previous work. The tool makes use of [Rete JS](https://github.com/retejs/rete) and several of its plugins to accomplish this. This project would not have been kicked off without their initial work.

![Satisflow](/resources/satisflow_demo_image.PNG)

Simple tutorial:

## Adding Factory buildings and connecting them:
![Add and connect nodes](/resources/AddingNodes.gif)
Adding nodes as as simple as dragging the desired node into the editor from the options on the left side. All non-power related buildings are available, though those may be added in the future. Connect nodes by clicking on an output port, hold the mouse pointer down and drag to an input port. If the correct item is transmited, you will see the labels update accordingly, indicating the item amounts coming in to the new node. You can also add a building by right-clicking an empty spot in the editor. 

## Selecting a Recipe
![Changing Recipes](/resources/ChooseRecipe.gif)
Some nodes include a dropdown of possible recipes to choose from. All known alternate recipes are included for each building. If any recipes are not working correctly or have the wrong amounts, please add an issue to the repo. 

## Cloning and Deleting
![Cloning and Deleting](/resources/CloningNodes.gif)
For speed, you can right click a node to clone it. Cloning will preserve whatever recipe you've already selected. Using the same method, you can also delete the node. 

## Overclocking
Most buildings have the ability to be overclocked up to 250%. To do this, add an overclock node and connect it to the overclock port. Note: overclock nodes can be connected to multiple structures, unlike other buildings. 

## Saving and Restoring
![Saving Progess](/resources/SavingReloadingLayouts.gif)
You can save your work by clicking the Export button, then copying the text produced and saving it somewhere of your choosing. When you are ready to restore it, paste the text back and select load. It is reccommended you save your work often, especially for larger projects. 

You can also clear the current progress by clicking the Clear Editor button. Note that you cannot recover your lost work if you click this by accident, and right now there is no confirmation message. 

## Known Issues
Sometimes the editor will hang-up and you will no longer be able to pan or zoom. If this happens, click the export button to save your work, copy the text, reload the page, the paste the text back and reload your progress. The error is not understood at this point in time. 

Not all recipes have been tested. 

If you encounter any other issues, please add it to the issues on this repository. 

## Donations

If you'd like to support me and this project, please use the donation button below:

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=2DS93F4W6JQKQ&currency_code=USD&source=url)
