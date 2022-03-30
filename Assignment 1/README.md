# The Auckland Road System

This assignment involved builing a program that lets a user view and search the 
Auckland Road system. For this assignment, I had to build a program that read a 
collection of files containing information about the roads in the Auckland 
region, displaiyed the information visually, and let the user view and search the 
data in several ways. The program needed to have several large data structures, 
and the key challenge of the assignment was to implement those data structures.

The Program had to:
  -   Read road data from files and construct an appropriate data structure to 
  store all the information about the road, road segments, and intersections.
  A road segment is a part of a road that connects two intersections. A road 
  consists of a sequence of road segments. Intersections are either places where
  two roads meet, or the end of a road. The data structure must include a graph
  of the intersection (nodes) and the road segments (edges), but it will also need
  to store information about the roads.
  -   Display the road data visually by drawing lines for all the roads segments. 
  Each road segment should be drawn as a sequence of straight lines (the points 
  along the road are specified in the data files). The program must allow the 
  user to either view the whole of the Auckland region, or zoom in on a smaller 
  region. At the minimum, the program should have two views - the whole region 
  and Auckland central. Ideally, the user should be able to zoom and pan to 
  arbitrary views of the data.
  -   Allow the user to enter the name of a road in a text box, and then highlight
  the road (all its road segments). To do this, the program should store all the 
  road names in a trie structure which will act as a searchable index into the 
  collection of road objects.
  -   Allow the user to click on the visual display of the roads, and then 
  highlight and display information about the closest intersection. The 
  information should include the location of the intersection and all the roads 
  that go through the intersection.
  
  ![](Assignment%201%20Small%20Graph.png)
  ![](Assignment%201%20Large%20Graph.png)
