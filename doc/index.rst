.. procedural_city_generation documentation master file, created by
   sphinx-quickstart on Fri Aug 21 11:27:23 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Procedural City Generation in Python - Documentation 
======================================================
Welcome to procedural_city_generation's documentation! In this page we will give an overview of all the things you need to know to get started  with this project. 
 
* `Getting it to work`_
* `Indices and tables`_



Getting it to work
--------------------
You can get the source code at our `Github Page <https://github.com/josauder/procedural_city_generation>`_
with::
	git clone https://github.com/josauder/procedural_city_generation.git

**Dependencies:**

* numpy
* scipy
* matplotlib
* Blender 2.69

To start the program with the GUI::

	cd procedural_city_generation
	python GUI

If everything worked so far, the GUI should open up and look like this:

.. figure::  images/GUI.jpg
   :align:   center

Overview of the structure
--------------------------

Roadmap Creation
++++++++++++++++
We refer to "road segments" as edges and the two ends of an edge as a vertex.
We create roadmaps by starting with an axiom (a list of Vertices) and defining a set of rules by which new Vertices are added and connected to existing one to form Edges. 
Many of the terms used here become obvious when you see them in action. Let's start by showing the most important inputs:

**The Growth-Rule Image:**

.. figure::  images/growth-rule.png
   :align:   center

This image describes which growth rule will be used in which area. Blue means that the radial rule will be used, Red means that the grid rule will be used, and Green means that the natural rule will be used. We will discuss the rules in detail later.

**The Population-Density Image:**

.. figure::  images/population-density.png
   :align:   center

This image describes the probabilities that vertices will be connected at all. The lighter, the more probable it is, that an edge will be built. 

**The output**

.. figure:: images/roadmap.png
   :align:   center
   
This is what the finished roadmap for a relatively small city looks like. As you see there are main roads and minor roads. The correlation between the input and the output is also very clear in this example.

**Correlation between input and output**

.. figure:: images/result.png
   :align:   left
.. figure:: images/result2.png
   :align:   right


It should now have become clearer as to what the growth rules and the population density actually describe. 






Polygon extraction and subdivision
+++++++++++++++++++++++++++++++++++
This is some text describing how we extract and subdivide polygons

Creation of 3D Data
++++++++++++++++++++
This is some text describing how we create 3D Data

Visualization in Blender
++++++++++++++++++++++++++
This is some text describing how we use Blender



.. toctree::
   :maxdepth: 2

.. procedural_city_generation


Indices and tables
==================

* :ref:`modindex`
* :ref:`search`
* :ref:`genindex`