# Visualize Data with Amazon QuickSight

## Introducing this Project!

In this project, I uploaded data into an S3 bucket and created different visualizations using Amazon Quicksight.

### Services Used

- S3
- QuickSight

### Concepts Learnt

- About manifest.json
- Connecting QuickSight with S3
- Creating different visualizations on QuickSight

### Architecture Diagram

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS0.png)

---

## Project Guide

### Step 1: Upload the Dataset file and Manifest file in S3

First, I navigated to S3 and set my region as the one closest to my geographical location (ap-south-1).

I then created my bucket with a globally unique bucket name ('nextwork-quicksight-project-sumeetsd') and uploaded the dataset file ('netflix_titles.csv') into my bucket.

Next, I copied the S3 URL of the dataset file and pasted it in the manifest.json file and then also uploaded the manifest.json file into my bucket.

A screenshot of the created bucket and the uploaded objects is shown below.

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS1.JPG)

### Step 2: Sign up for QuickSight

I signed up for QuickSight using the same email address that I used for my AWS account, selected the same region as that of my S3 bucket (ap-south-1) as the QuickSight region, and gave QuickSight the access to the S3 service. (**Very important: To avoid getting heavily charged, I de-selected the 'Add Pixel-Perfect Reports' add-on during sign up and deleted my QuickSight account after completing this project.**).

A screenshot of the successfull account creation page is shown below.

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS2.JPG)

### Step 3: Connect QuickSight with the S3 bucket

I navigated to the Datasets tab on QuickSight and created a new dataset with S3 as the data source and the S3 URL of the manifest.json file as the manifest file, as shown in the below screenshot, to complete the process of connecting QuickSight with my S3 bucket.

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS3.JPG)

### Step 4: Create the Visualizations on QuickSight

QuickSight allows us to sort, filter, or customise our data to create different visualizations. We can also experiment with different types of graphs such as bar charts, pie charts, and line graphs.

I created some visualizations by experimenting with the 'Data' and 'Visuals' sections on QuickSight, as shown in the below screenshots.

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS4.JPG)

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS5.JPG)

### Step 5: Solve some Use Cases and Publish the Dashboard

I created visualizations to solve the below use cases.
1. "I quite like the breakdown of TV shows/movies for each release year. Would it be possible to stack movies and TV shows in the same row, so you can visualise the % of each?"
2. "Now can you show me the same thing in a table? i.e. please show me the number of movies vs TV shows per release year in a table."
3. "On what day did Netflix add the largest number of movies/TV shows to their catalogue?"
4. "Of the TV shows and movies featured, how many were listed as 'Action & Adventure', 'TV Comedies', or 'Thrillers'? For simplicity, ignore the TV shows and movies that have multiple listings/categories."
5. "Of the TV shows and movies with the listing 'Action & Adventure', 'TV Comedies', or 'Thrillers', how many were released on 2015 or after?"

Finally, I gave some finishing touches to all the visualizations (resizing, labelling, etc.) and published the finalized dashboard, as shown in the below screenshot.

![Image](https://github.com/sumeet15n/visualizations-with-QuickSight/blob/master/Screenshots/SS6.JPG)

### Step 6: Delete Resources

Finally, I deleted all the created resources after completing this project to avoid any further charges on AWS.

---

## Project Reflection

This project took me approximately 2 hours to complete. The most challenging part was understanding how the manifest.json file works, and the most rewarding part was to see the final dashboard.

Big thanks to NextWork (https://www.nextwork.org/) for this project! I highly recommend this platform to anyone who wants to learn DevOps concepts and complete more projects like this one. The project guides on the platform are detailed, along with a walkthrough YouTube video for each project. Happy learning!