# Matplotlib-Plotting

# Plotting x and y points
The plot() function is used to draw points (markers) in a diagram.

By default, the plot() function draws a line from point to point. 

The function takes parameters fro specifying points in the diagram.

Parameter 1 is an array containing the points on the x-axis.

Parameter 2 is an array containing th epoints on the y-axis.

If we need to plot a line from (1, 3) to (8, 10), we have to pass two arrays [1, 8] and [3, 10] to the plot function.

Example

Draw a line in a diagram from position (1, 3) to position (8, 10):

    import matplotlib.pyplot as plt
    import numpy as np

    xpoints = np.array([1, 8])
    ypoints = np.array([3, 10])

    plt.plot(xpoints, ypoints)
    plt.show()

Show image result in the top file path like main.py in the near to READme.md file     

The x-axis in the horizontal axis.

The y-axis is the vertical axis.

# Plotting Without Line
To plot only the markers, you can use shortcut string notation parameter '0', which means 'rings'.

Example

Draw tow points in the diagram, one at position (1, 3) and one in position (8, 10):

    import matplotlib.pyplot as plt
    import numpy as np

    xpoints = np.array([1, 8])
    ypoints = np.array([3, 10])

    plt.plot(xpoints, ypoints, '0')
    plt.show()

Note: In the top you can see the result from a picture

# Multiple Points
You can plot as many points as you like, you make sure you have the same number of points in both axis.

Example 

Draw a line in a diagram from position (1, 3) to (2, 8) the to (6, 1) and finally to position (8, 10):

    import matplotlib.pyplot as plt
    import numpy as np

    xpoints = np.array([1, 2, 6, 8])
    ypoints = np.array([3, 8, 1, 10])

    plt.plot(xpoints, ypoints)
    plt.show()

Note: You can see the result in the top a picture even including file path    

# Default X-Points
If we do not specify the points on the x-axis, they will get the default values 0, 1, 2, 3(etc, depending on the length of the y-points.)

So, if we take the same example as above, and leav out the x-points, the diagram will look like this:

Example 

Plotting without x-points:

    import matplotlib.pyplot as plt
    import numpy as np

    ypoints = np.array([3, 8, 1, 10, 5, 7])

    plt.plot(ypoints)
    plt.show()

Note: You can see the result in the top a picture including 

