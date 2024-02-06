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
:percent:
:alpha: changes the standard deviation
:rate: video rate
:time: video time 
:hierarchy: [watershed_hierarchy_by_area] defines the hierarchy used
:selected_model: [resnet50, vgg16] defines the model to extract features
:is_binary: [true, false] define if the graph is binary 

To change the values of the predefined variables you have to indicate the path to the file that contains the specifications as mentioned in the early section.

.. code-block:: python

    from HieTaSum import HieTaSum
    HieTaSum(path_file_param=’your_json_file’)

This notebook is an example of this use case. 


