# Learning-about-HTML
This repository is used to house some of the examples I practiced while learning HTML.

<h2>html的基本标签</h2>
1、标题标签：h标题标签，可以把其中的文字放大加粗，有h1~h6六个，分别对应一到六级标题。<br>
2、段落标签：p是双标签，主要用于包裹一段文字，大多数会在编写网页正文时用到。  <br>
3、换行标签：br是单标签，需要换行时直接使用即可。<br>
4、水平线标签：hr，单标签，可以在网页中生成一条横线。<br>
5、字体样式标签：<br>
   字体加粗标签：b标签和strong标签都是字体加粗标签，显示效果两者没有区别，区别在于strong标签表强调语气（对PC生效）。<br>
   字体斜体标签：i标签和em标签都是字体斜体标签，显示效果两者没有区别，区别在于em标签表强调语气（对PC生效）。<br>
   字体加下划线标签：u和ins,为文字添加下划线。<br>
   字体加删除线标签：del，为字体添加一条删除线。<br>
   字体加标记标签<mark></mark>：为文字添加标记。<br>
6、图像标签：img,其中src是必要属性，填写图片文件的路径信息。<br>
7、链接标签：a，双标签，为包含在其中的内容添加超链接，其中href属性填写链接地址。<br>
8、锚点链接：也是a，但链接时需要定义id属性，可以在本页面内跳转到相应的位置。<br>
9、div标签，可以看作一个盒子，独自占浏览器的一行。<br>
10、span标签，也可以看作一个盒子，但占地没有div大。<br>
<h2>表格</h2>
1、表格的标签为table,tr(行),td(单元格)，td必须嵌套在tr内。th是表头标签，会将表头内容加粗居中。<br>
2、表格的属性标签有align(表格的对齐方式),border(表示表格是否有边框，默认值是0(无边框)，可改为1)，cellpadding是文字单元格边框的距离，cellspacing是单元格与单元格之间的距离。width,height可以改变表格的宽和高。<br>
3、一般情况下，表头要用th标签定义，th标签可以是=使内容加粗并居中。<br>
<h2>列表</h2>
1、无序列表：标签为ul双标签,ul标签内只能包含li标签，不能再有其他任何内容，但li标签内可以再添加其他标签和内容。<br>
2、有序列表：标签为ol双标签,其内也只能包含li标签，与无序列表相同，但列表的内容是有序的。<br>
3、自定义列表：标签为dl双标签，包含dt和dd两个标签，dt是列表的title标签，dd标签的内容是对dt标签的解释。<br>
<h2>表单</h2>
1、表单包括：表单域（用来收集用户信息，将用户信息提供到相应服务器），表单控件（表单元素），提示信息。<br>
2、表单域的标签是form，form中有三个属性分别为action="url地址"（信息将要发送到的位置），method="提供方法"，name="表单域名称"。<br>
3、表单的大部分功能都要用input标签实现：input type=""，type中填写想要实现的属性，常见属性有以下：<br>
 <strong>file：文件域，实现文件的上传<br>
 text 文本属性，用户可以看见输入的内容<br>
 vaule 属性只有在文本框中才会有明显的视觉效果，他的作用是将用户的选择数据提交给后台服务器<br>
 maxlength 规定文本输入的最大长度，一般较少使用<br>
 password 密码属性，用户不能看见输入的内容
 radio 单选按钮 实现多选1<br>
 name 是表单元素名字，这里radio的name必须相同 才能实现单选效果<br>
 label 标签用于绑定一个表单元素，当点击label标签内的文本时，光标会自动转到对应的表单元素上，以增加用户体验，可用于单选或复选框<br>
 checkbox 复选框 ，实现多选，name要求都相同<br>
 下拉列表标签：select，点击显示多个可选择的选项，节省页面空间，select是双标签，其中至少包含一对option标签，可以在option中使用selected="selected" 使该选项为默认选中状态<br>
 普通按钮：button，后期结合js 脚本使用<br>
 文本域标签：textarea,适用于需要输入大量文本时。cols表示每行可以显示的字数，rows表示文本域可以显示出的行数，实际开发中一般不使用<br>
 提交按钮：submit，点击此按钮后，表单域内所填写的内容就会被发送至相应的后端服务器(form中的action属性)，可以使用vaule改变按钮的内容<br>
 重置按钮:reset，可以使表单恢复至初始状态,可以使用vaule改变按钮的内容<br>
 checked 属性，用于单选框或复选框，他可以使页面在初次加载或刷新时，该按钮默认为选中状态<br> </strong>
 <h2>CSS样式</h2>
 css简称样式表，引入方式有三种，<strong>第一种</strong>是内部样式表，将css样式写在head标签中，且要用style标签包括，比较常用。<strong>第二种</strong>是外部样式表，将css样式写入一个新的css文件中，在html中使用link进行调用，在实际开发中最常用。<strong>第三种</strong>是行内样式表，在标签中直接使用style属性设计样式,一般用来修改少量样式。<br>
 <h3>选择器</h3>
 选择器就是选出要改变样式的目标，基本格式为：元素 {样式声明}
 <h4>一、基础选择器</h4>
 1、标签选择器：以html的标签作为选择器，可以选出所有目标标签，快速改变样式<br>
 2、类选择器，需要自己定义一个类名，具体格式为：.类名{样式}，类名为自己自定义的，在body部分，用class="类名"的格式来进行调用，类选择器可以按照自己的意愿选择想要改变样式的目标，在实际开发中十分常用。<br>
 3、id选择器：定义样式格式为 #id名，调用格式为 id="id名"，这种方法只可进行一次调用<br>
 4、通配符选择器：*，会把所有标签都选中并改变样式，特殊情况才会使用 <br>
 5、改变字体样式：写在选择器内，可以改变文本样式。常见的属性有以下：<br>
 <strong>
   colol：；改变文本颜色<br>
   font-size:;改变文本大小<br>
   font-family:;设定系列字体<br>
   font-weight:改变字体粗细<br>
   font-style:设置文本样式（斜体等）<br>
   简写（font：font-style font-weight font-size/line-height font-family 这些属性必须按照顺序写，不能颠倒，size和family属性必须保留，不然font：不起效果）<br>
   text-align:文本对齐方式<br>
   text-indent:首行缩进像素,一般单位是em，一个em就是当前段落一个文字的大小<br>
   line-height:设置行间距
 </strong>
 <h4>二、复合选择器</h4>
 1、后代选择器：可以选择父元素里的子元素，语法为：元素1  元素2 {样式声明} ，元素1是父级，元素2是子级，元素1和2之间要用空格隔开，最终选择的是元素2，元素1和2可以是任意基础选择器。<br>
 2、子代选择器：只能选择离父级最近的元素，语法为：元素1>元素2 {样式声明} ，最终选择的是元素2<br>
 3、并集选择器：可以选择多组标签，同时为他们定义相同的样式，语法为：元素1,元素2 {样式声明} ，同时选中元素1和2<br>
 4、链接伪类选择器：有四个，分别为 a:link(选择还未访问的链接) , a:visited(选择已经访问过的链接) , a:hover(选择鼠标经过的链接) , a:active(选择鼠标按下但还未弹起的链接)<br>
 5、focus伪类选择器：用于选中获得光标的表单元素，主要针对input类的表单元素，语法为：input:focus {样式}
 <h2>改变元素显示模式</h2>
 1、display：inline 转换为行内元素<br>
 2、display：block 转换为块元素<br>
 3、display：inline-block 转换为行内块元素<br>
