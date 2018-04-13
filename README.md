# viewRecorder
ImageLife is Jquery Plugin purpose for recording activity when user visit a website

## Live Demo
<a href="http://rockman84.github.io/viewRecorder/">http://rockman84.github.io/viewRecorder/</a>

## Usage
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
## Config
- interval (default: 500) milisecond
- mark_classname (default: vr-mark)
- pointer_idname (default: vr-pointer)
- target (default: window)
```
var recorder = viewRec({
	interval: 200,
	mark_classname: 'vr-mark'
});
```
## Method
### Start Record
```
recorder.startRecord();
```
### Stop Record
```
recorder.stopRecord();
```
### Play
```
recorder.play();
```
### Stop Play
```
recorder.stop();
```
### Clear data record
```
recorder.clearData();
```
### Get data record
```
recorder.getData();
```
### Set data record
```
var data = [];
recorder.setData(data);
```
### Clear Mark Click
```
recorder.clearMark();
```
### Event
```
recorder.on('event_name',function(){
	// event do
});
```

## Event available
- recording
- stop_record
- play
- stop

