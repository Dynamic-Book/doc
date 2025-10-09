# Dynamic Knowledge Models

A Dynamic Knowledge Model (DKM) is a model representing a media of some knowledge you can interact with. Two basic examples of DKM are a digital image in very high resolution and a music score. The images are numerous in a paper textbook, however, contrary to digital image, you can't interact with to zoom-in to discover additional details.

A more elaborated example of a DKM, illustrating more precisely its model dimension, is a DrGeo geometric sketch. Described with a script, the user will insert it as an interactive view in her document, along handwritten notes. The user could then interact into this view, dragging objects to observe what is happening and discovering behavior to engage in new learning.

In this example, the model itself is an interactive geometry engine from which the user produces sketches with simple text scripts, thanks to a dedicated [DSL](https://www.sciencedirect.com/topics/computer-science/domain-specific-language) --- ***Domain Specific Language***.

* The concept demonstrated in the Dybo with a simple text editor: https://mamot.fr/@drgeo/114154912013226195

The model dimension in a given DKM is what makes it versatile, with one you can design a lot of different interactive contents. It relies on the facilities provided by Oriented Object Programming, as explained by [Adele Goldberg](https://youtu.be/IGNiH85PLVg?si=HpbUQNGj1SU6rfwj&t=860).
Technically, all these views are Morph instances representing a view of the underneath model. The Morphs offer a common way to interact and to integrate in the handwritten document.


## Technical characteristics

A DKM has several characteristics and  requirements:

* It's a set of classes describing a model and at least one kind of PlacedMorph representing the main view of the model the user will operate with.

* Instance of the model are created by code. At minimum one line of code (i.e. `VerbTableMorph newOn: 'fill'`) or a several lines Smalltalk script using the dedicated DSL of the model (e.g. DrGeo Smalltalk script). This is this view instance dragged and dropped in the page of document.

* From the page the model instance was dropped, it is possible to edit the script used to create the instance to redefine it: literally replacing the existing model instance by a new instance from the edited script.

* The edited instance by script can be used as model for later use by dragging and dropping back it in a Flap.

* It has an icon and a textual description

* It can be load/saved from disk, from an archive

It contains a model, icon; one or several scripts, each one represented as a FlapItem in a Flap.
