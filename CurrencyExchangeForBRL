import requests
import time
import datetime


def get_currency_rate(currency_code):
    link = f"https://economia.awesomeapi.com.br/last/{currency_code}-BRL"
    response = requests.get(link)
    data = response.json()
    return data[f"{currency_code}BRL"]['bid']


def print_currency_rate(currency_code, country_name):
    rate = get_currency_rate(currency_code)
    print(f"{rate} BRL = 1 {currency_code} - {country_name}")


while True:
    print("=== Exchange Rates in BRL ===")
    print(f'=== Today {datetime.datetime.now()} ===')
    print(' ')
    print_currency_rate('USD', 'United States')
    print_currency_rate('EUR', 'Eurozone')
    print_currency_rate('GBP', 'United Kingdom')
    print_currency_rate('JPY', 'Japan')
    print_currency_rate('CAD', 'Canada')
    print_currency_rate('CHF', 'Switzerland')
    print_currency_rate('AUD', 'Australia')
    print_currency_rate('NZD', 'New Zealand')
    print_currency_rate('SEK', 'Sweden')
    print_currency_rate('NOK', 'Norway')
    print_currency_rate('DKK', 'Denmark')
    print_currency_rate('RUB', 'Russia')
    print_currency_rate('ARS', 'Argentina')
    print_currency_rate('CLP', 'Chile')
    print_currency_rate('MXN', 'Mexico')
    print_currency_rate('CNY', 'China')
    print_currency_rate('INR', 'India')
    print_currency_rate('TRY', 'Turkey')
    print_currency_rate('ZAR', 'South Africa')
    print("_"*50)
    time.sleep(60)