<h2>背景</h2>
1、背景颜色：通过设置background-color可以改变背景颜色，默认值是transparent（透明）<br>
2、背景图片：background-image,默认值为none（没有背景图片），要填写url才能显示对应的图片。<br>
3、背景平铺：background-repeat，默认值为repeat,其他值为no-repeat(不平铺),repeat-x(横向平铺),repeat-y（纵向平铺）<br>
4、背景位置：background-poisition  x(top center bottom) y(left center right) ,x与y的属性可以互换顺序，不会影响结果。若只写一个属性，则另一个属性默认为center。 x,y的值也可以是精确单位（px），若是精确单位，则x，y的顺序不能颠倒，若只指定了一个值（默认为x），则y默认是居中。xy也可以是混合单位，第一个值一定是x坐标，第二个是y坐标。<br>
5、背景固定：background-attachment  scroll(随着文本一起滚动)||fixed(固定的)，默认值为scroll。<br>
6、背景简写：color url() repeat attachment poisition  属性无固定顺序，这是平常约定的顺序。<br>
7、背景颜色半透明：background:rgba(0,0,0,0.5),a属性的值决定了背景颜色的透明度。
<h2>CSS的三大特性</h2><br>
1、层叠性：相同选择器设置的相同样式，此时会遵循就近原则，谁离结构进谁就起作用。<br>
2、继承性：子标签会继承父标签的某些属性（text- font- line color）<br>
3、优先级：设定的样式冲突时，执行的顺序是：继承或*(0000)  元素选择器(0001)  类选择器和伪类选择器(0010)  id选择器  行内样式style(0100)  样式+!imporant(1000),括号中表示选择器的权重。继承的权重是0，如果没有单独选中该元素，不管父元素的权重多高，继承来的权重都是0。若使用复合选择器，则权重会产生叠加，不会进位，需要重新计算，如 ul li {样式} 的权重就是0002。
<h2>盒子模型</h2>
盒子模型的组成部分有content(内容),border(边框),padding(内边距),margin(外边距)
<h4>border(边框)</h4>
1、border可以设置边框的样式，且会影响盒子的实际大小，有三种属性，语法为：border：border-width(边框粗细)，单位是px || border-style(边框样式，即实线虚线等)，常用的属性有dashed(虚线)，solid(实线)，dotted(点线) || border-color<br>
2、复合写法:border:width style color 属性没有顺序<br>
3、边框分开写法：border-top/bottom/left/right 可以分别设置边框的样式<br>
4、表格细线边框：border-collapse:collapse,合并两个相邻的边框。
<h4>padding(内边距)</h4>
1、padding可以设置盒子中内容与边框的距离，同时也会影响盒子的实际大小，语法为：padding-left/right/top/bottom : 值 ，单位是px。<br>
2、padding的复合写法：padding：值 值的个数代表了不同的样式。<br>
<strong>若只有一个值：padding：5px 则代表上下左右都是5px的内边距<br>
若有两个值：padding：5px 10px 代表上下内边距是5px 左右内边距是10px<br>
若有三个值：padding：5px 10px 20px 代表上内边距是5px 左右内边距是10px 下内边距是20px<br>
若有四个值：padding：5px 10px 20px 30px 代表上内边距是5 右内边距是10 下内边距是20 左内边距是30</strong><br>
3、在实际开发中，一般使用padding设置内边距来撑开盒子，而不是为盒子设置固定的值<br>
4、清除内外边距： * {margin: 0;  padding: 0;}<br>
5、margin控制盒子与盒子之间的间距，与padding的用法基本相同<br>
<h2>圆角边框</h2>
border-radius: 值；，单位是px，值越大弧度越大。<br>
<h2>盒子阴影</h2>
语法：box-shadow: h-shadow(必须，水平阴影的位置) v-shadow(垂直阴影的位置) blur(阴影的模糊程度) spread(阴影的尺寸) color(阴影的颜色) inset(改为内部阴影，默认为Outset外部阴影，但改回外部阴影的时候不用再写outset);<br>
<h2>文字阴影</h2>
语法：text-shadow: h-shadow(必须，水平阴影的位置) v-shadow(垂直阴影的位置) blur(阴影的模糊程度) color(阴影的颜色)
<h2>浮动</h2>
网页布局第一准则：纵向排列找标准流，横向排列找浮动。<br>
1、语法：float： {属性值（none left right）},float会使块元素强制为横向排列，且中间没有空隙。<br>
<strong>
   2、浮动特性-脱标：设置了float的元素会脱离标准流(浮)，移动到指定的位置(动)，且浮动的盒子不再保留原先的位置（浮动的盒子会在标准流盒子之上）,浮动的盒子只会影响后面的标准流，不会影响后面的标准流<br>
   3、浮动特性-元素一行显示：如果多个盒子都设置了浮动，则他们会按照属性值在一行内按顶端对齐的方式显示<br>
   4、浮动元素具有行内块元素的特性，不论之前是什么模式的元素。如果块级盒子没有设置宽度，默认宽度和父级一样宽，但添加浮动后，他的大小根据内容来决定。<br>
   5、清除浮动：很多情况下，父盒子中需要放很多元素，是不方便给固定高度的，最理想的情况就是不给父盒子高度，让子盒子将父盒子撑开，但子盒子是浮动元素，已经脱标，因此不给父盒子设置高度就会使父盒子高度为0，从而影响之后的标准流，这种情况就需要清除浮动，清除浮动的本质就是清除浮动元素的特性，清除浮动后，父盒子就会根据子盒子自动检测高度变化并随之变化。<br>
   6、清除浮动的方法： clear：both  <br> 
      <1>、额外标签法：在最后一个浮动元素后增加一个新的标签（只能为块级元素），在此标签中调用clear的选择器。<br>
      <2>、为浮动元素的父元素添加overflow代码，一般是overflow:hidden, 也可以是auto，scroll<br>
      <3>、after伪元素：<pre>.clearfix:after {
			content: "";
			display: block;
			height: 0;
			visibility: hidden;
			clear: both;
		}
         /* 低版本浏览器 IE6 / IE7 清除浮动样式 */
		.clearfix {
			*zoom: 1;  
		}</pre>
      <4>、双伪元素清除浮动:<pre>		/* 清除浮动 - 使用双伪元素清除浮动 */
		.clearfix:before,
		.clearfix:after {
			content: "";
			display: table;
		}
         		.clearfix:after {
			clear: both;
		}
         		.clearfix {
			*zoom: 1;
		}
      </pre>
