# ARCHTYPE OF NATIONAL BASKETBALL ASSOCIATION (NBA) PLAYERS

![wp4923812](https://user-images.githubusercontent.com/78009164/107141720-c5194580-6950-11eb-95fe-05c570cdea66.jpg)

## Motivation
For years players have been recognised by their defensive position on court and also informally known by names such as Rim Runner, Spot Up Bigs, and by their ball movements. This is the results provided on Wikipedia if we search for type of playersin basketball:

-  1–Pointguard 
-  2–Shooting guard   ![350px-Basketball_Positions](https://user-images.githubusercontent.com/78009164/107142230-58537a80-6953-11eb-91a4-b7cdb44f9694.png)        
-  3– Small forward
-  4–Power forward5–Center

But these are defensive position not player type, and similar results can be seen on official NBA website.

Thus there is a urgent need to analyse players on the basis of their performance/game on court rather than position, in order to understand players and team better. And take decisive actions in direction of improvement.

## Scraped Data
We will be scraping data from __[Basketball Reference](https://www.basketball-reference.com/)__  website and will be referring NBA official website for further help.\
In order to scrape data from the above stated website, we used library **urlopen** & **BeautifulSoup** to access the data available on website.
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Player</th>
      <th>Pos</th>
      <th>Age</th>
      <th>Tm</th>
      <th>G</th>
      <th>GS</th>
      <th>MP</th>
      <th>FG</th>
      <th>FGA</th>
      <th>FG%</th>
      <th>3P</th>
      <th>3PA</th>
      <th>3P%</th>
      <th>2P</th>
      <th>2PA</th>
      <th>2P%</th>
      <th>eFG%</th>
      <th>FT</th>
      <th>FTA</th>
      <th>FT%</th>
      <th>ORB</th>
      <th>DRB</th>
      <th>TRB</th>
      <th>AST</th>
      <th>STL</th>
      <th>BLK</th>
      <th>TOV</th>
      <th>PF</th>
      <th>PTS</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Álex Abrines</td>
      <td>SG</td>
      <td>25</td>
      <td>OKC</td>
      <td>31</td>
      <td>2</td>
      <td>19.0</td>
      <td>1.8</td>
      <td>5.1</td>
      <td>.357</td>
      <td>1.3</td>
      <td>4.1</td>
      <td>.323</td>
      <td>0.5</td>
      <td>1.0</td>
      <td>.500</td>
      <td>.487</td>
      <td>0.4</td>
      <td>0.4</td>
      <td>.923</td>
      <td>0.2</td>
      <td>1.4</td>
      <td>1.5</td>
      <td>0.6</td>
      <td>0.5</td>
      <td>0.2</td>
      <td>0.5</td>
      <td>1.7</td>
      <td>5.3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Quincy Acy</td>
      <td>PF</td>
      <td>28</td>
      <td>PHO</td>
      <td>10</td>
      <td>0</td>
      <td>12.3</td>
      <td>0.4</td>
      <td>1.8</td>
      <td>.222</td>
      <td>0.2</td>
      <td>1.5</td>
      <td>.133</td>
      <td>0.2</td>
      <td>0.3</td>
      <td>.667</td>
      <td>.278</td>
      <td>0.7</td>
      <td>1.0</td>
      <td>.700</td>
      <td>0.3</td>
      <td>2.2</td>
      <td>2.5</td>
      <td>0.8</td>
      <td>0.1</td>
      <td>0.4</td>
      <td>0.4</td>
      <td>2.4</td>
      <td>1.7</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Jaylen Adams</td>
      <td>PG</td>
      <td>22</td>
      <td>ATL</td>
      <td>34</td>
      <td>1</td>
      <td>12.6</td>
      <td>1.1</td>
      <td>3.2</td>
      <td>.345</td>
      <td>0.7</td>
      <td>2.2</td>
      <td>.338</td>
      <td>0.4</td>
      <td>1.1</td>
      <td>.361</td>
      <td>.459</td>
      <td>0.2</td>
      <td>0.3</td>
      <td>.778</td>
      <td>0.3</td>
      <td>1.4</td>
      <td>1.8</td>
      <td>1.9</td>
      <td>0.4</td>
      <td>0.1</td>
      <td>0.8</td>
      <td>1.3</td>
      <td>3.2</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Steven Adams</td>
      <td>C</td>
      <td>25</td>
      <td>OKC</td>
      <td>80</td>
      <td>80</td>
      <td>33.4</td>
      <td>6.0</td>
      <td>10.1</td>
      <td>.595</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>.000</td>
      <td>6.0</td>
      <td>10.1</td>
      <td>.596</td>
      <td>.595</td>
      <td>1.8</td>
      <td>3.7</td>
      <td>.500</td>
      <td>4.9</td>
      <td>4.6</td>
      <td>9.5</td>
      <td>1.6</td>
      <td>1.5</td>
      <td>1.0</td>
      <td>1.7</td>
      <td>2.6</td>
      <td>13.9</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Bam Adebayo</td>
      <td>C</td>
      <td>21</td>
      <td>MIA</td>
      <td>82</td>
      <td>28</td>
      <td>23.3</td>
      <td>3.4</td>
      <td>5.9</td>
      <td>.576</td>
      <td>0.0</td>
      <td>0.2</td>
      <td>.200</td>
      <td>3.4</td>
      <td>5.7</td>
      <td>.588</td>
      <td>.579</td>
      <td>2.0</td>
      <td>2.8</td>
      <td>.735</td>
      <td>2.0</td>
      <td>5.3</td>
      <td>7.3</td>
      <td>2.2</td>
      <td>0.9</td>
      <td>0.8</td>
      <td>1.5</td>
      <td>2.5</td>
      <td>8.9</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Deng Adel</td>
      <td>SF</td>
      <td>21</td>
      <td>CLE</td>
      <td>19</td>
      <td>3</td>
      <td>10.2</td>
      <td>0.6</td>
      <td>1.9</td>
      <td>.306</td>
      <td>0.3</td>
      <td>1.2</td>
      <td>.261</td>
      <td>0.3</td>
      <td>0.7</td>
      <td>.385</td>
      <td>.389</td>
      <td>0.2</td>
      <td>0.2</td>
      <td>1.000</td>
      <td>0.2</td>
      <td>0.8</td>
      <td>1.0</td>
      <td>0.3</td>
      <td>0.1</td>
      <td>0.2</td>
      <td>0.3</td>
      <td>0.7</td>
      <td>1.7</td>
    </tr>
    <tr>
      <th>6</th>
      <td>DeVaughn Akoon-Purcell</td>
      <td>SG</td>
      <td>25</td>
      <td>DEN</td>
      <td>7</td>
      <td>0</td>
      <td>3.1</td>
      <td>0.4</td>
      <td>1.4</td>
      <td>.300</td>
      <td>0.0</td>
      <td>0.6</td>
      <td>.000</td>
      <td>0.4</td>
      <td>0.9</td>
      <td>.500</td>
      <td>.300</td>
      <td>0.1</td>
      <td>0.3</td>
      <td>.500</td>
      <td>0.1</td>
      <td>0.4</td>
      <td>0.6</td>
      <td>0.9</td>
      <td>0.3</td>
      <td>0.0</td>
      <td>0.3</td>
      <td>0.6</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>7</th>
      <td>LaMarcus Aldridge</td>
      <td>C</td>
      <td>33</td>
      <td>SAS</td>
      <td>81</td>
      <td>81</td>
      <td>33.2</td>
      <td>8.4</td>
      <td>16.3</td>
      <td>.519</td>
      <td>0.1</td>
      <td>0.5</td>
      <td>.238</td>
      <td>8.3</td>
      <td>15.8</td>
      <td>.528</td>
      <td>.522</td>
      <td>4.3</td>
      <td>5.1</td>
      <td>.847</td>
      <td>3.1</td>
      <td>6.1</td>
      <td>9.2</td>
      <td>2.4</td>
      <td>0.5</td>
      <td>1.3</td>
      <td>1.8</td>
      <td>2.2</td>
      <td>21.3</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Rawle Alkins</td>
      <td>SG</td>
      <td>21</td>
      <td>CHI</td>
      <td>10</td>
      <td>1</td>
      <td>12.0</td>
      <td>1.3</td>
      <td>3.9</td>
      <td>.333</td>
      <td>0.3</td>
      <td>1.2</td>
      <td>.250</td>
      <td>1.0</td>
      <td>2.7</td>
      <td>.370</td>
      <td>.372</td>
      <td>0.8</td>
      <td>1.2</td>
      <td>.667</td>
      <td>1.1</td>
      <td>1.5</td>
      <td>2.6</td>
      <td>1.3</td>
      <td>0.1</td>
      <td>0.0</td>
      <td>0.8</td>
      <td>0.7</td>
      <td>3.7</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Grayson Allen</td>
      <td>SG</td>
      <td>23</td>
      <td>UTA</td>
      <td>38</td>
      <td>2</td>
      <td>10.9</td>
      <td>1.8</td>
      <td>4.7</td>
      <td>.376</td>
      <td>0.8</td>
      <td>2.6</td>
      <td>.323</td>
      <td>0.9</td>
      <td>2.1</td>
      <td>.443</td>
      <td>.466</td>
      <td>1.2</td>
      <td>1.6</td>
      <td>.750</td>
      <td>0.1</td>
      <td>0.5</td>
      <td>0.6</td>
      <td>0.7</td>
      <td>0.2</td>
      <td>0.2</td>
      <td>0.9</td>
      <td>1.2</td>
      <td>5.6</td>
    </tr>
  </tbody>
</table>

## Data Pre-processing, Feature Enginnering and EDA
Detailed analysis can be found in Jupyter notebook attached above as **Archtype of NBA Players**, here are some finding from this section.\
This is corrolarogram representing correlation between all the feature in the data.
![corrolarogram](https://user-images.githubusercontent.com/78009164/107150789-a84b3500-6985-11eb-9429-687f82152cee.png)
I tried to model linear relationship between all the scoring variables in the processed data.
![scatter plot](https://user-images.githubusercontent.com/78009164/107150960-43440f00-6986-11eb-9e7a-1009175abccb.png)
## Clustering Players on the basis of their Similarities and Dissimlarities.
Clustering can be largly classified into following 4 types, where every type uses unique technique to measure differences between the data points.  :
  -  Exclusive Clustering
  -  Overlapping Clustering
  -  Hierarchical Clustering
  -  Probabilistic Clustering
We will using all above stated methods excluding Overlapping Clustering.
### -  K-Means Clustering
Using Elbow plot & Silhouette Coefficient we decide the number of clusters
> ### Elbow Plot
 ![elbow plot](https://user-images.githubusercontent.com/78009164/107149728-49cf8800-6980-11eb-91c2-d1b7c8f85ea8.png)
> #### Silhouette Plot & Coefficient for different values of clusters
![Silhouette](https://user-images.githubusercontent.com/78009164/107149834-f3167e00-6980-11eb-90d1-3717d1ba6fb6.png)

### -  Hierarchical Agglomerative Clustering
This is a "bottom-up" approach: each observation starts in its own cluster, and pairs of clusters are merged as one moves up the hierarchy.
### -  Gaussian Mixture Models

### Comparision between these Method
we will be moving forward in our analysis with the clustering technique which has highest value of Silhouette Coefficient value.
![Comparison](https://user-images.githubusercontent.com/78009164/107142471-293e0880-6955-11eb-922d-649e52239de0.png)

## Results:
### Parallel Plot of all players in NBA season 2018-19
Parallel plot gives very good visualisation about the similarities and disimilarities between different clusters. Here every line describes a player and every colour describes a cluster. This is interactie plot, so you can slide over the respective feature axis, fix their limits and analyse the cluster you wish.
![newplot (1)](https://user-images.githubusercontent.com/78009164/107142901-ee899f80-6957-11eb-8c66-da7665dba10b.png)

## Analysis of Results
![boxplot](https://user-images.githubusercontent.com/78009164/107151755-53f68400-698a-11eb-8beb-5bc8d7c544ed.png)

# Conclusion

### - From above boxplot we conclude very valuable information that can be used by NBA team coachs to retrospect over their team and strengthen it further by removing and drafting new player of particular type.
### - If we consider mean as optimum value for our conclusion, then from above boxplot we can conclude that in order to make a strong team we should have the following proportion of every type of players:
> TYPE 1 : 25%\
>  TYPE 2 : 46%-49%\
>  TYPE 3 : 15%\
>  TYPE 4 : LESS than 10%

### - Every team consist of roughly 16 to 18 players, where only 5 of these players are in court while playing. Given the concluded proportion of type of players, it is very important that a team should have/draft the elite players of everytype in order to form a strong team. Also there are many other factors that can decide the fate of a team in a season.For example: the way coachs are making decisions on court in accordace to the situation, defence of our team, understanding between the players and many more.\
### - What I concluded is just one aspect of improvement, it will not always guarantee success to a team.
