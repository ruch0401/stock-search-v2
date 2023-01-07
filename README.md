# Stock Search Web Application

## Demo (Click on the thumbmail below to view on YouTube)

<a href="https://www.youtube.com/watch?v=43Dg7sZt1lc" target="_blank">
 <img src="https://raw.githubusercontent.com/ruch0401/resources/main/csci-571/stock-search-angular-thumbnail.png" alt="Watch the video for project demo"/>
</a>

### Salient Features

This stock search webpage allows users to search for stocks using the FinnHub API and display the results on the search page.

The web app also had auto-refresh feature where the stock information in the portfolio are updated every 15 seconds when the market is open.

A user can enter a stock ticker symbol and select from a list of matching stock symbols using “autocomplete.” A quote on a matched stock symbol can be performed. 

a) Home Route [‘/’] redirected to [‘/search/home’]– It is a default route of this application.
b) Search Details Route [‘/search/<ticker>’] – It shows the details of the <ticker> searched
c) Watchlist Route [‘/watchlist’] – It displays the watchlist of the user.
d) Portfolio Route [‘/portfolio’] – It displays the portfolio of the user.

## Hands On!

Try the app yourself here - https://jdofgbmx.uw.r.appspot.com/search/home

## Technologies Used

| Area     | Technologies         |
| -------- | -------------------- |
| Backend  | Node.js + Express.js |
| Frontend | Angular              |

## Server side code

### Library Details

| Libraries Used | Purpose                                         |
| -------------- | ----------------------------------------------- |
| `axios`        | For making API calls to the Finnhub API         |
| `cors`         | To handle cross-origin-resource-sharing issues  |
| `nodemon`      | For hot reloading of the node server            |
| `express`      | For making use of the Express Node.js framework |

### API endpoints

Host URL1: https://jdofgbmx.uw.r.appspot.com

| Purpose                       | Endpoint                       | Query Params                 | Example                                                                                                                   |
| ----------------------------- | ------------------------------ | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Company Description           | /company/description           | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/description?symbol=AAPL                                                |
| Company Historical Data       | /company/historical/data       | symbol, resolution, from, to | https://jdofgbmx.uw.r.appspot.com/company/historical/data?symbol=AAPL&resolution=D&from=1631022248&to=1631627048 |
| Company Latest Stock Price    | /company/latest-stock-price    | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/latest-stock-price?symbol=AAPL                                         |
| Company Autocomplete          | /company/autocomplete          | q                            | https://jdofgbmx.uw.r.appspot.com/company/autocomplete?q=AA                                                      |
| Company News                  | /company/news                  | symbol, from, to             | https://jdofgbmx.uw.r.appspot.com/company/news?symbol=MSFT&from=2022-03-09&to=2022-03-10                         |
| Company Recommendation Trends | /company/recommendation-trends | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/recommendation-trends?symbol=MSFT                                      |
| Company Social Sentiment      | /company/social-sentiment      | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/social-sentiment?symbol=MSFT                                           |
| Company Peers                 | /company/peers                 | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/peers?symbol=MSFT                                                      |
| Company Earnings              | /company/stock/earnings        | symbol                       | https://jdofgbmx.uw.r.appspot.com/company/stock/earnings?symbol=MSFT                                             |
