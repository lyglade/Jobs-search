## 前程无忧网招聘信息爬虫
### 目标网站 http://www.51job.com/
- 项目结构
    - jobspider.py
    </br>主爬虫程序，负责爬取信息并导入其他文件保存信息
    - savedata.py
    </br>信息保存文件，主要负责信息的保存方法
    - citynum.py
    </br>本项目中主要负责生成城市代号，因为51job的URL中城市是用自己网站划分的城市代号表示的
- Python库支持
</br>`requests`
 `Beautifulsoup`
`re`
`urllib.parse`
`pymysql`
- spider思路
</br>获取第一个链接信息>>提取信息>>保存信息到数据库>>获取下一页链接>>递归翻页
- 技巧与难点
</br>城市代码是在一个JS文件中复制过来的，
自己输入的城市需要跟这个字典匹配生成城市代码
- 数据样本见Excel表格
- 值得改进
    - 信息提取过少，只有页面的几个基本信息，更多的信息需要打开招聘页面进一步爬虫
    - 后续进一步的信息提取
    - 将爬取的信息进行数据分析，比如招聘信息中的技能要求进行词频分析，这个后续跟进

  
