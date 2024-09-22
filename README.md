## Smart India Hackathon -2020 for ISRO
### Gagan - Image Masking and Solar Energy Analysis
Solar energy is a vital source of electricity and an initiative for clean and renewable energy production. Solar energy potential at a particular region can be found efficiently by detecting local sky horizon. This technique involves separation of sky pixels and identifying the terrain from the image which could potentially obstruct the sun rays. 

With the help of our application “Vyomang”, users can capture or upload an image through their devices. The image is uploaded to the cloud server and masked to a sky-ground image using Machine Learning techniques such as k-means clustering and semantic segmentation. 

At the end, along with the binary masked image, a detailed statistical report showing the variations in the energy potential across different seasons and weather conditions is produced. This helps the user to understand and develop an efficient energy policy for solar energy consumption.



### **Installation Guide**

The given file is in the format of .ipynb which cannot be opened using any notebook such as Google colab, jupyter, Kaggle etc.

The step by step description of the code written are explained in the markdowns.

Requirements:

Additionally you might need to install:

    1.PIL    
    2.opencv    
    3.pvlib

And any other module if found lacking in the notebook.

The file to execute properly might require 2 files

 1. Input image to be masked
 2. Data of usage of electrical appliances in the csv format.
 
Upload the appliances.csv file and any test image from the zip file to the root folder of the source code.

Make sure to change the name of the input image in the first code block near input_file identifier.

The code uses static input for the optics and coordinate calculations.

The focal length and pixel levels are input from a standard Motorola smartphone but could be dynamically extracted from the device the application will run on.

The coordinated which are given as a static input could be extracted dynamically using GPS module in the smartphone.

The output of the code could be seen after various code blocks that include:

1. Masked image

2. Lowest sky pixels on the image

3. Angles of elevation for each lowest sky pixel

4. Optimum elevation angles for different seasons

5. Provision for solar panels

6. Height of solar panels

7. Solar energy potential

8. No. of panels required based on the need of the client.

9. Energy estimation based on usage.

*Note: The code could be further optimized by using semantic segmentation with the help of deep neural networks and linking the code to the cloud so as to dynamically produced the result by a server request by any handheld device.*
