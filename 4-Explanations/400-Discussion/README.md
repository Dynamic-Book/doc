*A discussion about the Dynabook with the aim of clarifying Hilaire's ideas. April 2024*

# Hardware

**---JR**: Let's start with the **hardware**, the Dynabook device. What hardware is envisaged?

**---HF**: RISC V architecture. It is, to my knowledge, the hardware as close as
possible to free software. Nevertheless software should be portable to
any hardware platform GNU/Linux can operate on.

You will want the Dynabook hardware to be assembled locally, to integrate
it the local economy.

**---JR**: Can you give more information about the idea of using RISC V hardware? I can sympathise with the idea of free hardware but using uncommon hardware without mature support of the main distros and operating systems would make the initial situation much harder for everybody. Besides, the experience with (perceived as) substandard-quality hardware was one of the problems with OLPC and the Spanish initiatives. We would have to analyze the reasons why former experiences failed before starting a new one.

**---HF**: No reason to stick to RISC V then. The Dynanook app will be tested with the existing devices in the school, that's what I want to experiment in my school anyway.

**---JR**: OK, then for the general architecture. In the [video of the presentation in Buenos Aires](https://www.youtube.com/watch?v=DBjJrAZSEHs) you mention that **a pen** is essential. Is that a pedagogical point? Can you develop that?

**---HF**: The pen is not only essential but central. If you can't operate fluently with an electronic pen and hand writing, the project is to be abandoned and the learner should use a paper notebook. [Some reading on the importance of writing](https://www.courrierinternational.com/article/education-apres-avoir-mise-sur-le-numerique-a-l-ecole-les-pays-scandinaves-font-machine-arriere)

**---JR**: Well, I would say that the research is inconclusive [Which modality results in superior recall for students: Handwriting, typing, or drawing?](https://jowr.org/index.php/jowr/article/view/963):

> Overall, the evidence did not suggest that the mechanisms involved in handwriting led to better free recall than those involved in typing.

And writing on paper might have different affordances from writing (not typing) on a screen. Therefore a prudential gradual introduction of reading and writing on digital devices, taking into account the age of the students, would be my present position. What age are the students supposed to be?

**---HF:** Late primary school and secondary I and II. The good news is Dynabook wants to offer all: handwriting and drawing through its paper object and typing with its virtual keyboard when appropriate.

## Alan Kay's Dynabook

**---JR**: Are you thinking of a device similar to Kay's idea? That's what I imagine from reading you.

![kays_dynabook](https://github.com/hilaire/dynabook/assets/3305693/b26956b1-26c2-4552-aa3f-1b95cf86bcda)

**---HF**: Not at all like the sketch of the Dynabook by Alan Kay. The two main assets of the learner are reading and writing from textbooks and notebooks, very often done simultaneously. In any electronic device pretending to be useful for education, this consideration should be taken seriously and central to the user experience.

Therefore, it is more a metaphor of paper notebook & textbook, [with two surfaces](https://github.com/hilaire/dynabook/tree/main/resources/doc/DynabookApp#concept) where the user can read and write simultaneously. It is subject to discussion to have two surfaces or just one surface split in two for simultaneous reading and writing. 

**---JR**: I suppose you imagine a situation in which each student has their Dynabook. Who would own the devices?

**---HF**: TBD. My point of view is it should belong to the users, students and teacher.

**---JR**: What if the student or the teacher chooses to use their own device?

**---HF**: The dynabook app will be portable but no hardware+software will match
the expectation of the Dynabook. So it's unlikely. I don't bring my laptop
in my classrooms, I use what is there. No reason to be different.

Nevertheless, as the Dynabook app is portable, the teacher could use it at
home, in their own device if it feels more appropriate, for example to
create a new dynamic knowledge model or to script existing one.

You know, as a free software user, that the current devices are also
restraining the freedom of the user. Alan Kay wrote a note about that,
it is worth reading it.

[An Interview with Computing Pioneer Alan Kay, April 02, 2013](https://techland.time.com/2013/04/02/an-interview-with-computing-pioneer-alan-kay/)

**---JR**: I'm not convinced by the idea that the teacher will use "*what is there*", I'm familiar with teachers unplugging screens, keyboards from Linux desktops... and plugging them to their laptops because they wanted to use their Windows or Mac... So a school policy must be created, be it that the app works on all operating systems and devices or that it's compulsory to use the classroom device.

**---HF**: In my school, in the teacher room, about 5/50 teachers use their own laptop. In the classroom, may be 2/50 use their own device. Some administrative duties are more easily done with the computer, not to mention the access to the teacher documents in the LAN. Nevertheless, I don't see any reason those teachers would not be able to continue so. However the idea is that the teacher should feel more comfortable to use her own Dynabook.

## One Laptop Per Child (OLPC)

**---JR**: Is this a continuation of the **OLPC** 2005 idea? What is different now?

**---HF**: No, it is not a continuation of OLPC. OLPC was intended for developing countries, something I don't feel at ease with. It felt like one community of people imposing a view of their own about how education should be conducted, discarding all the cultural heritage of those countries. If you consider the cultural heritage of South-America, it is as old as the Greek or Persian civilisations.

Dynabook is for **developed countries** which have different circumstances
than developing ones. Take a look at the first paragraph at
[An ordinary back-to-school season](https://github.com/hilaire/dynabook/blob/main/resources/doc/An%20ordinary%20back-to-school%20season.md).

Therefore, Dynabook intends to replace all these paper materials, notebooks
and textbooks, with a vehicle to represent knowledge in dynamic forms.

The device will operate differently than OLPC. At first, it will not try to mimic a mini-laptop, with the same kind of applications (logo, spreadsheet, text writer, etc), although you will have access to these applications. Its core feature, the closest thing you can imagine, is a paper notebook where the user writes in a document with an electronic pen and integrates, in this same document, dynamic knowledge models (think of a drgeo sketch).

It is a tool to represent knowledge --- as done with paper notebooks and textbooks --- but with dynamic models.

The core of the pedagogical dimension of the dynabook is to have such
dynamic knowledge models (think DrGeo) the teacher can rely on and
integrate to her document. This integration will be materialized
through a library of existing scripts of those models (think DrGeo
Smalltak Sketch) or through scripts of her own, adapted from existing
ones or newly edited ones (think the DrGeo Smalltalk Sketch Editor).

My intend is to use Cuis-Smalltalk as the main vehicle to do that.

In one aspect, thus existing and pre-developed models will be
parameterized or programmed with Smalltalk code (it is what Smalltak
was designed for). A user not interested in scripting will just use the library
of existing ones, a curious user will learn from existing scripts and
create their own.

One big difference with OLPC is OLPC it was targetting the learner. Dynabook
is for both teacher and learner.

**---JR**: The OLPC was both a hardware and a software project, like yours. I can admit that the hardware part was thought for the third world schools and students (and the project continues somehow in Uruguay, not Paraguay, not quite a third world country: 
[Ceibal](https://es.wikipedia.org/wiki/Ceibal_(Uruguay) 
---reading an independent assessment would be great), but the aim of the software aspect was to create a learning environment based on python and smalltalk. Now I think you propose a more reduced environment (no Sugar, no ordinary apps) based on a modern version of smalltalk, and you say it's going to be teacher-centred, which I hope it's an inaccurate way of saying school-centred or teaching/learning-process-centred. Tell me in what I have misunderstood you.

**---HF**: I disagree the OLPC was thought for the third world, my believe is the reality of education in the third world was not considered. The Sugar approach is based on activities, it is a very classic way of using a computer. The main idea --- or more likely ideal --- was that the learners would not need an adult and they would be able to educate themselves with the XO. 

I take a different approach by first looking at the existing reality in education in developed countries. As an educator experiencing different school systems, I think we can do better in how IT is introduced and/or used in the education system. If you consider the whole economy of a developed country, IT is present everywhere. Very often, specialized computer devices are designed for a specific domain of the economy. The objective is to make the tasks as effective as possible, with both dedicated software and hardware. Sometimes only the software is specialized. I take the example of the cash register to illustrate how specialized for a given task can a specialized computer device be.

The Dynabook's aim is to be the cash register of education. In that sense, I want to read the reality in the classroom and think how a dedicated computerized device should be designed both in its hardware and software to make this reality more efficient. I don't believe in revolutionizing the way teaching is done, but to improve it for both the teacher and the learner. For example, you will have some features one may think insignificant as how the documents, the tasks and the assignments are organized in the Dynabook but those are the reality both teachers and learners have to deal with, several times a day. Dynabook wants to be as neutral as possible considering the learning models and it will accommodate to how a teacher wants to organize his teaching activities.

**---JR**: So, your proposal is not an updated OLPC Dynabook, that's clear now. Can you speak about the RISC V architecture you mentioned? Is it powerful enough? Have you tried it?

**---HF**: I mentioned RISC V because this is to my understanding the closest architecture to free software. Nevertheless, the [OpenSmalltalk VM](https://opensmalltalk.org/) is not yet optimized for this architecture, Arm architecture is. But it does not really matter, we will iterate with prototypes using existing nano computers as the Raspberry PI 5.

Apart from choosing the nano computer there is the issue of the case. Does it need to be super light? I don't think so. A 4 kg weight could be acceptable as it will replace most things in the backpack. Could then the case be integrated to the back pack?

As we have no choice but to enter a sustained world, should not the case be made of wood? Which wood is resistant enough? For the same reason, it should be assembled locally, to make it even easier to fix when broken.

What about the battery? We certainly do not want a battery pack hard to repair but instead a set of individual cylindrical battery cells which can be replaced individually when damaged.

The autonomy of the Dynabook should be as a minimum half of a school day but 8 hours of autonomy would be optimal. This raises the question of the dual display, it will be an energy hog. Will e-ink be an option, or dual bw/color screen as in the OLPC for lower power consumption?


## The Cash Register metaphor

**---JR**: Let's speak a bit more about the **cash register** metaphor. If I understand, you propose to create a tool that does one task and does it well. But that's not the trend of the times for hardware (software is another world here and the principle should be considered): digital cash register machines do more than just add numbers, they keep registers and print tickets now; smartphones are no longer simply phones, they are complete computers plus cameras, audio recorders, gps devices, music players... Why a single-task specialized device? Would it be much cheaper? No, unless economy of scale is achieved. Would it be the only device to be used in a school or would additional more generic ones be necessary? Would it respond to all the needs of the students and the teachers of would they also have to take to school their computers or their smartphones?

**---HF**: Nowadays cash registers are indeed involved in all the associated tasks to make consumer retails more efficient. So should the Dynabook. This is the exact point of my metaphor.

The Dynabook will not do only one task. I described the core tool of the Dynabook, the Dynabook app, whose objective is to replace the paper notebook, school textbook, binder, etc. as used today in the classroom. I see no reason a learner could not use [Wims](http://wims.univ-cotedazur.fr) or [LibreOffice](http://libreoffice.org) with the Dynabook.

**---JR**: So obviously I misunderstood you. You write

> I take the example of the cash register to illustrate how specialized to a given task can a specialized computer device be.

So you mean that especially designed hardware and software must be created, after analyzing the "realities" of the classroom. To be realistic, I don't think a project like this has the capacity to design hardware from scratch, it can only choose between the hardware options available which options it prefers, and for its implementation cost and availability will be the decisive criteria. As regards software, we are not going --I guess--- to rewrite the operating system, just maybe adapt a Linux distro, and add the Dynabook app plus possibly some more educational resources.

In the second place, if we don't want to start with intuitions but facts about the "realities" of the classroom but facts, and if we don't want to reproduce bad practices but the best ones (the reality of the classroom can be that the teacher is a bad teacher or teachers used to and dependant on privative software), we need that analysis before designing anything. Or at least a theory about what this reality is. What IT does the teaching/learning process need? We'd soon arrive at the competencies discussion. And to the libre vs. privative one. I don't think we can convince an administration or a schhol without these discussions.

**---HF**: As a teacher I experience the reality of my classes every day. When you are an expert of a domain, here education, and you are practicing it at a regular pace, you have the best and more meaningful know-how about what is needed and what is not needed. So my assertions on Dynabook prerequisites are more based on facts than intuitions, although there is some part of intuitions on how you want the design realized in the Dynabook. But you are absolutely right that it is best to diversify your observations with different teacher practices. Hopefully, in a close future I will have opportunities to observe the reality of the classes with other teachers.

Designing the hardware from scratch is difficult indeed, but it is not because something is hard that it should not be attempted. Nevertheless, it may not be necessary at first to design hardware from scratch given the existing options of embedded hardware based on ARM and Risc V CPUs.

## Reading & Textbooks

**---JR**: About the **reading** skill. Above you have written
> Dynabook intends to replace all these paper materials, notebooks and textbooks

and you have quoted research about the advantages of reading on paper, not on screen. I wonder if the Dynabook should substitute paper textbooks, or whether a balance should be looked for. Anything to say about this?

**---HF**: I think Dynabook should replace both notebooks and school textbooks, and the experience of reading and writing should be excellent with it. Having both Dynabook and paper school textbooks is antinomic. Digital textbooks will be on the Dynabook. If not possible, don't use the Dynabook.

On the other hand, kids equipped with a Dynabook should continue reading paper books. A reader is emotionally engaged with a story in a book, which is unlikely with a school textbook. The cognitive experiences of reading a school textbook and a book are very different.

**---JR**: Are you familiar with the digital-textbooks-only experiences around the world? I don't think they are successful without nuances. You have to take into consideration many aspects, the age of the students again, but also cultural aspects, their ability... There's not a simple generalizable solution.

**---HF**: Yes I know some. The first difficulty is the access to the digital textbook. As one can understand, publishers can not always provide the textbooks on digital form, free to use and to modify on deployed devices. However a few publish textbooks under a free documentation license. Such publishers and professional teacher organizations should be favored and involved. Right now, it is an aspect out of the scope of the present Dynabook project. Although deploying Dynabook will not make sense if the involved educational institutions have not secured the access to digital textbooks. The second difficulty is "are the devices fit to the task" or is it a tool that degrades the experience of using a textbook? Often the experience is largely degraded over a paper textbook. I think we can do better, with both device and software designed for that purpose.

**---JR**: It's an issue to discuss whether textbooks in pdf format are an improvement over paper textbooks. Yes, one reduces weight on the backpack and they can be reproduced infinitely, but the psychological proprieties and affordances of interacting with them are different, and they keep on being closed external resources neither created nor modified by the teacher. Maybe what you are thinking about are free atomic learning resources for the teacher to reuse, modify, mix, etc. This is not new, it's the way I worked some ten years ago (I'm retired now). The resources exist; they have been written in flash, java, javascript, smalltalk, html5... time after time. But I'll tell you this is difficult to generalize because it's much more work for the teacher to find, assess, adapt, etc. and because the students have the idea that computers and smartphones are tools for communicating and for playing, but not for learning (you were right: the learning machine is a myth because the internet BigTech has created wants consumers, not learners); after the inicial surprise I found a lot of resistance from the students when using the computers systematically. And I insist, we need research to prove that studying a lesson on a screen yields the same as studying it on paper, maybe the age and they way the transition is done are to be considered.

Anyway I myself can't find an argument for digital interactive atomic learning resources independent from a constructivist perspective.

**---HF**: Oh, pdf format is definitely a degradation over paper textbooks. Think about the way you can interact with a paper textbook: book marking with colored tags, handwritten notes, looking at several pages at once with your fingers used as temporary bookmarks. And also paper textbooks are extremely ubiquitous, extremely resistant to physical stress. The way a Dynabook user will interact with a pdf document will have to be thought with a lot of attention in the details.

It is likely that some pdf textbook could not be modified, nor routed with its source counter part you can edit on the Dynabook [jr: I don't understand: routed? rooted?]. It really depends on local policy regarding the selected textbooks. Teachers also have the freedom to design their own documents, as complementary resources to the textbook. I don't believe too in atomic resources found there and there, at least for the core pedagogical documentations, of course it does not discard supplementary resources for specific needs. If a Dynabook is to be deployed, provide the digital textbooks, if not, stick to the paper textbook, after all we have been just fine for decades like that.

Regarding a standard workflow, as observed in my school, I believe in pdf documents as resources produced by the teacher or taken from the textbook, imported as a digital paper document and enriched with handwritten annotation and dynamic knowledge models if appropriate. Those enriched pdf's will be short lived resources, produced for a given context of teaching.

Therefore, the digital paper document is to be an important part of the Dynabook app that needs to be carefully designed. Without a doubt, it will evolve in several iterations.

Regarding the consumer behavior of the students, as professionals of the domain, it is our duty to expose them to meaningful and educative use cases of the computer and network. Wims is an excellent example.

**---JR**: It's obvious we agree, we are speaking of free dynamic modifiable resources. It was your usage of *pdf's* and *textbooks* that was ambiguous, I think the point is clear now. 

# Software

**---JR**: What happened to **DrGeo**? Isn't this a new rebirth of DrGeo? Or does it live underneath, in the scripts de app runs?

**---HF**: DrGeo exists as a standalone application of its own. In the Dynabook device, I envision it will continue to exist as a standalone application of its own, but also as an integrated part to the Dynabook application, through sketches designed by Smalltalk code. DrGeo is also my laboratory to explore new ideas as the Smalltalk Sketch and associated GUI design. A DrGeo sketch designed with Smalltalk code is an example of a dynamic knowledge model related to geometry. DrGeo is really my test bed to see how you will want the tooling be arranged to let teachers design dynamic knowledge models: How will the code editor be arranged? What contextual help? Do we want it in local language? So far, there are several domains I am not satisfied with like the debugging experience of Smalltalk Sketch and how the integrated documentation is designed.

DrGeo is quite a complex application because you have both the dynamic knowledge model (in the field of euclidean geometry) and the whole GUI to build the sketch with mouse and clic operations. However, it is possible to build a much simpler application with only its dynamic knowledge model and its public Smalltalk interface to script it. This makes the whole application smaller. Most dynamic knowledge models taught in school should be developed like that.

## Dynamic Knowledge Model

**---JR**: In your presentation to the public you wrote:

> Any serious Dynabook realization should be considered as a *cash register of education* (...)
> A dedicated hardware and software environment for a meaningful use in education (...)
> A vehicle for *dynamic models of knowledge* the user can design and/or operate on

This is too generic, all constructivist educational software since Papert and Kay would be included. What's new? What's different now? Do you have anything to say about why the older proposals didn't succeed?

**---HF**: There are some details in the [introduction of Dynabook App](https://github.com/Dynamic-Book/doc/tree/main/technical/DyboApp). Nevertheless, I don't agree that _all constructivist educational software since Papert and Kay would be included_, Dynabook is not about constructivism.

I never mentioned constructivism. To be honest, I don't subscribe to the idea of constructivism, it is most of the time an ineffective teaching model, although in some situation it is valuable. Read my article [Dynabook and its learning models](https://gnu-drgeo.blogspot.com/2018/07/the-dynabook-and-its-learning-models.html).

To be honest I am neutral to the teaching methods, all approaches should be equally accessible, this is the the freedom of the teacher. The Dynabook should not interfere with that. After all, a notebook doesn't dictate how a teacher is conducting her job.

I prefer to think of dynamic knowledge media inserted in a _traditional notebook_. It will encourage both reading and writing while manipulating media to foster learning. Depending on how the teacher will arrange her contents and learning activities, one or several specific learning models will be engaged. In another learning activities, the same teacher may design differently her activities with other learning models engaged. This is what happens in the classroom, teacher are not stuck to one learning model.

The older proposals, as you wrote it, failed because it was not teacher-centered but learner-centered with a lot of dazing romance. As long as we have teacher with students, you want a system to be centered around its main prescriptor, the teacher. This is why in the Dynabook app model I described a dedicated [business model](https://github.com/hilaire/dynabook/tree/main/resources/doc/DynabookApp#business-objects), taking in consideration some of the professional constraints of the teachers, and the students as well.

**---JR**: Can you explain what a ***dynamic knowledge model*** is?

**---HF**: It is a model representing a media of some knowledge you can interact with. Two basic examples of dynamic knowledge models are a digital image in very high resolution and a digital sound track. The images are numerous in a paper textbook, however, contrary to digital image, you can't zoom-in to discover additional details.

A more elaborated example of a dynamic-knowledge-model, illustrating more precisely its model dimension, is a DrGeo geometric sketch. Described with a script, the user will insert it as an interactive view in her document, along handwritten notes. The user could then interact into this view, dragging objects to observe what is happening and discovering behavior to engage in new learning.

In this example, the model itself is an interactive geometry engine from which the user produces sketches with simple text scripts, thanks to a dedicated [DSL](https://www.sciencedirect.com/topics/computer-science/domain-specific-language) --- ***Domain Specific Language***.

The model dimension in a given dynamic-knowedge-model domain is what makes it versatile, with one you can design a lot of different interactive contents. It relies on the facilities provided by Oriented Object Programming, as explained by [Adele Goldberg](https://youtu.be/IGNiH85PLVg?si=HpbUQNGj1SU6rfwj&t=860).
Technically, all these views are Morph instances representing the underneath model. The Morphs offer a common way to interact and to integrate in the handwritten document.

**---JR**: Regarding  Goldberg's interview ---[text transcript](https://archive.computerhistory.org/resources/access/text/2013/05/102701984-05-01-acc.pdf) available---, the main point seems to be

> So the lovely part that has proven true for professional
> programmers as well as kids is when you start with something, an object that does something, and then
> you put many objects like those together and have them interact, and then you extend and make them
> behave a little differently, you can take a very incremental approach to learning how to control a computer
> system

but I would need more explanations to understand your point. You seem to defend that Smalltalk is a better technical solution, that provides direct access to the objects underneath, but I don't see how to present these points as convincing arguments to teachers in search of easily usable resources. 

**---HF**: These are technical aspects on how those resources (text scripts of dynamic knowledge model) will be produced. [I explained earlier](#one-laptop-per-child-olpc) that most teachers will rely on existing collections of scripts to insert dynamic content views in their documents. Nevertheless, the few willing to go further in designing dynamic content will be able to do it directly from the Dynabook, with a dedicated editor. The picture below shows at the left the text script edited with a DSL on Euclidean geometry, the view at the right is the resulting dynamic content illustrating a property on geometry. Most teacher will only deal with content as presented in the right view.

[[images/Script-DynamicKnowledge.png|Editor of script on geometric Dynamic Knowledge Model]]

Regarding the choice of Smalltalk to both develop and script Dynamic knowledge model, this programming language and environment was designed with kids in mind. It offers both an extremely coherent language and a live environment to experiment ideas and code. Cuis-Smalltalk is a modern incarnation focusing on simplicity and elegance.

**---JR**: Let me try to understand. Are [PhET simulations](https://phet.colorado.edu/) dynamic knowledge models?

**---HF**: Answer the following questions and you will find out. As the name suggests, these simulations are interactive and related to science, so they convey some sort of dynamic knowledge representation. Now, can those simulations be described by simple user scripts, that a teacher can learn from to edit, to modify and to reuse differently? If yes there are dynamic knowledge models, if not they are dynamic knowledge application or representation, that maybe the user can parametrize but it will not make a model.

**---JR**: We are speaking of free resources, so we already have their source and the rights to use and modify them. Doesn't the answer to your question depend of the familiarity of the user with the programming language or scripts, or on the existence of high level tools to create and modify the simulations? If we took this statistic point of view, would the fact that more teachers use python or javascript than smalltalk prove anything? And as a second point, do we really expect the teachers to create the resources? Isn't it enough to reuse, mix, adapt,assess... free available educational resources? Are the ones available so bad, so insufficient? And the educational institutions and volunteers have been creating resources for more than twenty years? Are they useless and have always been so?

**---HF**: So we will not know if PhET instances are models or just user applications... In dynamic knowledge model, the meaning of model must be understood clearly. A *Model* is an object or group of objects created and manipulated through a set of programming instructions in the context of a dedicated *DSL*, in a live environment the experience is even easier.

Access to the source and rights is one thing, the ability to modify the source to achieve a different result in the context of real use case is a completely different thing. There is a huge barrier in concept, knowledge and accessibility between the two, even if you have access to the source. In the Dynabook app I want to lower this barrier as much as possible, to give maximum freedom to the user to study, to learn and to modify.

Smalltalk is ontologically designed with this very specific intention, to empower users. This is something that is hardly done with JS or Python, they fall short in some conceptual and technical areas as pure OOP, partial compiling of objects, environment with "live" entities to interact with. When you know one programming language, learning another is not an issue, otherwise we will still be programming in Fortran.

I don't understand your questions regarding existing free resources, your tone seems to indicate I discard them. Not at all, I see no reason they can't be used in the context of the Dynabook. I am describing what is a dynamic knowledge model and I choose to implement the Dynabook App in Smalltalk and not js+css+html because the latter is terrible to manage complexity, although it benefits of the awesome job done by corporations like Google on the JavaScript VM regarding efficiency in execution (https://v8.dev).

**---JR**: Then an easy question for you to answer: why the **Cuis environment**? I know you fell in love with Smalltalk many years ago, but explain why not you as a developer but the end user should prefer the developers use Cuis over javascript plus html5 plus css.

**---HF**: First, I don't fall in love with programming languages, I use the right tool to achieve what I want to do. Smalltalk lets me handle the complexity far more easier that C++, the previous language DrGeo was coded with. You can search the literature why. The user has no preference regarding the developer environment as long as he does not need to operate directly on the engine, on the contrary Smalltalk is more developer friendly.

## Device & Operating System

**---JR**: Is your project multiplatform? Does in run on Windows, Linux, Android, containers, usb drive...?

**---HF**: Do we really care?

**---JR**: Yes we do, if we want it used it's a point that has to be answered. And I find a passive usage by the students, who definitely prefer to use mobile phones as their main tool, won't they be able to create or modify activities?

**---HF**: Main activities on Dynabook will be through handwriting, as done with a paper notebook. The pen gives a level of freedom to explore and to express ideas and thoughts unmatched by the restraining space of a phone screen or a computer keyboard. Nevertheless, there is no reason a student can't use their own phone when it is appropriate, and they will do so. However, trying to use handwriting on a phone, is like writing a dissertation on a stamp.

With little extra effort, the Dynabook app itself can be be made to work mostly identically on mobile devices. It was done more than 10 years ago with Dr. Geo on [Android tablet](https://www.dailymotion.com/video/xorui4) and [iPad iOS](https://www.dailymotion.com/video/xnp91c).

**---JR**: In one of the slides of your Buenos Aires speech you write, as one of the *iterations* of the project

> Develop Dynabook **operating system**

I hope this doesn't mean *develop from scratch*, but you might clarify it, above all the point whether the rest of the expected software (document editors, spreadsheets, browsers, gpg keys...) with be present.

**---HF**: This I don't know yet, there are plenty of Linux distributions to be based on. Linux Console only with framebuffer, while good on saving resources will be too narrow and it will not allow easily the use Web browser and office tool. So it will require a kind of 
Window manager to access the Dynabook app and other provided with the machine.

**---JR**: I still don't get it because some things are implicit and should be mentioned: you don't mean an OS from scratch, are you thinking of some GNU Linux derivative, of starting from some GNU Linux distribution? What should be included? You mention a web browser, an office tool... inside the smalltalk environment or standalone? What else should be included?

**---HF**: The Dynabook will be operated by a GNU Linux system, beside the Dynabook app what applications are to be included is still to be determined. And no, those will not be inside the Smalltalk windows.

**---JR**: Is the app integrated with the rest of the OS themes? (look, windows, dark/light modes..)

**---HF**: TBD

**---JR**: Is the app integrated with a learning environment?

**---HF**: Sort of, but with a gateway.

**---JR**: Can you explain this?

**---HF**: LMS would be used as back up, so maybe you want to use a very basic one. Most of the document exchange between educators and learners will be done in the classroom, on local wlan by direct dynabook to dynabook link.

# Deployment

**---JR**: Now some practical considerations. Who would install the Operating System in the device?

**---HF**: TBD. Depends on deployment policy I guess.

**---JR**: So a proposal must be written. What would be the ideal deployment?

**---HF**: Deployment is very contextual to how an education system is organized, if there are local human resources in the schools or if it's spread in a geographic area. But maybe you can elaborate on the idea?

**---JR**: Suppose a school has decided to try the Dynabook project. Who installs and configures the app? Is the process automatic or the person needs to follow a tutorial?

**---HF**: TBD locally.

**---JR**: What subjects (geometry...) can be explored with the app? Are activities available?

**---HF**: All taught subjects with dedicated dynamic knowledge model.

**---JR**: Where do they use the app? (IT lab, classroom, home, all of them?)

**---HF**: Classroom & home

**---JR**: What training do the teachers need to work with it? (use, develop tasks...) Who provides it?

**---HF**: TBD locally.

# Volunteers & Financing

**---JR**: Who would pay for the development?

**---HF**: TBD. Ideally all public institutions, through subscriptions,
donations, delegations or what suites their own constraints. Should be
flexible so all can participate to such a free software and hardware
project.

**---JR**: Now we come to the core problem of how we can convince educational institutions to support FOSS. FOSS has never had a marketing department, and the pressure of BigTech is overwhelming in our schools. What new arguments would convince a ministery, local authorities or the staff of a school that haven't convinced them during the last twenty years? What did we do wrong in FOSS advocacy in education and what could be done now?

**---HF**: This problem of lobbying is not something an individual can conduct or organize alone. I have no clue to give you, OFSET was created with this idea and failed. Nevertheless, if you stick to the consideration that advocating education institutions to support FLOSS is overwhelming, you end doing nothing. But it is true that at some time, an organization or foundation supporting the Dynabook project will be needed.

**---JR**: It's obvious that if we continue discussing these topics after more than twenty years we believe that something must be done, the danger is voluntarism. We can't do the same things again and again and expect a different result. We need a a critical analysis of the history of FOSS in education. Your project is the result of your analysis and my task in this discussion was simply to clarify the ideas and make visible the points we take for granted but maybe are not known by the possible readers.

It's been a very interesting discussion, and you have made some very clear statements:

> If you can't operate fluently with an electronic pen and hand writing, the project is to be abandoned and learner should use paper notebook
>
> Digital textbooks will be on the Dynabook. If not possible, don't use the Dynabook.
>
> The older proposals (...) failed because it was not teacher-centered but learner-centered with a lot of dazing romance. You want a system to be centered around its main prescriptor, the teacher. 

Do you stick to them? No nuances?

**---HF**: Handwriting, access to digital text books and be teacher centered are core features to Dynabook. If one of these features is missing, it will be a failure. At this stage of the prototyping (20/4/2024), I don't see the rational to discard one of them.

**---JR**: My view: handwriting is an important plus, free modifiable resources is a must (GNU, CC), and the *teacher* point of view (is it better?) is a pedagogical issue: the process is teaching/learning in a formal context, the school. Nothing especially new so far, but good to remind. What is original is the emphasis on free hardware and on the idea of the teachers and maybe the students going deep into how the educational resource was built. The common attitude of a teacher before a free resource is  'is this resource useful for my lesson plan?', 'how can I use it?', 'do I have to modify it and is it easy to do that?'. There are thousands of free resources, only some are knowledge models, OK, but what is your experience with your colleagues, are they ready to take the dive beyond reuse? And are teachers expected to go beyond reuse? I don't know if this makes the Dynabook a very niche project.

**---HF**: It would be a niche project if Dynabook were only about dynamic knowledge models. Based on my experience with young students, ["scripting Dr.Geo dynamic knowledge models" - jr: is this necessary here?], for a teacher to edit and test an existing text script would be as easy as editing a libreoffice document, may be even easier. More broadly, your questions echo the computer literacy in our modern IT society, and the Dynabook tries to address it in its fundamental conception by easing the access to computing.

One question you have not asked is who will develop the dynamic knowledge model which is fundamentally much more difficult than scripting a dynamic knowledge model.

**---JR**: I haven't asked because I'm afraid I know the answer - you, for the moment. A project like this needs the support of an organization to finance the hardware development and to write the code necessary to show the teachers that it pays to use the Dynabook. How many knowledge models are available so far, how many scripts, for how many different subjects? How many training offers for the teachers? How many examples of successful use in the classroom? Who will confront the BigTech lobbyists at the institutions and the staff rooms? They have finished, flashy solutions. Our solutions may be nearer the *fundamental conception* and are philosophically superior, but have an additional condition, they have to be usable and sufficient, and convincing. I understand that things have to start from a beginning, but the rest of the steps have to be seen down the road.

______________________________________________________________________

# Some links
[Oral History of Adele Goldberg](https://youtu.be/IGNiH85PLVg?si=HpbUQNGj1SU6rfwj)

[An Interview with Computing Pioneer Alan Kay](https://techland.time.com/2013/04/02/an-interview-with-computing-pioneer-alan-kay/)

[The Charisma Machine](https://mitpress.mit.edu/9780262537445/the-charisma-machine/) (an evaluation of the OLPC project)

[The Dynabook app](https://github.com/hilaire/dynabook)
