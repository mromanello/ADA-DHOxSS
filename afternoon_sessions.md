# Afternoon sessions

## Exercises

### Day 1

Create a new notebook in binder or locally and work on the film database or crypto art dataset (or both) and import them. Make sure you understand the structure of the data as it comes.

### Day 2

Consider the dataset on contracts of apprenticeship in Venice: is it sufficiently tidy? If not, work on tidying it up: first, create a UML schema on it (use pen and paper), then implement it in a new notebook. What are the benefits of your design over the original?

*Hint: you might want to start from considering which observation types are in the dataset now (all within the same table) and thus which variables (columns) might be redundant. Examples include the profession categorization and the masters.*

### Day 3

Consider the film database. It is organised into several tables: practice wrangling techniques on them, making sure you can do the following at ease:
* concatenate, merge and join tables
* order tables
* group observations and calculate summary statistics
* do basic plots (e.g., histograms)

### Day 4

Consider any dataset you like and perform an exploratory data analysis on it. Start by stating some general questions you would like to provide an answer to, based on your knowledge of the dataset and your interests. State them down in a new notebook, and then go about answering them using descriptive statistics, correlations and visualizations.

# Project ideas

* African-American Film database: what can we learn about the production of African-American films by exploring this dataset? To what kind of sub-genres do these films belong to? Were these films produced by companies owned by white or african-american? Is there a trend on this respect, and if so how does it vary over time? Can you identify salient actors? Do e.g. actors tend to work in film companies with a specific ownership (white vs. african-american)?
* Crypto art transactions: can you think about how to distinguish between users that are primarily collectors and artists? Who are the dominant collectors and artists? How is the market developing over time in number of transactions and their value? Can you predict an artist's future success?
* BL books dataset: characterise the four genres using the provided dataset. Where and when are them published? Which words tend to be most associated with a given genre? Can a logistic regression classifier based just on metadata perform eauqlly well to one based on the full texts?
