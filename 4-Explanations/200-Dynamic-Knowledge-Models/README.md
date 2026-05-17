# Dynamic Knowledge Models

A Dynamic Knowledge Model (DKM) is a model representing a media of some knowledge you can interact with. Two basic examples of DKM are a digital image in very high resolution and a music score. The images are numerous in a paper textbook, however, contrary to digital image, you can't interact with to zoom-in to discover additional details.

A more elaborated example of a DKM, illustrating more precisely its model dimension, is a [DrGeo](http://gnu.org/s/dr-geo) geometric sketch. Described with a script, the user will insert it as an interactive view in her document, along handwritten notes. The user could then interact into this view, dragging objects to observe what is happening and discovering behavior to engage in new learning.

The model dimension in a given DKM is what makes it versatile, with one you can design a lot of different interactive contents. It relies on the facilities provided by Oriented Object Programming, as explained by [Adele Goldberg](https://youtu.be/IGNiH85PLVg?si=HpbUQNGj1SU6rfwj&t=860).
Technically, all these views are [Cuis](http://cuis.st)'Morph instances representing a view of the underneath model. The Morphs offer a common way to interact and to integrate in the handwritten document.

# Examples

## Interactive geometry
In this example, the model itself is an interactive geometry engine from which the user produces sketches with simple text scripts, thanks to a dedicated [DSL](https://www.sciencedirect.com/topics/computer-science/domain-specific-language) --- ***Domain Specific Language***.

The user edits the model in the script editor at the left and gets the resulting dynamic media at the right, ready to be inserted in the document.

<img src="./images/drgeo2.png" width=400 />

Once edited, the DKM view is updated in the user document. The user can
then interact with the DKM view. Here it is an interactive geometry
framework where the user drags the geometric objects and observes
the behavior of the whole geometric sketch:

<img src="./images/drgeo1.png" width=400 />

At any time, the user is free to edit again a DKM script, to adjust
its contents. With the pointer tool selected, hovering a border of a
DKM view makes its halo icons to emerge; the left edit button opens
the DKM script editor:

<img src="./images/drgeo3.png" width=400 />


Script and sketch can be complex. Here a randomized variation of the
Sierpinski square:

<img src="https://static.mamot.fr/media_attachments/files/112/570/486/116/968/458/original/d0bf0c17e4be5a98.png" alt="The script model and the resulting dynamic view" width=400 />

## Text editor

A text editor model with style capabilities proves to be a valuable
DKM. At first it may seem odd to have a text editor as a DKM but
scripting text and style occurred to be valuable.

An example of a french text turned as a conjugation exercise, with
styled subject and verbs:

<img src="./images/text1.png" width=400 />

The example above also illustrate how a DKM view can be user hand
annotated with the highlighter or the pen.

This exercise is described with the dedicated script on the Text DKM:

<img src="./images/text2.png" width=400 />

Editing such script can be tedious but AI proved to be a valuable
aid. Indeed, AI with appropriate training can write these scripts. The
`brain` button, in the DKM script editor, generates the appropriate
prompt, specific to each DKM.

## Timeline

Timeline is another neat example of a DKM, interestingly empowered
with AI, to both retrieve historical events and edit the associated
script.

Again, a timeline is described with a dedicated and simple DSL. From
the document, the dynamic timeline can be reedited at any time.

<img src="./images/timelineEdit.png" width=400 />

The DSL is so simple that an AI can learn to use it from an example or
an appropriate prompt. With the request: "Give me another timeline for
the 10 most important battles of Alexander the great". It suggests:

```smalltalk
Timeline title: 'Major Battles of Alexander the Great' ::
	addEvent: 'Battle of the Granicus River. First major victory over Persian satraps in Asia Minor.' on: '-334.5.1'; 
	addEvent: 'Siege of Halicarnassus. The prolonged siege that forced the Persians to switch to naval warfare.' on: '-334.7.1'; 
	addEvent: 'Battle of Issus. Alexander directly defeats King Darius III, who flees the battlefield.' on: '-333.11.5';
	addEvent: 'Siege of Tyre. Seven-month siege using a massive mole (causeway) to conquer the island city.' on: '-332.1.1'; 
	addEvent: 'Siege of Gaza. A difficult, two-month siege of a key city on the route to Egypt.' on: '-332.10.1';
	addEvent: 'Battle of Gaugamela. The decisive, final defeat of Darius III and the Achaemenid Persian Empire.' on: '-331.10.1';
	addEvent: 'Battle of the Persian Gate. Alexander defeats a fierce resistance in the Zagros Mountains on the route to Persepolis.' on: '-330.1.1';
	addEvent: 'Siege of Aornos. Capture of a major mountain fortress, a feat even Hercules supposedly failed to achieve.' on: '-326.3.1';
	addEvent: 'Battle of the Hydaspes River. A costly victory over King Porus, featuring war elephants.' on: '-326.5.1';
	addEvent: 'Siege of Mallia. Alexander is severely wounded in a siege against the Malli tribe during his march south.' on: '-326.11.1';
	unshrink ;
	width: 4;
	color: Color yellow;
	view
```

The resulting timeline:

![Ten greatest battle of Alexander the Great](https://static.mamot.fr/media_attachments/files/115/356/691/735/237/920/original/189661d13dc24c40.png)

The user can learn simple programming assisted with an AI. Of course
the suggested historical data should be double checked and the script
edited accordingly.


# Technical characteristics

A DKM owns several characteristics and follow some requirements:

* It's a set of classes describing a model and at least one kind of
  PlacedMorph to represent its view. This view is plugged in the end
  user document.

* A specific instance of a DKM is described by a script. The script
  can be as short as one line of code (i.e. `VerbTableMorph newOn:
  'fill'`) or several lines of code. A script is written in Smalltalk
  with the dedicated DKM's DSL (e.g. see examples above).

* A DKM instance inserted in a document can be edited any time, its
  view is then modified accordingly. It is done by the invocation of
  the DKM script editor.


* **A DKM view can be annotated!** Here a text editor DKM was
  annotated with a pen and a highlighter. The handwritten annotations
  are attached to the view, and move and rotate with it. When the
  document is scaled, the annotations scale accordingly.

<img src="https://static.mamot.fr/media_attachments/files/113/896/653/214/030/283/original/e771e9a2057a6ccd.png" alt="Annotated text editor" width=300 />

* A DKM instance can be saved in the user's DKM library, for later
  resuse.

* Each DKM model comes with an icon, a textual descriptions, an
  example and a text prompt for AI training.

* DKM instances can be loaded and saved from the user library. They
  can be shared among users, as simple text script.


The [Cuis-Smalltalk](http://cuis.st) package **DKM-Core** is the minimal
prerequisite to develop additional DKM
https://github.com/istoa-eu/app/tree/main/src/dkm

