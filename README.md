# viewRecorder

##Usage
add script link inside header tag
```
<script language="javascript" href="view_recorder.js"></script> 
```
add style script
```
<style>
.vr-mark{
	width:30px;
	height:30px;
	border:1px solid #000;
	z-index:5000;
}
#vr-pointer{
	background:url('mouse.png');
	height:27px;
	width:15px;
	z-index:5000;
}
</style>
```
and
```
// set configure
var recorder = viewRec({interval:500});
 
// start record
recorder.startRecord();
 
// stop record
recorder.stopRecord();
 
// play record
recorder.play(); 
```

##Method
###Start Record
```
recorder.startRecord();
```
###Stop Record
```
recorder.stopRecord();
```
###Play
```
recorder.play();
```
###Stop Play
```
recorder.stop();
```
###Clear data record
```
recorder.clearData();
```
###Get data record
```
recorder.getData();
```
###Set data record
```
var data = [];
recorder.setData(data);
```
