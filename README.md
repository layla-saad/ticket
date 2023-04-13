```
def _retrieve_event_data(self, event):
    """
    retrieve data from datasport for a specific event
    """
    operator_list = self._get_operator_list(event['identifier'])
    category_list = self._get_category_list()

    # 1 # self.makeHTMLFile(self.browser.get_current_page().text)

    response = self.browser.session.post(...)

    ```
    [# 2 #](2_uscreteil_1681395450.html)  
    
    ```
    # 3 # self.makeHTMLFile(response.text)

    response = self.browser.session.get(...)

    # 4 # self.makeHTMLFile(response.text)

    try:
        (...)
    except Exception as exc:
        (...)

    response = self.browser.session.post(...)

    # 5 # self.makeHTMLFile(response.text)

    response = self.browser.session.get(...)

    # 6 # self.makeHTMLFile(response.text)

    return response.text
    ```
