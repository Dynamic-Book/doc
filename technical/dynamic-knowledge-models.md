# Dynamic Knowledge Models

A Dynamic Knowledge Model (DKM) is a model representing a media of some knowledge you can interact with. Two basic examples of DKM are a digital image in very high resolution and a music score. The images are numerous in a paper textbook, however, contrary to digital image, you can't interact with to zoom-in to discover additional details.

A more elaborated example of a DKM, illustrating more precisely its model dimension, is a DrGeo geometric sketch. Described with a script, the user will insert it as an interactive view in her document, along handwritten notes. The user could then interact into this view, dragging objects to observe what is happening and discovering behavior to engage in new learning.

In this example, the model itself is an interactive geometry engine from which the user produces sketches with simple text scripts, thanks to a dedicated [DSL](https://www.sciencedirect.com/topics/computer-science/domain-specific-language) --- ***Domain Specific Language***.

The model dimension in a given DKM is what makes it versatile, with one you can design a lot of different interactive contents. It relies on the facilities provided by Oriented Object Programming, as explained by [Adele Goldberg](https://youtu.be/IGNiH85PLVg?si=HpbUQNGj1SU6rfwj&t=860).
Technically, all these views are Morph instances representing a view of the underneath model. The Morphs offer a common way to interact and to integrate in the handwritten document.
