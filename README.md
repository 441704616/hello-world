# hello-world

#coding=utf-8
from selenium import webdriver
import time
import import_sj

# #打开guojj
driver = webdriver.Chrome()
driver.maximize_window()
driver.get("http://www.guojj.com/shenzhen")
time.sleep(1)

#import_sj.Logon()
driver.find_element_by_xpath('//*[@id="page"]/div[4]/div[1]/div/div[1]/ul[2]/li[1]/form/input[1]').send_keys('test_bill')       #姓名可配
driver.find_element_by_xpath('//*[@id="page"]/div[4]/div[1]/div/div[1]/ul[2]/li[1]/form/input[2]').send_keys(import_sj.sj)
time.sleep(1)
driver.find_element_by_xpath('//*[@id="yuyue_index"]').click()
time.sleep(1)
driver.quit()

import css
import reception
import finance
import ds_sjs
import finance_qianyue


