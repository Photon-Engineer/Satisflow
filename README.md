# Satisflow

Hello and thank you for your visiting this repo! For the actual tool, go to [photon-engineer.github.io/Satisflow](https://photon-engineer.github.io/Satisflow/). For the source code, see [Satisflow-Dev](https://github.com/Photon-Engineer/Satisflow-Dev).

This goal of this project is to provide a helpful and relativley unique planning tool for the game [Satisfactory](https://www.satisfactorygame.com/). The tool is a flow-based calculator where you can add nodes and make connections for the purpose of planning out the various buildings needed to get the output rates you want. The flow-based approach allows you plan your factory based on your exact needs. Everything can be setup starting from miners, or you can start with a 'Creative' node to match an item output that already exists in your factory. You can save your work (manually) by exporting the layout as text, which you can import later to restore your progress.

The tool makes use of [Rete JS](https://github.com/retejs/rete) and several of its plugins to accomplish this. This project would not have been kicked off without their initial work, so thank you to the Rete team!

![Satisflow](/public/resources/satisflow_demo_image.PNG)

Simple tutorial:

## Adding Factory buildings and connecting them:
![Add and connect nodes](/public/resources/AddingNodes.gif)
Adding nodes as as simple as dragging the desired node into the editor from the options on the left side. All non-power related buildings are available, though those may be added in the future. Connect nodes by clicking on an output port, hold the mouse pointer down and drag to an input port. If the correct item is transmited, you will see the labels update accordingly, indicating the item amounts coming in to the new node. You can also add a building by right-clicking an empty spot in the editor. 

## Selecting a Recipe
![Changing Recipes](/public/resources/ChooseRecipe.gif)
Some nodes include a dropdown of possible recipes to choose from. All known alternate recipes are included for each building. If any recipes are not working correctly or have the wrong amounts, please add an issue to the repo. 

## Cloning and Deleting
![Cloning and Deleting](/public/resources/CloningNodes.gif)
For speed, you can right click a node to clone it. Cloning will preserve whatever recipe you've already selected. Using the same method, you can also delete the node. 

## Item connections vs Pipe connections
(Image is TBD)
Green connection points represent item inputs and outputs, orange circular connection points represent pipe outputs. You cannot connect an item output to a pipe input and vise versa. There are some buildings however, such as mergers and splitters that can be connected to either type. This makes it so additional nodes aren't needed to perform those types of logistics on fluids. 

## Overclocking
Most buildings have the ability to be overclocked up to 250%. To do this, add an overclock node and connect it to the overclock port. Note: overclock nodes can be connected to multiple structures, unlike other buildings. 

## Saving and Restoring
![Saving Progess](/public/resources/SavingReloadingLayouts.gif)
You can save your work by clicking the Export button, then copying the text produced and saving it somewhere of your choosing. When you are ready to restore it, paste the text back and select load. It is reccommended you save your work often, especially for larger projects. 

You can also clear the current progress by clicking the Clear Editor button. Note that you cannot recover your lost work if you click this by accident, and right now there is no confirmation message. 

## Feedback
If you have any issues, please make a post in the issues tab on github. Be specific and provide the text associated with the layout you've produced with the issue, and I will try to fix it in a timely manner. 

## Known Issues
Sometimes the editor will hang-up and you will no longer be able to pan or zoom. If this happens, click the export button to save your work, copy the text, reload the page, the paste the text back and reload your progress. The error is not understood at this point in time. 

Not all recipes have been tested. There may be recipes missing. 

## Donations

If you'd like to support me and this project, please use the donation button below:

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=2DS93F4W6JQKQ&currency_code=USD&source=url)