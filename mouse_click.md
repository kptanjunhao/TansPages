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
	var val = document.getElementById("count_btn").innerHTML;
	document.getElementById("count_btn").innerHTML = 1 + parseInt(val);
}



</script>

<table width="100%" height="100%">

<tr>
<td align="center">
<button style="width:100px;height:100px;font-size:32px" id="count_btn" onclick="btn_click();">0</button>
</td>
</tr>

</table>