</strong>
<h2>定位</h2>
定位=定位模式+边偏移，定位模式就是以哪种方式固定盒子，有 static静态定位，ralative相对定位，absolute绝对定位，fixed固定定位。边偏移决定盒子最终的位置，有 top bottom left right 四个属性。<br>
1、静态定位： 语法：选择器 {position：static},这种定位没有边偏移，在实际开发中不常使用。<br>
2、相对定位：语法：选择器{position:relative},这种定位模式是以盒子自己为中心，且移动后还保留原来的位置，一般用来限制绝对定位。<br>
3、绝对定位：语法：选择器{position：absolute}，若此盒子没有祖先元素或祖先元素没有定位，则以浏览器为标准进行移动；若有祖先元素，则以最近一级的有定位的元素为标准进行移动。绝对定位脱离标准流，不占有原来的位置。<br>绝对定位居中算法：先left：50%走父盒子一半的宽度，再margin-left:负值  走定位盒子一半的宽度<br>
4、固定定位：语法：选择器{position：fixed}，固定定位以浏览器的可视区域为标准，跟父元素没有关系，固定定位的元素不会随着滚动条滚动，且不会占有原来的位置。<br>
	      固定定位小技巧：将盒子定位在版心的右侧：为盒子添加绝对定位走浏览器一半的宽度，再利用margin-left走版心盒子一半的宽度即可<br>
