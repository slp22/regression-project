#### Regression | Project Proposal

# Exporting American Movie Adaptations 

## Question
* What is the question behind your analysis or model and what practical impact will your work have?<br/>
    * How can a movie distributor decide if it's financially savvy to export a movie to an international market? Build a model that can predict a movie adaptation's international gross revenue.<br/>
* Who is your client and how will that client benefits from exploring this question or building this model/system?<br/>
    * Client: Fictitious international movie distributor, Movies Worldwide, Inc. <br/>
    * Movies Worldwide, Inc. needs a reliable model to help them choose which American box office hits are worth exporting.<br/> 
    
## Data Description
* What dataset(s) do you plan to use, and how will you obtain the data?<br/>
  * BoxOfficeMojo [Genre Keyword: Adaptation](https://www.boxofficemojo.com/genre/sg3101552897/?ref_=bo_gs_table_36) (n=964)<br/>
* What is an individual sample/unit of analysis in this project? In other words, what does one row or observation of the data represent?<br/>
    * Each unit of analysis is one movie, including re-releases.<br/>
* What characteristics/features do you expect to work with?
    1. domestic lifetime gross revenue
    2. domestic opening weekend revenue
    3. production budget
    4. MPAA rating
    5. domestic distributor
    6. release date
    7. running time
    8. genres<br/>
* If modeling, what will you predict as your target?<br/>
    * The model will predict **international gross revenue**.<br/>
 
## Tools
* How do you intend to meet the tools requirement of the project?</br>
    * Requests, BeautifulSoup, pickle
    * Pandas, Statsmodels, Scikit-learn <br/>
* Are you planning in advance to need or use additional tools beyond those required?</br>
    * None at this time. <br/>
 
## MVP Goal
* What would a MVP Example look like for this project?<br/>
    * Linear regression model with two features (gross domestic revenue and opening weekend revenue)
    * Residual plot of actual vs. predicted gross international revenue
    * Using all features, plot a heatmap to understand multicollinearity
    
