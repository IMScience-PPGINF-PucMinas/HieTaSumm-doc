.. __fundamentals:


Fundamentals
============

Concepts
------------------

HieTaSum is an approach for summarizing videos dynamically. The package uses graph hierarchy concepts to define keyframes and, consequently, keyshots, generating a summary for the original video. 
It is an approach based on unsupervised learning, using the cosine similarity between each frame, forming an undirected graph as a result in which the weight of each edge is the result of the cosine of the similarity.
From the graph generated, we compute the hierarchy using the watershed method by area and, finally, we cut the graph, keeping only the keyframes and obtaining the video summary.

The algorithm used is described in:
`"Hierarchical Time-aware Approach for Video Summarization"`_ Enhanced by Leonardo Vilela Cardoso, Silvio Jamil F. Guimarães and Zenilton K. G. Patrocínio Jr,

.. code-block:: python

    from HieTaSum import HieTaSum
    HieTaSum()

Summarizes a video or a set of videos following the concepts mentioned, generating a video as result. 

*Parameters*: 
    path_file_param indicates the path to the json file that contains the dynamic variables 
*Returns*: 
	A folder containing the summarized video

.. _"Hierarchical Time-aware Approach for Video Summarization": https://link.springer.com/chapter/10.1007/978-3-031-45368-7_18