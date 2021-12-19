# Data

## Stitch Overview

The problem in combining customer data with a disparate set of data sources, is that we can rarely find a common, unique key that links all records that belongs to an entity. This is the fundamental reason why identity resolution is required.

Graph-based entity resolution algorithms have emerged as a highly effective approach including utilization of Apache Spark  and GraphFrames. The technique will exhibit an example where efficacy can be achieved based on simple heuristics, and at the same time map a path to a machine-learning assisted entity resolution engine with a powerful knowledge graph at its center.

![image](https://user-images.githubusercontent.com/93347291/146683244-18dc6fdd-254a-4c6a-ba9e-9916737ae9dd.png)

SkyPoint’s approach to identity resolution produces rich, accurate, and precise customer 360 profiles. There are Three steps in the process of building customer 360 profiles.

# Step I: Map (Data preperation)

All of the initial work needed to get data into a Common Data Model (CDM) and prepare it for the match process.

The stitch process begins by ingesting data from multiple sources known as DataFlow. Once the DataFlow is successful, the first phase is to *map* the data columns ( Attributes of ingested data) with their semantic labels (CDM). Semantic labels help us to match the attributes semantically using advanced machine learning techniques.

# Step II: Match ( Match attibutes across entities to CDM)

Identity resolution is the process of matching identifiers across disperate datasets and touchpoints to a single profile. This helps build a cohesive, longitudinal view of a consumer, enabling brands to deliver relevant messaging throughout the customer journey.

Match process can be handled in two differnt ways

## a. Rule match (Static Rule approach)

In this approach, user has to manually select the rules based on which the algorithm will be applied. Here user can also select the match precision, for example exact match or Fuzzy match.
   1. Exact Match
      - When selecting Exact match, in built rule will find an exact match to resolve identity. Certain transformations like removing unwanted white spaces, trimming the text, lowercase, data formats etc can be applies. Identities will be considered a match only when they are exactly same after the transformation
   2. Partial/Fuzzy Match
      - When user selects, match precision as High/Medium/low, they gets the option to select which kind of algorithm they want to apply.
      - Currently SkyPoint Supports, Phonetic match, distance based Levenshtein match.
      - User can select Phonetic match over the column in which a match would be considered true when both the matching values are phonetically similar. ex- Dylan and Dillon
      - Distance based Levenshtein is a dynamic programming based approach and one of the most used approach for good quality matches. In the approach, two values are considered to be a match when converting from one value to another, requires less number of transactions. ex- Tony and Tonyy. Converting Tony to Tonyy requires only 1 transactions. Addition of 1 Y. 1 Transaction can be either update, delete, addition  

## b. ML Match (Machine Learning based matching)

![image](https://user-images.githubusercontent.com/93347291/146683903-33a03452-94b8-4ec4-bc9f-d1fe2e34af60.png)

In this approach Machine learning algorithms match the identities based on Data completeness and Match confidence threshold set. The semantic labeling of attributes is automatically handled by the algorithm. User can review and align the mapping by selecting a more appropriate semantic label or by creating a customer label before Running the match

ML match, being a more convenient way of mapping the attributes, is preferred over Rule match

# Step III: Merge (Merge matching records to create unique profiles)

The last step in the process of identity reselution is Merge. In this step, profiles identified to have matched either based on the Rule Match algorithms or the ML Match algorithms are created into clusters. Each cluster will be merged into one entity creating a unique and longitudinal customer profile. Once the Merge process is complete Unique profiles can be viewed Insight -> Profile

![image](https://user-images.githubusercontent.com/93347291/146684269-7e876782-4f42-450c-a527-34463bf7e842.png)

Removed from profile tab will display those records which were removed from the merge process primarily due to lack of quality data in the key attributes which can help the algorithm identify profiles uniquely

