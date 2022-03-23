# Exporting American Movie Box Office Hits 


## Abstract

[100 words]

## Design

Recent press has reported that [book adaptations earn more worldwide at the box office](https://www.forbes.com/sites/adamrowe1/2018/07/11/why-book-based-films-earn-53-more-at-the-worldwide-box-office/?sh=290c1dfc306f). And a small [2020 survey](https://www.bhg.com/news/book-vs-movie-debate/) of Americans found that respondents almost equally enjoyed the book as much as a movie adaptation. 

The (fictitious) international movie distributor, Movies Worldwide, Inc., wants a model to inform their choice of which American box office hits to export. 
The [original source for adaptation](https://stephenfollows.com/highest-grossing-movie-adaptations/) can influence its success. 

Certain artistic qualities make [book to movie](https://news.northeastern.edu/2012/03/27/kelly/) adaptations successful, but they can be subjective and are harder to model. 

There are [super earning book-to-film adaptations](https://filmthreat.com/features/what-makes-a-book-to-film-adaptation-so-successful/) which followed super earning book launches, such as the *Harry Potter* series and *Lord of the Rings*. 

Our client's niche market is to export movies with more affordable movie distribution rights. Our task is to build a model using available data for high gross earning movies abroad and use that model to predict lesser-known movie adaptations to recommend to export. 

**Research Question:** Can a model predict a movie adaptation's international total gross revenue based on movie data available on boxofficemojo.com?

## Data

This analysis uses data scraped from boxofficemojo.com. The sub-set of data was for movie that are adaptations of books<sup>1</sup>, television shows<sup>2</sup>, events, video games, and plays. 

The linear regression model robust domestic data. However, it did not result in a powerful model to predict international gross revenue for movie adaptations. Feature transformations include converting categorical data to dummy variables (MPAA ratings and distributors), log transformations of monetary features (international total gross and domestic total gross). Engineered features included interactions, such as profit (domestic_total_gross - budget), opening profit (domestic_opening - budget) and opening data (domestic_opening * opening_theathers). 

The analysis showed that predicting international gross revenue based on domestic data in this model is not reliable enough to make investment decisions. Boxofficemojo.com lists country-specific box office sales, which could better predict international gross revenue. 
<br></br>
<br></br>
<sup>1</sup> Books include young adult novels, contemporary novels, children's books, and commic books. 

<sup>2</sup> Television shows include children shows and cartoons.  


## Tools

* Requests, BeautifulSoup, pickle  <br/>
* Pandas, Numpy, Statsmodels, Scikit-learn <br/>


## Communication

Slides and code are available on https://github.com/slp22/regression-project.






