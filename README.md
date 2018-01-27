# AI-Law-Minicourse-HW

## Notes

### Step 1 - Data Collection & Preparation

* The code imports packages from Anaconda. Consider HTTP request (user agent requirement).
* Link url from caselaw to create a list of Supreme Court documents and assign all requested cases to a variable.
* The codes then modifies the variable concerning the year of the judgment and executes the URL request to obtain the requested decisions. 
* Define a method to create a data frame table.
* The code results in displaying the year in the data frame table. By clicking on the year you are able to see all decisions of the corresponding year.
* Check table values.

### Step 2 - Data Collection & Preparation

* Import packages.
* The code implements the output of Step 1. 
* In order to avoid too many hits on the website, we devide the request into three sections.
* The code implements the describtion of each case, which you can request if you are clicking on the specific dataset. 
* Adding scraped data (case details) to frame table. 
* Save project!

### Step 3 - Data Processing

* Receive more exact outcomes by importing a stopword list and assigning variables to common words.
* Afterwards all those words are lemmatized and the stoplist is applied.
* The text is now cleaned.

### Step 4 - Topic Modeling Method Testing

* Test the current model with LatentDirichletAllocation, Non-negative Matrix Factorization and Latent Semantic Analysis. 
* Apply those topic modeling methods and check if you reach the right result. 

### Step 5 - Topic Model Application to Data

1. Step: run the model against the entire dataframe to collect the topics
* By executing this code, all case descriptions are stacked together to receive one document consisting of all decisions.
2. Step: take this model and apply it back to the dataframe to assign most likely topic to each case 
* The topic modeling methods result specific probabilities which relate to the different topics. 
3. Step: make a dictionary of the components that make up each topic from the original model
* The code creates a dictionary for each topic consisting of 30 words. 
4. Step: use this dictionary to "look up" the topic components and apply those to the dataframe
* The applied code searches for the words of each topic dictionary in the dataframe. 
5. Step: Getting data together for visualization!
* Pivot data in order to visualize it (creating data point for every topic, for every year).
* Fin!
