github網址：meow8525.github.io
進去預設打開的是index.html

我有在家裡桌電的vscode裝live server的擴充
在html的code裡右鍵open with live server可以有一個實時隨檔案更動的預覽網頁，按ctrl S就會刷新

網頁有四個html：
index(home)
research
Teaching
Lab

CSS的內容很亂，全部丟在style.css裡面了。
css的code很零散，如果需要改變網頁上對應的排版請用html裡區域對應的class在style.css裡面ctrl F
在css裡面，同樣class的設定後面會蓋掉前面，所以務必看完全部ctrl F搜尋到的東西以後再看要改哪


index.html：

上面一排四個html都是一樣的
左邊的可以點擊 會返回index.html
右邊的四個可以前往對應的html
對應的區域是<header>

hero是實驗室名字大標題的那塊

接下來有兩個section 都是一樣的
是關於教授和關於我們的區塊
中間有個<div class="footer gap"> 他只是網頁裡面的空白區域而已 搞排版用的

最後每個頁面也都有一樣的footer，可以看要不要刪掉或是留著寫一些你需要的東西。



Research.html:

一樣會有header
也有hero。Research下面那行小字記得要改

下面有兩個feature list
按下會跳到對應的文章處
#ongoing1, #ongoing2 之類的反正就是照順序。

接下來每個research的區塊都是複製貼上的
總共有十篇
有點亂，不過html本來就很亂，畢竟文字和其他東西隨便混在一起
反正就是title、左邊img、右邊summary+list出來的文獻
有需要加的話就是直接複製 裡面東西改一改就行
如果有研究沒有references的話 要把這一行留下來：<span class="research-more"></span> 這和see more的運作有關係 不留會關不起來

再下面是Selected additional works and publications
這裡偷懶用了Teaching用到的css的class，如果要動的話兩邊會一起動、需要的話可以去style.css裡面自己創新class
然後反正就是list出來

下面還有一段handle see-more的code，反正就一個if else，沒很複雜。

最後面也有footer



Teaching.html

沒什麼特別的，Teaching下面的小字記得改
footer也記得改



Lab.html

同上



style.css

所有code裡面最亂的，尤其一直改東改西沒照順序，導致裡面可能操控兩個相鄰區塊的css相隔200行，因此請使用ctrl F
直接跟copilot說要改什麼基本都能改好。這次用下來這裡都沒出什麼問題。