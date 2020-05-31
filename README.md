# Fuck_heima(某培训机构)

也是服了，对于这家机构，前几天想把数据库MySQL学一下，然后就去这家培训机构官网看有没有好的课程，刚一进去就他们那个**聊天窗口**就弹了出来,问我有什么需要，我说**MySQL**, 然后就给我整**嗯嗯。零基础也是可以的哦，给您发送下 [Mysql]相关的课程资料，学习教程，黑马的内部视频，您先了解下，您看行吗？**, 还信誓旦旦的给我说，这是**是免费的偶**我就信以为真的把电话号码发过去。

效率是真的快，电话立马就打过来了，问我什么学习进度和基础（真贴心），然后我就说你们课程在哪里领啊？

**我们没有免费课程偶，都是要付费的偶**

在一阵子的**唇枪舌战之后**

既然他们是干程序这行业的，那我就...

看代码
``` python

# selenium 自动化教训这个培训机构
from selenium import webdriver
import time
from scrapy import Selector

browser = webdriver.Chrome()

browser.get('http://www.itheima.com/')

html = browser.page_source

selector = Selector(text=html)
time.sleep(3)

contact_button = browser.find_element_by_xpath('/html/body/div[1]/div[4]/ul/li[1]/a')

contact_button.click()

time.sleep(3)

browser.switch_to.frame('chatIframe')

input_element = browser.find_element_by_xpath('//*[@id="chatbox_input"]')

time.sleep(3)
while True:
    input_element.send_keys('骗子机构！')

    input_element.send_keys('\n')

    time.sleep(2)

```
