# Stock Ticker API

<br>

Fetch stock tickers from the SP500 index using the endpoints below.

## API Endpoints

<table style="background-color: #fafafa;">
  <tr>
    <th>Endpoint</th>
    <th>Data</th>
  </tr>
  <tr>
  
  </tr>
    <tr>
   <td><a href="https://ticker-api.herokuapp.com/docs">https://ticker-api.herokuapp.com/docs<a/></td>
    <td>Get FastAPI Docs</td>
  </tr>
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/sp500">https://ticker-api.herokuapp.com/sp500<a/></td>
    <td>Get All SP 500 Tickers</td>  
  </tr>
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/sectors">https://ticker-api.herokuapp.com/sectors<a/></td>
    <td>Get All sector names in SP500</td> 
  </tr>
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/technology">https://ticker-api.herokuapp.com/technology<a/></td>
    <td>Get All stock tickers in technology sector</td>
  </tr>
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/utlities">https://ticker-api.herokuapp.com/utilities<a/></td>
    <td>Get All stock tickers in Utilities sector</td>
  </tr>  
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/real-estate">https://ticker-api.herokuapp.com/real-estate<a/></td>
    <td>Get All stock tickers in Real Estate sector</td>
  </tr>  
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/industrials">https://ticker-api.herokuapp.com/industrials<a/></td>
    <td>Get All stock tickers in Industrials sector</td>
  </tr>  
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/healthcare">https://ticker-api.herokuapp.com/healthcare<a/></td>
    <td>Get All stock tickers in Healthcare sector</td>
  </tr>  
  <tr>
    <td><a href="https://ticker-api.herokuapp.com/financials">https://ticker-api.herokuapp.com/financials<a/></td>
    <td>Get All stock tickers in Financials sector</td>
  </tr>
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/energy">https://ticker-api.herokuapp.com/energy<a/></td>
    <td>Get All stock tickers in Energy sector</td>
  </tr> 
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/consumer-defensive">https://ticker-api.herokuapp.com/consumer-defensive<a/></td>
    <td>Get All stock tickers in Consumer Defensive sector</td>
  </tr>
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/consumer-cyclical">https://ticker-api.herokuapp.com/consumer-cyclical<a/></td>
    <td>Get All stock tickers in Consumer Cyclical sector</td>
  </tr> 
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/communication-services">https://ticker-api.herokuapp.com/communication-services<a/></td>
    <td>Get All stock tickers in Communication Services</td>
  </tr> 
   <tr>
    <td><a href="https://ticker-api.herokuapp.com/basic-materials">https://ticker-api.herokuapp.com/basic-materials<a/></td>
    <td>Get All stock tickers in Basic Materials sector</td>
  </tr>      
</table>

<br>

## Usecase

Fetch data using python

```Python


import requests
import json

url = "https://stock-tickers-api.herokuapp.com/get-tickers/sp500"
data = requests.get(url)


def jprint(data):
    # create a formatted string of the Python JSON object
    text = json.dumps(data, sort_keys=True, indent=4)
    format_obj = text.replace(',', '')
    print(format_obj.replace('"', ''))


jprint(data.json())


```
