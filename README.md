# Successful Movie Analysis
Group 6
Team members: Zane Rios, Gino Hernandez, Kristal Concepcion

We set out to determine what were the key aspects that lead to a successful movie. To do this there are a few factors to consider. First we needed to answer questions relating to movie themes and genres. Once this was done we needed to collect multiple datasets, transform them into key aspects/fields, and load it into a singular readable dataset for comparing and analyzing.

### Data Sets
* We pulled our conclusions from two data sets. The first was a csv file with movie titles from 2022, their release date, and rating. The second we created ourselves by web scraping from BoxOfficeMojo.com, we pulled information that was missing from the original csv file such as genre, publishing studio, and gross. 
* To clean the original csv file we had to drop unnecessary columns such as ‘original language’, ‘original title’, and any rows that had blank information as we needed movies with complete data. To compile the information we needed from BoxOfficeMojo.com we used BeautifulSoup to scrape 2022 movies, their genre, gross, and studio company. Then we exported both of these datasets as csv files. 

### Final Summary Notes:

 * We set out to determine what were the key aspects that lead to a successful movie. To do this there are a few factors to consider. First we needed to answer questions relating to movie themes and genres. Once this was done we needed to collect multiple datasets, transform them into key aspects/fields, and load it into a singular readable dataset for comparing and analyzing.
* We pulled our conclusions from two data sets. The first was a csv file with movie titles from 2022, their release date, and rating. The second we created ourselves by web scraping from BoxOfficeMojo.com, we pulled information that was missing from the original csv file such as genre, publishing studio, and gross. 
* To clean the original csv file we had to drop unnecessary columns such as ‘original language’, ‘original title’, and any rows that had blank information as we needed movies with complete data. To compile the information we needed from BoxOfficeMojo.com we used BeautifulSoup to scrape 2022 movies, gross, and studio company. Then we exported both of these datasets as csv files. 
* After we cleaned up the two datafiles we merged them together on their common titles to get a single dataframe with complete data for each movie. This dropped any movies that were missing any data so we could only look at completed data. The final dataframe ended up with popularity, vote average, release month, release year, and rank that we got from the first csv file, then the scraped data columns that included studio company, release, and gross. This complete dataframe was loaded it into pgAdmin as workable database
