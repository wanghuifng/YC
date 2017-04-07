# jquery.slides

一款基于jQuery无缝轮播图插件,支持图内元素动画，可以自定义动画类型
##### 兼容性:
`ie8+` `google` `firefox` `360` `QQ` `欧朋` `safi`
## javascript
```javascript
$(".slideInner").slide({

	slideContainer: $('.slideInner a'),
	
	effect: 'easeOutCirc',//动画类型
	
	autoRunTime: 5000,//自动轮播时间
	
	slideSpeed: 1000,//速度
	
	nav: true,//是否显示左右导航
	
	autoRun: true,//是否自动滚动
	
	prevBtn: $('a.prev'),//左按钮
	
	nextBtn: $('a.next')//右按钮
	
	});
```


## html实例：

slides默认会为个个滑块里面的类名为moveElem的元素添加上动画的效果
元素上的rel属性则是设置对应的 延迟执行时间和动画类型两个属性
每个滑块内可同时添加多个元素
``` html
	<body>
		<div class="slides">
			<div class="slideInner">
				<a href="#" style="background: url(img/slide1.jpg) no-repeat;">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				<a href="#" style="background: url(img/slide2.jpg) no-repeat">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide2p1.png" />
					</div>
				</a>
				<a href="#" class="slide3" style="background: url(img/slide3.jpg) no-repeat;">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide3p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide3p2.png" />
					</div>
					<div class="moveElem img3" rel="300,easeInOutExpo">
						<img src="img/slide3p3.png" />
					</div>
				</a>
				<a href="#" style="background: rgb(113, 209, 231);">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				<a href="#" style="background: rgb(178, 44, 44);">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				
			</div>
			<div class="nav">
				<a class="prev" href="#"></a>
				<a class="next" href="#"></a>
			</div>
		</div>
	</body>
```