5、粘性定位：语法：选择器{position：sticky}，以浏览器的可视窗口为标准移动，占有原来的位置，在使用时必须至少添加一个边偏移元素才能起效果，可以看作相对定位和绝对定位的结合。<br>
6、可以通过z-index属性改变定位盒子的优先级，即叠放顺序。<br>
<h2>元素的显示与隐藏</h2>
1、display：none可以隐藏元素，display：block可以显示元素，隐藏的元素不再占有位置。<br>
2、visiblity:hidden隐藏元素，visiblity:visible显示元素，隐藏的元素仍然占有位置。<br>
3、overflow:只处理溢出的部分元素，overflow:hidden可以隐藏溢出部分的元素，overflow:auto可以在文本溢出时添加滚动条，overflow:scroll总是显示滚动条，默认是overflow:visible，不处理溢出元素。<br>
<h2>精灵图sprites</h2>
1、精灵图主要针对于小的背景图片使用，主要借助于backgroung-position来实现，一般情况下精灵图都是负值(网页中x轴向右，y轴向下),精灵图的实现可以看作是有一个小盒子在精灵图上移动，想要显示哪张图片就要移动（实际上移动的是sprites背景图）至相应的坐标位置。<br>
代码案例：<pre>
  .box {
	width: 27px;
	height: 25px;
	background: url(sprites.png) no-repeat -155px -106px;
}
</pre>
<h2>字体图标</h2>
1、字体图标iconfont,展现的是图标，实质上是文字，可以更改颜色大小等属性。<br>
2、字体图标是在网上已经制作好的图标，直接下载使用即可。https://icomoon.io<br>
3、字体图标的引入：在网页中下载好字体突变压缩文件后，将其中的fonts文件放在根目录中，复制好引入所需的代码放在style中。<br>
4、后续追加新的图标需要在网页中选择selection.json文件重新下载，然后把原来的fonts文件替换掉。<br>
<h2>用户界面</h2>
1、鼠标样式：cursor:值， 值有default(默认光标，小箭头)， pointer(小手)， move(移动，十字架)， text(文本)， not-allowed(禁止样式)
2、取消表单默认轮廓颜色：outline:0或none,可以把聚焦后表单边框的默认蓝色去除。<br>
3、文本域防拖拽：resize:none,用户不能改变文本域的大小。<br>
<h2>溢出文字省略号显示</h2>
1、单行文字：首先将文字强制单行显示(white:nowrap),然后去除文字的溢出部分(overflow:hidden),最后显示省略号(text-overflow:ellipsis)
<h2>H5提高</h2>
1、新增语义化标签：<header>头部标签，<nav>导航标签，<article>内容标签，<section>定义文档某个区域,<aside>侧边栏标签，<footer>尾部标签。<br>
2、新增视频标签：video:src="视频地址"。 autoplay视频自动播放。 controls显示播放控件。 width,height修改视频大小。 loop视频循环播放。 muted静音播放，谷歌浏览器需要添加此属性。 poster加载等待的画面图片,视频文件最好用mp4格式<br>
3、新增音频标签：audio:src="视频地址"。 autoplay视频自动播放。 controls显示播放控件。 muted静音播放，谷歌浏览器需要添加此属性。 音频文件最好用mp3格式 <br>
4、新增表单属性：required表示内容不能为空，必填。placeholder="提示文本"，表单的默认提示信息。  autofocus自动聚焦到指定表单。  autocomolete=on/off 表示是否自动保存并显示历史记录，一般为off。  multiple可以多选文件提交<br>
<h2>CSS3提高</h2>
<h3>新增属性选择器</h3>
属性的选择必须用中括号包起来<br>
1、选择具有某属性的标签，例如：input[value]表示选中包含value属性的input标签<br>
2、选择属性等于某值的标签，例如：input[type="text"]表示选中type值等于text的input标签<br>
3、选择属性以某个值为开头的标签，例如：input[class^="icon"]表示选择以icon为开头的含有class属性的标签<br>
4、选择属性以某个值为结尾的标签，例如：input[class$="data"]表示选择以data为结尾的含有class属性的标签<br>
5、选择属性中含有某个值的标签，例如：input[class*="age"]，只要属性的值中含有age即可被选中<br>
<h2>结构选择器</h2>
结构选择器通常用来选择后代属性，用冒号连接<br>
1、选择第一个子元素，例如：ul li:first-child，可以选中ul中的第一个li元素<br>
2、选择最后一个子元素，例如：ul li:last-child,可以选中ul中的最后一个li元素<br>
3、选择任意一个或多个子元素nth-child(n)，n的值是从0开始的。例如：ul li:nth-child(2),可以选中ul中的第二个li元素，child(n)中的n可以是任意数字、关键字或公式，例如：ul li:nth-child(even/odd)可以选中偶数或奇数的子代。若写公式，括号内的字母只能为n，例如：ol li:nth-child(2n/2n+1/...)，可以根据公式灵活选择子代<br>
4、与nth-child(n)对应的是nth-of-type(n),两者的用法和效果基本相同，但是nth-child在使用时会将所有的元素排序，在执行时首先看 :nth-child(n),然后再回头看是什么类型，即先找到第n个子代，再匹配前面的元素类型，因此若子元素中的类型不同则不容易选中对应的元素。而nth-of-type在执行时只会将对应类型的元素排序，如：section div:nth-of-type(1),在执行时首先看div，然后再看nth-of-type(1)，即先匹配前面的元素类型，再找到第n个子代，最后选中子元素中第一个div元素。<br>
<h3>伪元素选择器</h3>
1、语法：element::before/after{content='' },before和after会创建一个行内元素,创建的元素会插入element的前面或后面<br>
2、伪元素属于element的子代<br>
<h3>CSS过渡</h3>
1、语法：transition:要过渡的属性  花费时间(s)  运动曲线（速度）  何时开始（延迟）；最后两个一般可以省略<br>
2、属性：想要变化的css属性，宽，高，背景颜色等都可以，如果想要过渡所有属性，将第一个值写成all即可<br>
<h3>2D转换</h3>
1、移动：transform:translate(x,y);或者分开写translateX(),translateY()，translate对行内标签没有作用，但不会影响到其他元素，移动时以x,y轴为基准，其中的百分比单位是相对于自身大小的。可以配合绝对定位实现盒子的垂直水平居中。如：<br>
<pre>
	div {
	position:absolute;
	top:50%;
	left:50%;
	transform:translate(-50%,-50%);
	}

