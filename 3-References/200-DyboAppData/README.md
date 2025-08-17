## Root directory

The user data of a DyboApp is saved in a tree of directories located in the host computer at ``DyboApp/resources/data``. This path is called the **userDataPath**. In the application code, the absolute path is at ``DySystem userDataPath``

At **userDataPath** are found:

* the file ``data.obj``, a tree of Smalltalk objects of the general user data (identity, schools, classes, students, class groups, lessons, topics, school year description with time slot and days off)

* the schools' directory matching the schools set in the user settings (settings tool). The directories are named after the school name. Invalid chars in the school name are converted to #. For example ``CO Foron`` set a directory named ``CO#Foron`` in the host computer.

* the directory ``tasks`` enumerates in distinct directories, the data of the assigned tasks (written notes). Each directory contains a document file ``doc.dat``

## Document directory

In each school directory, the document files are spread in sub directories structured as: ``SchoolName/ClassGroup/Lesson/Topic/TimeStamp``.

For example with ``CO#Foron/1022/Mathématiques/Calcul#littéral/2025-08-16-19h30m45s``,
* CO#FORON is the school
* 1022 is the class group
* Mathématiques is the lesson
* Calcul#littéral is the topic
* 2025-08-16-19h30m45s the directory for the document created at this date and time.

The time stamped leaf directory contains the document files: a mandatory ``doc.obj``, tree of Smalltalk objects representing the pages of the document -- sheets, written notes, interactive morphs; an optional annotated pdf document and its JPEG previews.

## PDF document
Dybo document can annotate PDF document. To do so, the Dybo document is created when importing a PDF file. This file is copied in the time stamped document directory and bitmap previews of the PDF document are generated at this same location.

* The package ``popper-utils`` and its program ``pdftocairo`` is used to generate the the bitmap preview. See the class method ``DySystem>>import:to:pages:``.