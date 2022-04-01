# The Auckland Road System v2

This assignment extends [Assignment 1](/Assignment%201) to provide the user with two tools: route finding using A*
search, and critical intersection identification with the Articulation Point Algorithm.

The Program had to:
  -   Create a route finding tool like that in Google Maps or car navigation systems. This should allow the user to specify two intersection on the map and will then find (using A* search) and display the shortest route between those two locations. It should highlight the route on the map (by colouring all the road segments along the route) and should also output a list of all the roads along the route, along with the length of each part of the route and the total length of the route. The user should also be able to choose between the shortest route or the quickest route and it should take into account the restrictions (eg. no right turn).
  -   Identify every intersection that would have bad consequences for emergency services if it were blocked or disabled in some way. An intersection that is the only entrance into some part of the map is a critical intersection ('articulation points'). These points should be highlighted. Note: emergancy services don't care about restrictions.
