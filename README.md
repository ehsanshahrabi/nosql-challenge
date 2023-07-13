# Eat Safe, Love - UK Food Hygiene Ratings Analysis

Food critics and journalists face the ever-challenging task of finding fresh establishments to cover in their articles. With this in mind, we embarked on a journey to analyze the food hygiene ratings of various eateries across the United Kingdom. We believe that the ratings, evaluated and presented by the UK Food Standards Agency, will serve as a valuable resource for the team of the food magazine, Eat Safe, Love.

his repository contains two Jupyter notebooks that meticulously guide you through our analysis.

NoSQL_setup_starter.ipynb: Here, you'll witness how we paved our way into the world of NoSQL databases, imported our data, and prepared it for the impending examination.

NoSQL_analysis_starter.ipynb: This notebook brims with exploratory analysis. It delves deep into the dataset and uncovers answers to intriguing questions that will aid the Eat Safe, Love team in choosing the bestestablishments for their next features.

### Data

Our source of information is the establishments.json file, a treasure trove teeming with details about the establishments. It spills secrets about the establishments' names, types, addresses, hygiene scores, rating value, geolocation, and much more.

### Database

To manage this vast array of information, we've chosen MongoDB, a NoSQL database revered for its agility and scalability. The establishments.json file breathes life into a MongoDB database named uk_food, populating the collection establishments.

### Data Preparation

Before plunging into the exploration, the data undergoes a rigorous preparation process. This includes:

Creating new entries: Our analysis would be incomplete without considering the latest culinary spots. Therefore, we ensure to insert new entries, such as the recently opened "Penang Flavours" restaurant.

Updating existing entries: Information changes, and we make sure our data does too. For example, we updated the "BusinessTypeID" of the newly added restaurant.

Eliminating unrequired entries: To maintain focus on the areas of interest, we removed establishments in areas not under consideration. An example is the deletion of establishments from the "Dover" local authority area.

Data type rectification: Data should speak the same language. We've converted number values mistakenly stored as strings back to their numeric form.

### Exploratory Analysis

Our analysis brings to light answers to a host of questions that will benefit Eat Safe, Love. Each query's result is displayed via count_documents for the document count, pprint for the first document, and a Pandas DataFrame showcasing the first ten rows. Here's a sneak peek into our explorations:

#### Identifying establishments with a hygiene score equal to 20

Result: 41 establishments make the cut.

#### Spotting establishments in London boasting a RatingValue greater than or equal to 4

Result: London proudly hosts 33 such establishments.

#### Unveiling the top 5 establishments with a RatingValue of 5, closest to the new restaurant "Penang Flavours", and sorted by the lowest hygiene score

Result: The notebook reveals the top contenders.

#### Counting establishments in each Local Authority area that proudly bear a hygiene score of 0

Result: 55 Local Authority areas host such establishments.

Please refer to the NoSQL_setup_starter.ipynb and NoSQL_analysis_starter.ipynb Jupyter notebooks for a detailed rundown of our code, results, and analysis.
