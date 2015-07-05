# touchslider

##less 样式
```
.wcontainer {
	width: 100%;
	height: auto;
	.sliders {
	width: 100%;
	height: 245px;
	overflow: hidden;
		.sliderlist{
			width:100%;
			height:245px;
			float:left;
			img{
				width:inherit;
				height:inherit;
			}
		}
	}
}
```

##html结构
```
<div class="wcontainer">
	<div class="sliders" id="sliders">
		<div  class="sliderlist" ng-repeat="picurl in productDetailData.picUrlArr">
			<img ng-src="{{picurl}}" alt="">
		</div>
	</div>
</div>
```

##使用方法
```
$("#sliders").touchSlider({
	animatetime:300,
	automatic:!0,
	timeinterval:4e3,
	sliderpoint:!0,
	sliderpointwidth:8,
	sliderpointcolor:"#fa9d00"
});
```