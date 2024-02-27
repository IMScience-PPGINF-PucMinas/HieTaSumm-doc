.. __fundamentals:


Fundamentals
============

Dynamic Variables
------------------

The ``options.json`` file is responsible for defining some variables used in the code and in defining the summary scope. 
The standard values used in the ``options.json`` file are listed below: 

.. code-block:: javascript 

    {
      "video_path": "./videos",
      "summary_path": "./summary",
      "percent": 15,
      "alpha": 75,
      "rate": 4,
      "time": 8,
      "hierarchy": "watershed_hierarchy_by_area",
      "selected_model": "resnet50",
      "is_binary": true,
      "keyshot": true, 
      "keyframe": true
    }

:video_path: define the path to the videos folder
:summary_path: define the summary result path 
:percent: defines the percentage of the original video that is represented by the summary
:alpha: changes the standard deviation
:rate: video rate
:time: video time 
:hierarchy: [watershed_hierarchy_by_area] defines the hierarchy used
:selected_model: [resnet50, vgg16] defines the model to extract features
:is_binary: [true, false] define if the graph is binary 

To change the values of the predefined variables you can pass the name followed by the value when calling the HieTaSumm method.

.. code-block:: python

    from HieTaSum import HieTaSum
    HieTaSum(video_path='localpath/to/your/video', percent=10)

`This notebook`_ is an example of this use case. 

The algorithm used is described in:

`"Hierarchical Time-aware Approach for Video Summarization"`_ Enhanced by Leonardo Vilela Cardoso, Silvio Jamil F. Guimarães and Zenilton K. G. Patrocínio Jr.

An example of the algorithm application is available in: 

`Hierarchical Time-Aware Summarization with an Adaptive Transformer for Video Captioning.`_ Enhanced by Leonardo Vilela Cardoso, Silvio Jamil F. Guimarães and Zenilton K. G. Patrocínio Jr.

.. _"Hierarchical Time-aware Approach for Video Summarization": https://link.springer.com/chapter/10.1007/978-3-031-45368-7_18
.. _This notebook: https://colab.research.google.com/github/IMScience-PPGINF-PucMinas/HieTaSumm-examples/blob/main/Updating-the-dynamic-variables/Updating-the-dynamic-variables.ipynb
.. _Hierarchical Time-Aware Summarization with an Adaptive Transformer for Video Captioning: https://openurl.ebsco.com/EPDB%3Agcd%3A12%3A12367964/detailv2?sid=ebsco%3Aplink%3Ascholar&id=ebsco%3Agcd%3A173810537&crl=c