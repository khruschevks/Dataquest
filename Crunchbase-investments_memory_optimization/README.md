# Project: Pandas dataframe data consumption omptimization (from Dataquest data engineer course)
## Introduction
In this project, assumme, there is limitation by memory which can be used to conduct analysis on Dataset. Lets say, only 20 MB of RAM, that can be used to store dataframe.

Crunchbase-investments dataset is given. The goal is to choose the correct datatype for each column to reduce overall memory consumption. It is not essential, what actual data is in the dataset. Only its data types matters.

So, this is stated:  
* **Problem**: 20 MB memory limitation  
* **Goal**: Reduce dataframe memory consuption as much as possible  
* **Approach**:
    * Clean corrupted values
    * Format columns
    * Determine appropriate data types to convert. Data types used: *Category, float, int, datetime, bool*.
    * Process in chunks to fit in memory limitation 

**Distinctions from ["Loans_memory_optimization"](https://github.com/khruschevks/Pandas-memory-optimization/tree/main/Loans_memory_optimization)**:  
* Checking for duplicates
* More attention to NaN values
* Parsing date month and quarter
* Determing source csv encoding
