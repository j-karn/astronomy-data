# astronomy-data
This repository captures the assignments I did as part of the 6-week Data Driven Astronomy course using Python + SQL offered on Coursera by the University of Sydney.<br>
</br>
  <b>Week 1: Understanding and detecting Pulsars</b></br>
  <b>Task:</b> As pulsars give off very faint signals, astronomers use image stacking technique in order to detect the underlying signals. To do so, they find the mean brightness at each pixel of the images. This approach averages out the noise and enhances a bright spot revealing the potential pulsars.
  <br>
    <li>Uploading, opening, and cleaning csv and <a href="https://en.wikipedia.org/wiki/FITS">FITS</a> files</li>
    <li>Working with lists and arrays
    <li>Writing a function to calculate the mean of a set of potential pulsar signals</li>
    <b>Tools & Libraries</b> - pandas, numpy, astropy.io, matplotlib
<br></br>
  <b>Week 2: Cross matching between different astronomical catalogues</b></br>
   <b>Context:</b> When studying galaxies, it is crucial to review different parts of the electromagnetic spectrum to comprehensively understand the structure and composition of the galaxies. This means astronomers compare data about those objects from different telescopes at different wavelengths. This requires positional cross-matching to find the closest counterpart within a given radius on the sky.
   <br></br><b>Task:</b> Crossmatches between a radio survey catalogue (BSS) and an optical survey (SuperCOSMOS) to see how many of the bright radio sources in the BSS catalogue have a counterpart in the SuperCOSMOS.
  <br></br>
    <li>Import and work with csv and dat files</li>
    <li>Convert celestial coordinates to decimal degrees/ radian and calculate the angular difference between the objects</li>
    <li>Write a function to cross match between the two catalogues and output the matched objects that are within predefined maximum distance</li>
    <b>Tools & Libraries</b> - requests, numpy
<br></br>
  <b>Week 3: Querying database using SQL to answer questions around Exoplanets</b></br>
   <b>Task:</b>The goal this week is to use SQL syntax and command to find out answers regarding Exoplants.


   <br>1 Write an SQL query to find the radius and temperature of the stars in the Star table that are larger than our sun.
   <br>2 Write a range query which returns the kepler_id and the t_eff attributes of all those stars in the Star table whose temperature lies between 5000 and 6000 Kelvin (inclusive).
   <br>3 Write a query to find the kepler_name and radius of each planet in the Planet table which is a confirmed exoplanet, meaning that their kepler_name is not NULL, or, equivalently, whose status is 'CONFIRMED'.

Restrict your results to those planets whose radius lies between one and three earth radii, and remember that the radius of the planets is relative to the earth radius.
<br>4 Find min, max, avg, stdev radii
<br>5 Find out how many planets in the Planet database are in a multi-planet system. Planets sharing the same star will have the same kepler_id, but different koi_name values. Your query should return a table in which each row contains the kepler_id of the star and the number of planets orbiting that star (i.e. that share this kepler_id). Limit your results to counts above one and order the rows in descending order based on the number of planets.
6 Write a query that returns the radius of each star and planet pair whose radii have a ratio greater than the Sun-to-Earth radius ratio. Order the results in descending order based on the stellar radii. Use sun_radius and planet_radius as attribute aliases for the star and planet radii.
7 Write a query which counts the number of planets in each solar system where the corresponding stars are larger than our sun (i.e. their radius is larger than 1).</br>
  <br></br>
    <li>Aggregation - ```COUNT, MAX, MIN, SUM```</li>
    <li>```WHERE``` clause + ```HAVING```</li>
    <li>```IS NULL, IS NOT NULL```</li>
    <li>```JOIN.. ON + JOIN.. USING```</li>
    <li>```INNER + OUTER JOIN```</li>
<br></br>
 <b>Week 4: Managing database</b></br>
   <b>Task:</b> Continuing from last week, this week tasks involve using ```CREATE, INSERT, DELETE,``` and ```UPDATE``` command to manipulate a table's content.
  <br></br>
    <li>Import and work with csv and dat files</li>
    <li>Convert celestial coordinates to decimal degrees/ radian and calculating the angular difference between the objects</li>
    <li>Write a function to cross match between the two catalogues and output the matched objects that are within predefined maximum distance</li>
    <b>Tools & Libraries</b> - requests, numpy
<br></br>
  <b>Week 5: Using decision trees to predict the redshift of galaxies from the Sloan Digital Sky Survey</b></br>
   <b>Context:</b> To calculate the redshift of a distant galaxy, the most accurate method is to observe the optical emission lines and measure the shift in wavelength. However, this process can be time consuming and thus infeasible for large samples, not to mention the lack of spectroscopic observations on many galaxies.
   <br></br><b>Task i:</b> Use the flux magnitudes to create colour indices and calculate the redshift. Flux magnitudes are the total flux (or light) received in five frequency bands (u, g, r, i and z). The inputs to the decision tree are the colour indices (u-g, g-r, r-i and i-z) from photometric imaging and the output is a photometric redshift prediction. The training data uses accurate spectroscopic measurements.
  <br><b>Task ii:</b> Compare the predictions generated by the model with the actual values to test how well the model performs.
  <br><b>Task iii:</b> Split the data into training and testing subsets to validate the model.
  <br><b>Task iv:</b> Cross validate using KFold
    <li>Create an empty array using ```np.zero(x)```</li>
    <li>Suppress print out in scientific notation - ```np.set_printoptions```</li>
    <li>Understand the importance of ```abs```</li>
    <b>Tools & Libraries</b> - numpy array, DecisionTreeRegressor and KFold from scikit-learn
<br></br>
 <b>Week 6: Exploring machine learning classification</b></br>
   <b>Task:</b> Using DecisionTree to classify galaxies into three types (ellipticals, spirals or galactic mergers) based on their observed properties.
      <li>Split data into train and test set</li>
      <li>Shuffle the position of the indexes</li>
      <li>Generate features and targets</li>
      <li>Calculate accuracy</li>
      <b>Tools & Libraries</b> - numpy, DecisionTreeClassifier
