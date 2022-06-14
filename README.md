{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Microsoft Movie Studio\n",
    "***"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "![microsoft logo](images/microsoftlogo.png)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Overview\n",
    "Flatiron School Data Science Phase 1 project.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Business Problem\n",
    "Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Data Used\n",
    "\n",
    "data from the following sources can be found in the 'zippedData' folder\n",
    "\n",
    "* [IMDB](https://www.imdb.com/) - im.db.zip\n",
    "* [Box Office Mojo](https://www.boxofficemojo.com/) - bom.movie_gross.csv.gz\n",
    "* [The Numbers](https://www.the-numbers.com/) - tn.movie_budgets.csv.gz"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "![Movie Data ERD](images/movie_data_erd.jpeg)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Deliverables\n",
    "\n",
    "\n",
    "\n",
    "* [Non-Technical Presentation]()\n",
    "* [GitHub Repository](https://github.com/ceflynn/dsc-phase-1-project-v2-4)\n",
    "* [Jupyter Notebook](https://github.com/ceflynn/dsc-phase-1-project-v2-4/blob/master/student.ipynb) "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Action Steps\n",
    "* **Recommendation 1** - Compete with Big Studios\n",
    "    * Create dataframe from BoxOfficeMovie.com\n",
    "    * Data Cleaning  \n",
    "    \n",
    "        * Missing values and NaN \n",
    "        * Commas in 'foreign_gross' - Get Values from website\n",
    "        * Change columns in int64 for calculations\n",
    "    * Find and graph total gross \n",
    "    * Create dataframe from the-numbers.com\n",
    "    * Data cleaning\n",
    "        * Get rid of '$' and ',' from 'production_budget' and 'worldwide_gross\n",
    "        * Change those columns to int64\n",
    "        * Create column and calculate profit\n",
    "        * Drop unecessary columns\n",
    "        * Change 'release_date' to 'year' and only have the 4 digit year\n",
    "    * Merge data with studio data\n",
    "    * Get full studio names\n",
    "    * Create data visualization for movie studio Profit\n",
    "* **Recommendation 2** - Create Multi-Genre Movies \n",
    "    * unzip db\n",
    "    * Create dataframe\n",
    "        * Join tables (movie_basics and movie_ratings)\n",
    "        * Get popular and highly rated movies\n",
    "    * Data cleaning\n",
    "    * Create boolean multi-genre column\n",
    "    * Data visualization using value_counts()\n",
    "    \n",
    "* **Recommendation 3** - Focus on Biographies\n",
    "    * Get list of Genres from the dataframe in Rec 2\n",
    "    * Create boolean column for each Drama\n",
    "    * Count values for genre columns\n",
    "    * Create data visualization for genre_counts\n",
    "    * Find average rating for each genre for all Movies\n",
    "    * Data cleaning\n",
    "    * Use most common genres\n",
    "    * Get the mean for each genre\n",
    "    * Create data visualization for genre ratings"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Repository"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "* images/\n",
    "    * awesome.gif\n",
    "    * microsoftlogo.png\n",
    "    * movie_data_erd.jpeg\n",
    "* pdf/\n",
    "    * microsoft-pres.pdf\n",
    "* zippedData/\n",
    "    * bom.movie_gross.csv.gz\n",
    "    * im.db.zip\n",
    "    * rt.movie_info.tsv.gz\n",
    "    * rt.reviews.tsv.gz\n",
    "    * tmdb.movies.csv.gz\n",
    "    * tn.movie_budgets.csv.gz\n",
    "* student.ipynb \n",
    "* CONTRIBUTING.md\n",
    "* Instructions.md\n",
    "* LICENSE.md\n",
    "* README.md"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python (learn-env)",
   "language": "python",
   "name": "learn-env"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.5"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}
