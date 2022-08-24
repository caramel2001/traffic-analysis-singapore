<h1 align="center">Taxi Availability Singapore</h1>

<p align="center">
 <font color='green'>We're interested in seeing how traffic levels have changed between Jan 2019 - a normal year, and Jan 2020 - a COVID year in Singapore.

The hypothesis is that the levels have dropped, and we're determined to find out through looking at the traffic cameras and computer vision.
</font>

</p>

## 📝 Table of Contents

- [Data](#problem_statement)
- [Flow of project](#project)
- [Part 1 - Data Collection and Mining](#1)
- [Part 2 - Data Cleaning](#2)
- [Part 3 - Data Engineering](#3)
- [part 4 - Machine Learning](#4)
- [Acknowledgments](#acknowledgments)

## 🗂 Data <a name = "problem_statement"></a>

The data is from Singapore government provided API at https://data.gov.sg/dataset/traffic-images .

## Flow of project <a name = "project"></a>

1. Explore Singapore's traffic camera API and map the locations of the cameras (Part I)
2. Make two one-month API calls to collect the initial data (Part II)
3. Collecting massive amounts of image data from API (Part III)
4. Prepare for GPU-enabled object detection (Part III)
5. Using computer vision to count traffic in 2019 and 2020 (Part IV)
6. Compare the traffic between two years (Part V)

## Part 1 <a name = "1"></a>

- Explore the traffic camera API from Singapore's Data.gov.sg
- Map the locations of the traffic camera in Singapore
- Identify the best camera to focus on for data collection

## Part 2 <a name = "2"></a>

- Collect two years' worth of traffic image JSON
- Combine the eventual DataFrame
- Filter for camera ID 1709 only
- Export DataFrame for Part III

### Part 3 <a name = "3"></a>

- Write a function to download images into drive
- Execute the function concurrently
- Prepare for OpenCV GPU execution in Part IV

### Part 4 <a name = "4"></a>

- Test object detection on one image
- Detect number of objects in all images
- Updating the DataFrames with the vehicle count

### Part 5 <a name = "5"></a>

- Transform and simplify the DataFrames
- Plot the respective num_cars over time

## 🎉 Acknowledgments <a name = "acknowledgments"></a>

- Tribe Academy
