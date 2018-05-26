# weather_api


一、中央气象台API接口：

1. XML接口
http://flash.weather.com.cn/wmaps/xml/china.xml
这个是全国天气的根节点，列出所有的省，其中的pyName字段是各个省XML的文件名，比如北京的是beijing，那就意味着北京的XML地址为
http://flash.weather.com.cn/wmaps/xml/beijing.xml
一个省的天气，其中列出该省各个市的数据，北京就列出各个区。
tmp1是最低温低，tmp2是最高温度，state1和state2是神马转神马，每个数代表一个天气现象。
 
2. 图片接口
http://m.weather.com.cn/img/c0.gif
http://m.weather.com.cn/img/b0.gif
http://www.weather.com.cn/m/i/weatherpic/29x20/d0.gif
http://www.weather.com.cn/m2/i/icon_weather/29x20/n00.gif
这个图就是天气现象0（晴）的图片，其他天气现象的图片依此类推。c打头的图片是20*20像素的，b打头的是50*46像素的，d打头的是反白的图标，29*20像素，n打头的是夜间反白图标，29*20像素，注意这里的文件名是两位数字！

3. JSON接口
http://m.weather.com.cn/data/101010100.html

http://www.weather.com.cn/data/sk/101010100.html

http://www.weather.com.cn/data/cityinfo/101010100.html

各个城市的代码，自己百度一下。例如：北京的代码就是101010100



二、中华万年历API接口：

1、JSON

http://wthrcdn.etouch.cn/weather_mini?city=北京

http://wthrcdn.etouch.cn/weather_mini?citykey=101010100

2、XML

http://wthrcdn.etouch.cn/WeatherApi?city=北京

http://wthrcdn.etouch.cn/WeatherApi?citykey=101010100



三、新浪天气API接口：

http://php.weather.sina.com.cn/xml.php?city=%B9%E3%D6%DD&password=DJOYnieT8234jlsK&day=1

city=城市的URL编码（广州：%B9%E3%D6%DD）。

password固定。

day=0，表示当天天气，1表示第二天天气，以此类推，最大取值为4。

新浪天气图片：

78*78：

白天：http://php.weather.sina.com.cn/images/yb3/78_78/duoyun_0.png

夜间：http://php.weather.sina.com.cn/images/yb3/78_78/duoyun_1.png

180*180：

白天：http://php.weather.sina.com.cn/images/yb3/180_180/duoyun_0.png

夜间：http://php.weather.sina.com.cn/images/yb3/180_180/duoyun_1.png
