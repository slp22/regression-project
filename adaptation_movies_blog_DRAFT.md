# Exporting American Movie Box Office Hits 


## Abstract

[100 words]

## Design

The (fictitious) international movie distributor, Movies Worldwide, Inc., has requested a model to inform their choice of which American box office hits to export. 
The [original source for adaptation](https://stephenfollows.com/highest-grossing-movie-adaptations/) can influence its success. 

They have seen the press from the last few years, which reports that [book adaptations earn more worldwide at the box office](https://www.forbes.com/sites/adamrowe1/2018/07/11/why-book-based-films-earn-53-more-at-the-worldwide-box-office/?sh=290c1dfc306f). And a small [2020 survey](https://www.bhg.com/news/book-vs-movie-debate/) of Americans which found that respondents almost equally enjoyed the book as much as a movie adaptation. 

Certain artistic qualities make [book to movie](https://news.northeastern.edu/2012/03/27/kelly/) adaptations successful, but they can be subjective and are harder to model. 

There are [super earning book-to-film adaptations](https://filmthreat.com/features/what-makes-a-book-to-film-adaptation-so-successful/) which followed super earning book launches, such as the *Harry Potter* series and *Lord of the Rings*. 

Our client's niche market is to export movies with more affordable movie distribution rights. Our task is to build a model using available data for high gross earning movies abroad and use that model to predict lesser-known movie adaptations to recommend to export.  

## Data

Scraped data for movie adaptations from boxofficemojo.com. Adaptations include:
* books<sup>1</sup>
* television shows<sup>2</sup>
* events, 
* video games, and 
* plays. 

Created a linear regression model (ordinary least squares) with one feature,`domestic_total_gross`, to predict the `international_total_gross`. The model has an adjusted R<sup>2</sup> of 0.763. 

The linear regression model plot shows that the model does not capture the data well enough to make accurate predictions. The data points are clustered close to the origin of the graph. 

Movies with high revenues highly impact the predictive power of the model. The residual plot indicates heteroskedasticity which is likely due to the wide range of domestic movie revenue (\\$742 - \\$543,638,043).
<br></br>
<br></br>
<sup>1</sup> Books include young adult novels, contemporary novels, children's books, and commic books. 

<sup>2</sup> Television shows include children shows and cartoons.  


## Tools

* Requests, BeautifulSoup, pickle
* Pandas, Statsmodels, Scikit-learn <br/>


## Communication

Slides and code are available on https://github.com/slp22/regression-project.




