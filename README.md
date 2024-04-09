# FELON FINDER

This application aims to facilitate the recognition of a potential assailant by producing composite sketches.

## Table of contents
* [General info](#general-info-)
* [Installation](#installation-)
* [Documentation](#documentation-)
* [Q&A](#qa-)

### General info :
***

When launching FELON FINDER, four randomly selected images from our database (celebA dataset) are presented to the user.

The user selects the most similar images. They can choose from one to four photos each time.

By clicking on the "Valider" button, the selected images are then processed to produce four new composite sketches that increasingly resemble the assailant.

Once the user has identified a suitable sketch, they can save the image.

The software is currently only available in French.

### Installation :
***

WIP

### Documentation :
***

[Read the documentation](https://alexandrelayous.github.io/felon-finder/)

### Q&A :
***

- I selected the wrong images. How can I go back ?

To go back, select the "Photos précédentes" button.

- I selected images but can't remember which ones. What should I do ?

The images from the previous selection are available as reference images below the composite sketches until you go back or search for new pictures from the database.

- None of the produced composite sketches suit me. What should I do ?

If none of the images presented by the interface are similar, you have two options :

1) The “Nouvelles photos” button : By selecting this option, four new images will once again be randomly chosen from our database.

2) The “Rafraîchir” button : By selecting this option, the genetic algorithm will provide you with four new composite sketches based on your previous selection.

- How are the composite sketches produced ?

The images selected by the user are encoded using a variational autoencoder. Modifications inspired by genetic mutations and crossovers are then applied to the encoded images. After these modifications, the images are decoded and returned to the user.

- How can I change the settings ?

When selecting a single potential assailant, you can change the settings used by the algorithm to generate the new images. This flexibility has yet to be implemented for more than one face selection. 

To do this, click on the "Paramètres" button and choose the desired mean ("Moyenne") and variance values.

The "Réinitialiser" button allows you to return to the default settings every now and then.

- I want to change my display mode.

To switch from dark mode to light mode, click on the "Paramètres" button and use the switch before validating your changes.

- I found my assailant !

If you have identified the perfect composite sketch of your assailant among the produced files, select their image, press the "Enregistrer" button, and let the authorities do the rest of the work.

- **Does FELON FINDER guarantee 100% accurate identification of an assailant ?**

FELON FINDER is an identification aid tool and cannot guarantee 100% accurate identification. However, it can greatly facilitate the identification process by providing detailed composite sketches based on your descriptions and memories.
