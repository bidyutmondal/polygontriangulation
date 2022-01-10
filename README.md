# PolygonTriangulation

The code written is based on modified earclipping method.
The algorithm consists of finding such an ear/triangle, removing it from the polygon
which results in a new polygon that still meets the conditions and repeating until there is only one triangle left.
The running time complexity of the code is O(n*n).
In this code we go through each vertex of the polygon and check if we can cutoff the ear/triangle from the polygon.
We cut an ear from a polygon only when the angle between two edges is less than 180 (i.e that part of the polygon is convex)
and there doesnot lie any point inside the ear/triangle so that when we draw diagonal it does not cut any edge or diagonal.
The checking condition of each vertex take O(n) time, so for n vertices of a polygon the time complexity becomes O(n*n).
Lastly, I sorted the output diagonal array using quicksort which takes O(nlogn) time.
So the total time complexity still remains O(n*n).
Please note that the output diagonal is in sorted order based on starting vertex.

The site is active on https://bidyutmondal.github.io/polygontriangulation/
