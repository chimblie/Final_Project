# Final_Project
Self-Assessment 
For this project, I was grouped with 2 other classmates. First, we discussed what topic we wanted to talk about. We came up with a few topics then we narrowed it down to 3. After a long discussion we decided to go with Art. We decided on art because there are a lot of data/datasets available to test different scenarios and theories.
My role was to create visualizations using Tableau. I chose Tableau because it is one of the most popular data visualizations tools out there. During the project, I encountered a few challenges. One of them was that I wanted to create a map that shows the countries or regions where the artists are from. To do that, I need to know the latitude and longitude, but my data did not provide it. So, I got a little frustrated, but I did not give up. I did a little research, and I was able to figure out how to do it. 
 image.png
My contributions to the roles I didn’t play was first, when I team member that was assigned to create the diagrams on quick DBD would have a doubt or did not know if a column was a varchar or integer. Then I would tell her if I knew on the top of my head and if I didn’t know I offered to look it up. Another team member was getting an error message when she was creating the tables on SQL. The error message read “extra data after last expected column”. When we got together via Zoom and she shared her screen, I looked at the table and suggested that she should increase the numbers of varchar and see what could happen. She did and it worked. See the image below.
 image.png
For the “Title” she had VARCHAR (700) that’s why she was getting the error, but when she increased it to 1000 it worked. 
To summarize our project, it was quite interesting. We chose to talk art because we left the art is a global phenomenon and we were able to find a lot of datasets to choose from.  We worked very well as collaborators. We communicated mainly via slack and zoom, and it worked perfectly. We wouldn’t do it any other way. For the team strength, it seems to be cleaning data using python. Our dataset (Artwork) had about 5.5% of pieces with multiples artists. For our analysis, we wanted to look only at pieces with one artist, so we dropped the rows that had pieces with multiples artists. 
 image.png
While analyzing our data, we found out that the number of female artists is significatively low compared to the male artists, as the image below shows.
 image.png
For that reason, we decided to create a plot to see how the percentage of female artists has increased over the years. From the plot, we can see that the number of female artists has skyrocketed in the 2000’s. 
image.png
 
As for our machine learning model, we used the Supervised Naive RandomOverSampling model. Our goal was to create a model that predicts the likelihood of a piece of artwork being cataloged. We started by importing our dependencies and loading the data. After loading the data, we removed all unnecessary columns and dropped all columns with Null values.
With our clean data, we created our features, target, and trained the data.
image.png 
 image.png
And finally, we calculated the balanced accuracy score and printed the imbalanced classification report.
 image.png
 
The balance accuracy score is about 65%. The likelihood of an artwork being cataloged is 87% with 66% sensitivity which makes a F1 of 74%. Since the likelihood of an artwork NOT being cataloged is only 33%, we can say that our model is a good one.






