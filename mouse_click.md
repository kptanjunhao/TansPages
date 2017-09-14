---
layout: default
---

[Back to Index](index).

<script>

var click = 0;
var int=self.setInterval("count_clear()",1000);

function count_clear(){
	document.getElementById("count_btn").innerHTML = 0;
}

function btn_click(){
	var val = parseInt(document.getElementById("count_btn").innerHTML);
	document.getElementById("count_btn").innerHTML = 1 + val;
    var max = parseInt(document.getElementById("max_click").innerHTML);
    if(val >= max){
        document.getElementById("max_click").innerHTML = 1 + val;
    }
}



</script>

<table style="width:100%;height:100%;font-size:32px">

<tr>
<td align="center">
<button style="width:100px;height:100px" id="count_btn" onclick="btn_click();">0</button>
</td>
<td>
当前最大点击数:
<div id="max_click">0</div>
</td>
</tr>

</table>