</pre>
2、旋转：transform:rotate(度数),单位时deg，正数顺时针，负数逆时针，默认旋转点是元素中心。transform-origin：x,y可以改变旋转的中心点，x,y可以是具体数值也可以是方位名词(top, left, bottom, right)。<br>
3、缩放：transform:scale(x,y);x,y代表放大的倍数，若小于一则缩小，这种方法不会影响其他元素，且可以设置中心点的位置。<br>
4、transform简写：transform:translate()  rotate()  scale()  顺序不能改变。<br>
<h3>animation动画</h3>
1、定义动画，例：<br>
<pre>
	@keyframes 动画名称 {
	#动画开始状态
	0%(from) {
	    transformX:translate(0);
	}
	#中间可以添加其他状态：25%，...等。
	#结束状态
        100%(to) {
	      transformY:translate(200px);
        }
	}
</pre>
2、调用动画<br>
<pre>
	div {
	     animation-name: 动画名称;
	     animation-duration: 持续时间(s)
	}
</pre>
3、常用属性：<br>
<strong>
	animation-delay:规定动画何时开始<br>
	animation-iteration-count:规定动画的播放次数<br>
	animation-direction:规定动画是否在下一周期逆向播放,默认是normal,alternate逆向播放<br>
	animation-play-state:控制动画的播放和暂停，默认是running，还有paused<br>
	animation-fill-mode:规定动画结束后的状态，forwards保持backwards回到起始<br>
	简写属性：animation:名称  持续时间  运动曲线  何时开始  播放次数  是否反方向  结束状态
