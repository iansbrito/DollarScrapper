def get_dollar_today():
    from lxml import html
    import requests

    url = 'https://www.remessaonline.com.br/cotacao/cotacao-dolar'
    html_content = requests.get(url).content
    tree = html.fromstring(html_content)
    dolar = tree.xpath('/html/body/div/div[2]/div/div[1]/div/div[1]')[0].text_content()
    return dolar[:4]
