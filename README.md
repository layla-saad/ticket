```
def _retrieve_event_data(self, event):
    """
    retrieve data from datasport for a specific event
    """
    operator_list = self._get_operator_list(event['identifier'])
    category_list = self._get_category_list()

    # 1 # self.makeHTMLFile(self.browser.get_current_page().text)

```
[Creteil](files/uscreteil/1_uscreteil_1681395225.html)<br>
[Biarritz](files/bo/1_bo_1681395251.html)
```

    response = self.browser.session.post(...)
    
    # 2 # self.makeHTMLFile(response.text)

```
[Creteil](files/uscreteil/3_uscreteil_1681395726.html)<br>
[Biarritz](files/bo/3_bo_1681395736.html)
```

    response = self.browser.session.get(...)

    # 3 # self.makeHTMLFile(response.text)
    
```
[Creteil](files/uscreteil/4_uscreteil_1681395858.html)<br>
[Biarritz](files/bo/4_bo_1681395865.html)
```

    try:
        valmod = re.findall(r"selected\" value=\"(\d+)\"", response.text)[0]
    except Exception as exc:
        raise InvalidPageFormat(self._get_root_url() + '/App/Etats/Manifestations/PlacesManif_FiltreFichier.aspx') from exc

    response = self.browser.session.post(...)

    # 4 # self.makeHTMLFile(response.text)

```
[Creteil](files/uscreteil/5_uscreteil_1681396226.html)<br>
[Biarritz](files/bo/5_bo_1681396236.html)
```

    response = self.browser.session.get(...)

    # 5 # self.makeHTMLFile(response.text)

```
[Creteil](files/uscreteil/6_uscreteil_1681396335.html)<br>
[Biarritz](files/bo/6_bo_1681396347.html)
```

    return response.text
    ```