</strong>
<h2>3d转换</h2>
1、3d转换：transform:translate3d(x,y,z),z轴由屏幕向外为正,每个属性值都不能省略，若不需要就写0。<br>
2、透视:perspective:500px；3d效果的实现必须借助于透视属性，透视属性要加在元素的父盒子上，通过透视可以实现元素近大远小的效果，透视值越小元素越大，透视值越大元素越小。<br>
3、3D旋转：rotateX(deg),rotateY(deg),rotateZ(deg),正值是向里旋转。也可以自定义旋转rotate(x,y,z,deg),可以看作矢量，如1,1,0,即沿着对角线旋转。<br>
4、3D呈现：transform-style:默认flat平面展示，还有preserve-3d保留子元素的3d状态<br>
<h2>flex弹性布局</h2>
通过给父盒子添加flex属性从而控制子盒子的位置和排列方式。flex会使子级中的float、clear、vertic-align等属性失效。
<h3>父项常见属性</h3>
1、改变主轴，默认是x轴row，元素沿着主轴排列。flex-direcion: row/row-revers/column/column-revers<br>
2、设置主轴上元素的排列方式，justify-content:flex-start默认值，从主轴的头部开始。flex-end从尾部开始排列。center在主轴居中对齐。space-around平分剩余空间。space-between先两边贴边再平分剩余空间<br>
3、flex-wrap控制盒子(在一行中装不下时)是否换行,默认值是nowrap不换行，wrap换行。<br>
4、设置侧轴上的排列方式（单行）:align-items:flex-start默认值从上到下，flex-end从下到上，center垂直居中,stretch拉伸(子盒子不能给高度)<br>
5、设置侧轴上的排列方式（多行）:align-content:flex-start默认值头部开始，flex-end尾部开始，center侧轴居中,space-around子项在侧轴平分空间，space-between子项先在侧轴两头分布再平分空间，stretch子项平分父元素的高度<br>
<h3>子项常见属性</h3>
1、flex属性，定义子项分配剩余空间，用flex表示所占份数。flex:number，默认为0，使用此属性时最好不要给元素宽度，可以自动填充<br>
2、align-self:控制单独某个盒子的排列方式
