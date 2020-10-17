# Selenium
## Тест "Ждем нужный текст на странице"


## Фрагмент кода
### Находим цену дома и ждем, пока она не станет 10 000 RUR, бронируем
```python
button = browser.find_element_by_id("book")
price = WebDriverWait(browser, 15).until(
	EC.text_to_be_present_in_element((By.ID, "price"), "10000 RUR")
)
button.click()
```
