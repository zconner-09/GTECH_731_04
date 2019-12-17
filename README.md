# GTECH_731_04
Homework assignment 4 for GTECH 731. For this assignment, let's start working more with spatial data.  To start doing this, and to get a better feel for functions, what I would like you to do is to write a function that takes a list of points as a parameter, carries out  some operation on them, and returns a result, which can be a summary number or another geometry.
 
Since we already started doing this in the last assignment, this one can build on what you did before, by using the pluto geojson as input.  Or use a new set of points if you prefer.
 
Here are some suggestions:

1. Calculate the center point of each polygon.  Again, there are varied methods of doing this, and you could start simple and work up to area-weighted average, or other more sophisticated method.   The simplest would be the average x and average y.    Another would be the center of the bounding box (min x, min y, max x, max y), of the centroid function from the book or jupyter notebook.

2.  Do a spatial query - a function could take a point and a number to return, and return the top n closest buildings. 

3. Reproject the points to another projection.  See the projection function examples that we will have reviewed in class.  The Xiao book has some projection information, but delves into some more complex examples that may be challenging, but feel free to try these if you would like.

 4. Calculate the area / perimeter ratio of the tax lots.  It may be interesting to, for example, get the area / perimeter ratio, plot a histogram of these in matplotlib, and see if the distribution tells you something about your neighborhood.  Does the distribution change much for neighborhoods with a different layout?  To do this, you would need to calculate the distance from one point to another.  For simplicity's sake, it might be best to simply work in decimal degrees, or try the spherical distance function from the Xiao book.  The book includes the basic Euclidean distance function if you need a refresher.

5. If the data you're working with is point data, you could try a nearest neighbor analysis.  One is listed in page 178 of the textbook.
Any other similar problem that you are interested in looking at would be fine, just be sure to keep it simple and try to work it out in pseudocode first.  

