from selenium import webdriver
from selenium.webdriver.edge.service import Service
import time

service = Service("C:\\Users\\Pranathi\\Downloads\\edgedriver_win64\\msedgedriver.exe")

driver = webdriver.Edge(service=service)
driver.get("https://www.google.com")
time.sleep(20)

driver.quit()



from selenium import webdriver
from selenium.webdriver.edge.service import Service
import time

service = Service("C:\\Users\\Pranathi\\Downloads\\edgedriver_win64\\msedgedriver.exe")

driver = webdriver.Edge(service=service)
driver.get("https://www.facebook.com")
time.sleep(20)

driver.quit()



from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time

driver = webdriver.Edge()
driver.get("https://www.google.com")
driver.maximize_window()

search_box = driver.find_element(By.NAME, "q")
search_box.send_keys("Selenium Web Testing")
search_box.send_keys(Keys.RETURN)

time.sleep(3)

search_button = driver.find_element(By.NAME, "btnK")
print("Google Search button found.")


driver.quit()
