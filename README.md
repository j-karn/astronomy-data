# astronomy-data
This repository captures the assignments I did as part of the 6-week Data Driven Astronomy course using Python + SQL offered on Coursera by the University of Sydney.<br>
</br>
  <b><u>Week 1</u>: Understanding and detecting Pulsars</b></br>
  <b>Context:</b> As pulsars give off very faint signals, astronomers use image stacking technique in order to detect the underlying signals. To do so, they find the mean brightness at each pixel of the images. This approach averages out the noise and enhances a bright spot revealing the potential pulsars.
  <br>
    <li>Upload, open, and clean csv and <a href="https://en.wikipedia.org/wiki/FITS">FITS</a> files</li>
    <li>Work with lists and arrays
    <li>Write a function to calculate the mean of a set of potential pulsar signals</li>
    <b>Tools & Libraries</b> - pandas, numpy, astropy.io, matplotlib
<br></br>
  <b>Week 2: Cross matching between different astronomical catalogues</b></br>
   <b>Context:</b> When studying galaxies, it is crucial to review different parts of the electromagnetic spectrum to comprehensively understand the structure and composition of the galaxies. This means astronomers compare data of those objects from different telescopes at different wavelengths which requires positional crossmatching to find the closest counterpart within a given radius on the sky.
   <br></br><b>Task:</b> Crossmatch between a radio survey catalogue (BSS) and an optical survey (SuperCOSMOS) to see how many of the bright radio sources in the BSS catalogue have a counterpart in the SuperCOSMOS.
  <br></br>
    <li>Import and work with csv and dat files</li>
    <li>Convert celestial coordinates to decimal degrees/ radian and calculate the angular difference between the objects</li>
    <li>Write a function to cross match between the two catalogues and output the matched objects that are within predefined maximum distance</li>
    <b>Tools & Libraries</b> - numpy, operator
<br></br>
  <b>Week 3: Querying database using SQL to answer questions around Exoplanets</b> - <a href="https://github.com/j-karn/astronomy-data/blob/main/Week_3_Querying_database_using_SQL_to_answer_questions_around_Exoplanets.ipynb" target="_blank" rel="noopener noreferrer">Link</a></br>
   <b>Task:</b>The goal this week is to use SQL syntax and command to find out answers regarding Exoplants.
    <li>Aggregation - ```COUNT, MAX, MIN, SUM```</li>
    <li>```WHERE``` clause + ```HAVING```</li>
    <li>```IS NULL, IS NOT NULL```</li>
    <li>```JOIN.. ON + JOIN.. USING```</li>
    <li>```INNER + OUTER JOIN```</li>
<br></br>
 <b>Week 4: Managing database</b> - <a href="https://github.com/j-karn/astronomy-data/blob/main/Week_4_Managing_database.ipynb" target="_blank" rel="noopener noreferrer">Link</a></br>
   <b>Task:</b> Continuing from last week, this week tasks involve using ```CREATE, INSERT, DELETE,``` and ```UPDATE``` command to manipulate a table's content.
    <li>command</li>
    <li>command</li>
    <li>command</li>
<br></br>
  <b>Week 5: Using decision trees to predict the redshift of galaxies from the Sloan Digital Sky Survey</b> - <a href="https://github.com/j-karn/astronomy-data/blob/main/Week_5_Predicting_the_redshifts.ipynb" target="_blank" rel="noopener noreferrer">Link</a></br></br>
   <b>Context:</b> To calculate the redshift of a distant galaxy, the most accurate method is to observe the optical emission lines and measure the shift in wavelength. However, this process can be time consuming and thus infeasible for large samples, not to mention the lack of spectroscopic observations on many galaxies.
   <br></br><b>Task:</b> Use the flux magnitudes to create colour indices and calculate the redshift. Flux magnitudes are the total flux (or light) received in five frequency bands (u, g, r, i and z). The inputs to the decision tree are the colour indices (u-g, g-r, r-i and i-z) from photometric imaging and the output is a photometric redshift prediction. The training data uses accurate spectroscopic measurements.
    <li>Import and work with npy file</li>
    <li>Compare the predictions generated by the model with the actual values to test how well the model performs</li>
    <li>Split the data into training and testing subsets to validate the model</li>
    <li>Cross validate using KFold</li>
    <li>Understand the importance of ```abs```</li>
    <b>Tools & Libraries</b> - numpy array, DecisionTreeRegressor and KFold from scikit-learn
<br></br>
 <b>Week 6: Exploring machine learning classification</b> - <a href="https://github.com/j-karn/astronomy-data/blob/main/Week_6_Galaxy_classification.ipynb" target="_blank" rel="noopener noreferrer">Link</a></br>
   <b>Task:</b> Using DecisionTree and RandomForest to classify galaxies into three types (ellipticals, spirals or galactic mergers) based on their observed properties.
      <li>Import and work with npy file</li>
      <li>Generate features and targets</li>
      <li>Fit data into models</li>
      <li>Calculate accuracy and visualise using confusion matrix</li>
      <b>Tools & Libraries</b> - numpy, DecisionTreeClassifier, RandomForestClassifier, matplotlib
