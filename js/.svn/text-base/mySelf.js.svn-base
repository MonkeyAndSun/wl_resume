$(function() {

	         /*初始化代码*/

	FastClick.attach(document.body);
	var mySwiper = new Swiper('.swiper-container', {
		direction: 'vertical',
		loop: true,
		onInit: function(swiper) { //Swiper2.x的初始化是onFirstInit
			swiperAnimateCache(swiper); //隐藏动画元素 
			swiperAnimate(swiper); //初始化完成开始动画
		},
		onSlideChangeEnd: function(swiper) {
			swiperAnimate(swiper); //每个slide切换结束时也运行当前slide动画
		}
	})
	
	           /*音乐按钮*/
	var audio = document.querySelector("audio")
    var autoPlay = document.querySelector("#autoPlay")
    window.setTimeout(function() {
    	audio.play();
    	autoPlay.className="music play"
    }, 500);
	autoPlay.onclick=function(){
		if(audio.paused){
			console.log(2222)
			audio.play()
			autoPlay.className="music play"
		}else{
			console.log(111)
			audio.pause()
			autoPlay.className="music"
		}
		
		console.log(audio.played)
	}
})