10.16 09:03
jQuery动态随机修改id
<script type="text/javascript">


$(document).ready(function(){
  $("#button1").click(function(){
    

var colors = ['a','b','c','d','e','f','g'];


var x = colors[(Math.floor(Math.random() * (colors.length)))]



var colorsxy = ['a','b','c','d','e','f','g'];


var xy = colorsxy[(Math.floor(Math.random() * (colorsxy.length)))]



//$("#to").attr('id','xx');//之后变成xx
 

$("#"+x).val(Math.floor(Math.random()*7+1));



$("#a").attr('id','g');

$("#b").attr('id','f');


$("#c").attr('id','e');


$("#d").attr('id','d');

$("#e").attr('id','c');


$("#f").attr('id','b');


$("g").attr('id','a');



  });
});
</script>

