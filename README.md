# API_Homework
## This homework assignment focused on the following:
* Ingesting API data into a Python notebook
* Using the JSON library to access specific data elements from the API data
* Determining asset values and comparing those values to a target amount
* Using the Monte Carlo simulations library to perform simulations to provide possible ranges for investment outcomes
    * One key item that was identified during the pulling of data for the simulations is that Alpaca the provider we use for closing prices only allows us to pull 1,000 days worth of closing prices. This is in contrast to the instructions which ask for 5 years of worth of data, which would be 1,260 days of closing prices.
        * This is significant because the smaller the data window we use for our inputs into the Monte Carlo simulation the more our output is subject to the idiosyncrasies of our time period. I bring this up because the 4 year window that was used as input into our Monte Carlo simulation included a one year return on SPY over 50%. In actuality we should probably target 10 years worth of data for input into out Monte Carlo simulations.