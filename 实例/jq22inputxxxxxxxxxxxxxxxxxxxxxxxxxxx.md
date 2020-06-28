

<!doctype html>
<html>
<head>
<title>表格内容的增删（原创）</title>
<meta name="description" content="对表格内容进行增加删除" />
<meta name="keywords" content="表格，增加，删除,修改,原创" />
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="renderer" content="webkit">

<link href="/css/bootstrap.min.css" rel="stylesheet" media="screen">
<link href="/fonts/font-awesome.min.css" rel="stylesheet" media="screen">
<!--[if lt IE 9]>
 	<script src="/js/respond.min.js"></script> 
	<script src="/js/html5shiv.min.js"></script>    
<![endif]-->
<link href="/css/my.css" rel="stylesheet" media="screen">
<link href="/css/dl.css" rel="stylesheet" media="screen">
<link rel="stylesheet" type="text/css" href="/css/wangEditor.css">
<script src="/js/jquery.min.js"></script>
<script src="/js/bootstrap.min.js"></script>
<script>var n = 1; var cfzi = 1;</script>
<script src="/js/m.js"></script>
<script src="https://cdn.bootcss.com/ace/1.2.6/ace.js"></script>
<script src="ace/ext-language_tools.js"></script>
<script src="/js/f.js"></script>
<style>
    html,body{height:100%}body{overflow-y:hidden;}.zuo h6{margin-bottom:10px;}.zuo h4{padding-bottom:10px;}iframe{padding:0px;margin:0}.webleft{float:left;position:relative;width:220px;background:#fff;height:100%;margin-right:-220px;}.webright{float:right;width:100%;height:100%;}.webright_content{margin-left:220px;height:100%;}.web50{width:50%;float:left;height:100%;background-color:#e4e3e3;}.dtab{width:98%;height:88%;margin-top:10px;margin-left:1%;padding-top:10px;padding-bottom:5px;background-color:#fbfbfb;border-radius:7px 7px 0px 0px;overflow:hidden;box-sizing:border-box;background-clip:padding-box,border-box;background-origin:padding-box,border-box;position:relative;}.dtop{position:absolute;top:10px;left:0;width:100%;height:35px;}.dtab ul{display:block;width:30.6666%;padding:0;margin:0;float:left;line-height:34px;text-align:center;cursor:pointer;transition:all .5s ease 0s;border-top-left-radius:5px;border-top-right-radius:5px;}.dtab ul:hover{border:1px solid #559ece;border-bottom:0px;background-color:#bdf9ff;font-weight:bold;}.dtab .dz{margin-top:7px;border:1px solid #e8e8e8;border-bottom:0px;background-color:#f1f1f1;font-weight:bold;color:#828282;font-family:Verdana;}.dtab .dq{margin-top:0px;border:1px solid #1e1e1e;border-bottom:0px;background-color:#fff;font-weight:bold;transition:all .5s ease 0s;color:#000;}.dtad li{display:block;float:left;margin-left:5px;width:15px;height:15px;background-color:#e4514f;border-radius:15px;}.dt1{height:95%;margin-top:35px;background-color:#2f2e2e}.dt2{height:60%;margin-top:35px;}.dt3{height:40%;background-color:#fff}.dtac .dz{margin-left:0.5%;margin-right:0.5%}#editor,#editor2,#editor3{width:100%;height:100%;}.prekj{height:95%;}pre{border-radius:0px;}.dtop h2{font-size:1.3em;font-weight:550;padding-left:20px;line-height:30px;}.dtadown{height:10%;width:98%;margin-left:1%;background-color:#2f2e2e;border-radius:0px 0px 7px 7px;position:relative;}.dtadownbut{height:65%;width:25%;background-color:#d9534f;text-align:center;position:absolute;top:0;right:1.5%;bottom:0;margin:auto;}.mlz pre{padding:5px;font-size:12px;background-color:#fff;border:1px dashed #CCCCCC;border-radius:4px;overflow:auto;}.dtadownbut .inner2{display:inline-block;position:relative;top:50%;color:#fff;transform:translateY(-50%);}@media screen and (max-width:1000px){.webleft{display:none;}.webright_content{margin-left:0px;}}.cjms,.cjms2{width:96%;margin-left:2%;}::-webkit-scrollbar{width:5px;height:5px;background-color:#F5F5F5;}::-webkit-scrollbar-track{-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.3);background-color:#F5F5F5;}::-webkit-scrollbar-thumb{border-radius:5px;-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,.3);background-color:#555;}::-webkit-scrollbar-thumb:hover{background-color:#2b93e6;}.mlztx{width:60px;height:60px;border-radius:60px;background-color:#2b93e6;position:fixed;bottom:50px;right:20px;-webkit-box-shadow:0px 0px 2px 3px hsla(0,0%,0%,0.1);box-shadow:0px 0px 2px 3px hsla(0,0%,0%,0.1);font-size:30px;text-align:center;line-height:55px;color:#fff;transition:all 1s ease 0s;z-index:99;}.mlz{width:687px;position:fixed;bottom:125px;background-color:#FFFFFF;right:20px;border-radius:5px;border:1px solid #2b93e6;z-index:99;display:none}.mlz ul{padding:7px;padding-bottom:0px;margin-bottom:0px}.mlz h4{background-color:#2b93e6;color:#fff;padding-left:10px;line-height:30px;font-size:14px;margin:0px;margin-bottom:4px;border-radius:5px;}.mlztx{opacity:.6;width:60px;height:60px;border-radius:60px;background-color:#2b93e6;position:fixed;bottom:50px;right:20px;font-size:30px;text-align:center;line-height:55px;color:#fff;transition:all 1s ease 0s;z-index:99}.mlztx:hover{opacity:1;background-color:#00b1ff;width:65px;height:65px}.msagely pre{padding:5px;font-size:12px;background-color:#fff;border:1px dashed #CCCCCC;}.mlz::-webkit-scrollbar{width:5px;height:5px;}.mlz::-webkit-scrollbar-track{background:#2b93e6;}.mlz::-webkit-scrollbar-thumb{background:#2b93e6;border-radius:5px;}.mlz::-webkit-scrollbar-thumb:hover{background:#3d89c4;}.mlz::-webkit-scrollbar{width:5px;height:5px;}.mlz::-webkit-scrollbar-track{background:#dedede;}.mlz::-webkit-scrollbar-thumb{background:#2b93e6;border-radius:5px;}.mlz::-webkit-scrollbar-thumb:hover{background:#000;}.mlz-scrollbar-filler{background:#000;}.mypl1,.mypl2{display:block;text-align:center;line-height:30px}.msagely p{word-break:break-word;}.plbg{margin-bottom:10px;}.msagely{background-color:#fbfbfb;border-bottom-width:1px;border-bottom-color:#b2d4de;padding-top:5px;padding-bottom:5px;position:relative;margin-bottom:5px;padding-left:7px;padding-right:5px;transition:all 1s ease 0s;}.mlz ul{padding:0px;}.pl ul{padding:0px 10px;line-height:26px;}.pl pre{font-size:12px;}.tx{left:-45px;width:45px;}.ace_folding-enabled > .ace_gutter-cell{color:#7b7b7b;}.cjms2{height:65%;overflow:auto}.huif2{width:680px;position:fixed;bottom:125px;z-index:999;right:26px;background-color:#f7f7f7;border-radius:5px;border-top:1px solid #B9B9B9;display:none;}.huif2 ul{padding:20px}@media screen and (max-height:1200px){.cjms2{height:68%;}}@media screen and (max-height:1140px){.cjms2{height:63%;}}@media screen and (max-height:1000px){.cjms2{height:59%;}}@media screen and (max-height:920px){.cjms2{height:53%;}}@media screen and (max-height:840px){.dt1{height:93%;}.dt2{height:50%;}.cjms2{height:75%;}}@media screen and (max-width:800px){.web50{width:100%;}body{overflow-y:auto;}}@media screen and (max-width:770px){.mlz,.huif2{width:90%;}}@media screen and (max-height:770px){.cjms2{height:68%;}}@media screen and (max-height:680px){.mlz{height:60%;}.cjms2{height:58%;}}@media screen and (max-height:640px){.dt1{height:91%;}.cjms2{height:55%;}}.mpl{color:#fff;padding-left:10px}.mpl:hover{color:#acdfff;}.corfff{color:#909090;padding:10px;}.inner2 a{display:block;color:#fff}.ace_editor.ace_autocomplete .ace_completion-highlight{color:#00b317;font-weight:600;text-shadow:0 0 0;}.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line{background-color:#235f36;}.ace_editor.ace_autocomplete{border-radius:3px;background:#333333;border:1px #040404 solid;color:#c1c1c1;}.webul{padding-top:5px;padding-bottom:5px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}.webul a{color:#2f2e2e;transition:all .5s ease 0s;}.webul a:hover{color:#2b93e6;text-decoration:none;padding-left:10px;}.dong{transition:all 1s ease 0s;}.pl{font-weight:400;}
        .cjms2 p{font-weight:400}.pl {margin-top: 10px;}.mlztx span{position:absolute;top:-12px;right:10px;font-size:12px;}.mlztx{animation:ripple 0.6s linear 5;}@keyframes ripple{0%{box-shadow:0 0 0 0 rgba(93,190,219,0.2),0 0 0 10px rgba(93,190,219,0.2),0 0 0 20px rgba(93,190,219,0.2),0 0 0 30px rgba(93,190,219,0.2);}100%{box-shadow:0 0 0 10px rgba(93,190,219,0.2),0 0 0 20px rgba(93,190,219,0.2),0 0 0 30px rgba(93,190,219,0.2),0 0 0 40px rgba(93,190,219,0);}}
       .xgdm{width:100%;height:auto}.xgdm a{display:block;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;line-height:26px;color:#525252;transition:all .3s ease 0s;border-top:1px solid #F4F4F4;}.xgdm a:hover{text-decoration:none;color:#0C8AFF;padding-left:5px;}.cjms2 pre{font-size:13px;font-weight:400;padding:10px;border-radius:5px;border:1px dashed #dcdcdc;margin:5px;background-color:#fffdfa;}
        .cjms2 h3 {padding-top:15px} .cjms2 p {padding-bottom:10px}textarea{outline:none;border:0px;transition:1s;border:1px solid #DDDDDD;-moz-box-shadow:2px 2px 4px #f5f5f5 inset;-webkit-box-shadow:2px 2px 4px #f5f5f5 inset;box-shadow:2px 2px 4px #f5f5f5 inset;padding:10px}textarea:focus{outline:none !important;background-color:#fafbf5;border:1px solid #4ca957;-moz-box-shadow:2px 2px 4px #e8e9e4 inset;-webkit-box-shadow:2px 2px 4px #e8e9e4 inset;box-shadow:2px 2px 4px #e8e9e4 inset;}textarea::-webkit-input-placeholder{color:#A4A4A4;}textarea::-moz-placeholder{color:#A4A4A4;}textarea:-moz-placeholder{color:#A4A4A4;}textarea:-ms-input-placeholder{color:#A4A4A4;}
    </style>
</head>
<body data-spy="scroll" data-target=".navbar-example">

<nav class="navbar navbar-inverse navbar-fixed-top">
<div class="container-fluid">
<div class="navbar-header">
<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar"> <span class="sr-only">Toggle navigation</span> <span class="icon-bar"></span> <span class="icon-bar"></span> <span class="icon-bar"></span> </button>
<a class="navbar-logo" href="http://www.jq22.com/"><img src="https://www.jq22.com/img/logo.png" height="100%" alt="jQuery插件,jQuery,jQuery特效.jQuery ui,jQuery 教程,css3,网页特效,JS特效"></a> </div>
<div id="navbar" class="navbar-collapse collapse">
<ul class="nav navbar-nav navbar-right">
<li><a href="http://www.jq22.com/daima"><i class="fa fa-code"></i> &nbsp;在线代码</a></li>
<li><a href="https://www.jq22.com/webide"><i class="fa fa-edit"></i> &nbsp;在线编辑器</a></li>
<li><a href="http://www.jq22.com/textDifference"><i class="fa fa-balance-scale" aria-hidden="true"></i> &nbsp;文本比较</a></li>
<li><a href="http://www.jq22.com/jquery-info122"><i class="fa fa-download"></i> &nbsp;jQuery下载</a></li>
<li><a href="https://www.jq22.com/jquery/jquery.html" target="_blank"><i class="fa fa-ship" aria-hidden="true"></i> &nbsp;前端库</a></li>
<li><a href="https://www.jq22.com/chm/jquery/index.html" target="_blank"><i class="fa fa-book"></i> &nbsp;在线手册</a></li>
<li class="dropdown"><a rel="nofollow" href="https://weibo.com/jq22" target="_blank"><i class="fa fa-weibo"></i> &nbsp;微博</a></li>
<li>
<a href="#" data-toggle="modal" data-target="#myModal">
<i class="fa fa-user"></i> &nbsp;注册/登录<span class="sr-only">(current)</span></a>
</li>
</ul>
</div>

</div>
</nav>


<div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
<div class="modal-dialog">
<div class="modal-content2 tcc">
<div class="modal-header2 top20">
<button type="button" class="close" data-dismiss="modal" aria-hidden="true">
&times;
</button>
<h4 class="modal-title" id="myModalLabel">
</h4>
</div>
<div class="modal-body tcck">
<div class="input-group input-group-lg parentCls">
<span class="input-group-addon" id="email"><i class="fa fa-envelope-o"></i></span>
<input type="text" class="form-control inputElem" placeholder="请输入登录邮箱" aria-describedby="email" id="ema" style="width: 466px;">
</div>
<div class="input-group input-group-lg top20">
<span class="input-group-addon" id="pwd"><i class="fa fa-unlock-alt" style="width:18px"></i></span>
<input type="password" class="form-control" placeholder="请输入登录密码" aria-describedby="pwd" id="pw">
<span class="input-group-btn tccBut">
<button class="btn btn-success" type="button" onclick="emdl()">登 录</button>
</span>
</div>
</div>
<div class="modal-footer2">
<div class="f">
<a href="pwd.aspx">忘记密码?</a></div>
<div class="r"><a href="register.aspx">注册新用户</a></div>
<div class="dr"></div>
</div>
<div class="d3f modal-body tcck2">
<a href="#" onClick="tz()" class="qq"></a>
<a href="https://api.weibo.com:443/oauth2/authorize?client_id=3364913104&redirect_uri=http%3A%2F%2Fwww.jq22.com%2FWeiboReturn.aspx&response_type=code&display=default" class="sina"></a>
<a href="https://www.jq22.com/zfbReturn.aspx" class="zfb"></a>
<a href="#" onClick="gt()" class="git"></a>
</div>
<script>          
             function tz() {
                 var urldz = "https://graph.qq.com/oauth2.0/authorize?response_type=code&client_id=101135281&redirect_uri=http://www.jq22.com/QQReturn.aspx?tjurl=" + window.location.href;
                window.location.href = urldz;
             }
             function gt() {
                 var urldz = "https://github.com/login/oauth/authorize?client_id=cf869185ea7d8fcab6df&state=jq22&redirect_uri=http://www.jq22.com/github.aspx?tjurl=" + window.location.href;
                 window.location.href = urldz;
             }
         </script>
</div>
</div>
</div>

<div class="yn jz container-fluid nav-bgn m0 visible-lg visible-md visible-sm" id="menu_wrap">
<div class="container m0" style="position:relative;"><a class="nzz" href="http://www.jq22.com/jqueryUI-1-jq" id="z1"><span class="sort"><i class="fa fa-paint-brush"></i>&nbsp;UI <i class="fa fa-angle-down"></i></span></a>|<a class="nzz" href="http://www.jq22.com/jquery输入-1-jq" id="z2"><span class="sort"><i class="fa fa-keyboard-o"></i>&nbsp;输入 <i class="fa fa-angle-down"></i></span></a>|<a class="nzz" href="http://www.jq22.com/jquery媒体-1-jq" id="z3"><span class="sort"><i class="fa fa-film"></i>&nbsp;媒体 <i class="fa fa-angle-down"></i></span></a>|<a class="nzz" href="http://www.jq22.com/jquery导航-1-jq" id="z4"><span class="sort "><i class="fa fa-paper-plane-o"></i>&nbsp;导航 <i class="fa fa-angle-down"></i></span></a><span class="navxs">|<a class="nzz" href="http://www.jq22.com/jquery其他-1-jq" id="z5"><span class="sort"><i class="fa fa-dropbox"></i>&nbsp;其他 <i class="fa fa-angle-down"></i></span></a></span><span class="navxs">|<a href="http://www.jq22.com/jquery-plugins布局-1-jq" target="_blank"><span class="sort"><i class="fa fa-th-large"></i>&nbsp;网页模板</span></a>|<a href="http://www.jq22.com/jqueryAPP模板-1-jq" target="_blank"><span class="sort"><i class="fa fa-tablet"></i>&nbsp;APP模板</span></a>|<a href="http://www.jq22.com/webinfo1" target="_blank"><span class="sort"><i class="fa fa-file-code-o"></i>&nbsp;常用代码</span></a>|<a href="http://www.jq22.com/daima" target="_blank"><span class="sort"><i class="fa fa-code"></i>&nbsp;在线代码</span></a></span></div>
<style>.sort {padding-right: 20px; padding-left: 20px;} @media screen and (max-width:1220px) {.azj {display: none}.sort {padding-right: 10px; padding-left: 10px;}}</style>
<div class="container-fluid"><div id="n1" class="nav-zi ty" style="display: none;"><ul id="nz1" class="nn list-inline container m0" style="display: none;"><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins背景-1-jq"><i class="fa fa-delicious ls"></i>背景</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins对话框和灯箱-1-jq"><i class="fa fa-bell-o ls"></i>对话框和灯箱</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins筛选及排序-1-jq"><i class="fa fa-sort-numeric-desc ls"></i>筛选及排序</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins反馈-1-jq"><i class="fa fa-comments-o ls"></i>反馈</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins弹出层-1-jq"><i class="fa fa-stack-overflow ls"></i>弹出层</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins悬停-1-jq"><i class="fa fa-hand-o-up ls"></i>悬停</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins布局-1-jq"><i class="fa fa-th-large ls"></i>布局</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins图表-1-jq"><i class="fa fa-bar-chart ls"></i>图表</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins加载-1-jq"><i class="fa fa-spinner ls"></i>加载</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins圆边-1-jq"><i class="fa fa-circle-o ls"></i>圆边</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins滚动-1-jq"><i class="fa fa-long-arrow-down ls"></i>滚动</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins标签-1-jq"><i class="fa fa-tags ls"></i>标签</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins文本链接-1-jq"><i class="fa fa-link ls"></i>文本链接</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins工具提示-1-jq"><i class="fa fa-info-circle ls"></i>工具提示</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins网络类型-1-jq"><i class="fa fa-code-fork ls"></i>网络类型</a></li></ul><ul id="nz2" class="nn list-inline container m0" style="display: none;"><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins拾色器-1-jq"><i class="fa fa-eyedropper ls"></i>拾色器</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins定制和风格-1-jq"><i class="fa fa-paint-brush ls"></i>定制和风格</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins日期和时间-1-jq"><i class="fa fa-clock-o ls"></i>日期和时间</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins拖和放-1-jq"><i class="fa fa-arrows ls"></i>拖和放</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins通用输入-1-jq"><i class="fa fa-keyboard-o ls"></i>通用输入</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins自动完成-1-jq"><i class="fa fa-calculator ls"></i>自动完成</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins密码-1-jq"><i class="fa fa-lock ls"></i>密码</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins投票率-1-jq"><i class="fa fa-thumbs-up ls"></i>投票率</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins搜索-1-jq"><i class="fa fa-search ls"></i>搜索</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins选择框-1-jq"><i class="fa fa-caret-square-o-down ls"></i>选择框</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins快捷键-1-jq"><i class="fa fa-adn ls"></i>快捷键</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins触摸-1-jq"><i class="fa fa-hand-o-down ls"></i>触摸</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins丰富的输入-1-jq"><i class="fa fa-h-square ls"></i>丰富的输入</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins上传-1-jq"><i class="fa fa-upload ls"></i>上传</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins验证-1-jq"><i class="fa fa-key ls"></i>验证</a></li></ul><ul id="nz3" class="nn list-inline container m0" style="display: none;"><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins音频和视频-1-jq"><i class="fa fa-play-circle-o ls"></i>音频和视频</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins幻灯片和轮播图-1-jq"><i class="fa fa-exchange ls"></i>幻灯片和轮播图</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins图片展示-1-jq"><i class="fa fa-eye ls"></i>图片展示</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins图像-1-jq"><i class="fa fa-picture-o ls"></i>图像</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins地图-1-jq"><i class="fa fa-map-marker ls"></i>地图</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins滑块和旋转-1-jq"><i class="fa fa-arrows-h ls"></i>滑块和旋转</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-pluginsTabs-1-jq"><i class="fa fa-folder-o ls"></i>Tabs</a></li></ul><ul id="nz4" class="nn list-inline container m0" style="display: none;"><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins水平导航-1-jq"><i class="fa fa-long-arrow-right ls"></i>水平导航</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins垂直导航-1-jq"><i class="fa fa-long-arrow-down ls"></i>垂直导航</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins文件树-1-jq"><i class="fa fa-sitemap ls"></i>文件树</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins分页-1-jq"><i class="fa fa-chevron-right ls"></i>分页</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins手风琴菜单-1-jq"><i class="fa fa-trello ls"></i>手风琴菜单</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins其他导航-1-jq"><i class="fa fa-location-arrow ls"></i>其他导航</a></li></ul><ul id="nz5" class="nn list-inline container m0" style="display: none;"><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins动画效果-1-jq"><i class="fa fa-rocket ls"></i>动画效果</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins浏览器调整-1-jq"><i class="fa fa-expand ls"></i>浏览器调整</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins移动-1-jq"><i class="fa fa-arrows-v ls"></i>移动</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins独立的部件-1-jq"><i class="fa fa-cogs ls"></i>独立的部件</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins杂项-1-jq"><i class="fa fa-gift ls"></i>杂项</a></li><li><a class="c-btn c-btn--border-line" href="http://www.jq22.com/jquery-plugins游戏-1-jq"><i class="fa fa-gamepad ls"></i>游戏</a></li></ul></div></div>
</div>

<div class="container-fluid m0 bod" id="zt" style="margin-top: 50px; height: 100%; padding-bottom: -32px">
<div class="webleft" style="padding-bottom:82px">
<div class="affd affix-top" style="width: 200px; margin-left: 10px; margin-top: 10px;">
<ul class="zuo f ">
<h6>PROMULGATOR</h6>
<a href="../mem792516"><img src="../tx/54.png"></a>
<div class="zuox f">
<h4>yuebanzhou</h4>
<i class="fa fa-map-marker"></i> <span>河北省邢台市</span>
</div>
<button type="button" class="btn btn-z top20" onclick="zuozhe()"><i class='fa fa-plus-circle'></i> 关注作者 <span>(10)</span></button>
<button type="button" class="btn btn-z top10" onclick="sc()"><i class='fa fa-heart-o'></i> 收藏此代码 <span>(75)</span></button>
<div class="df"></div>
</ul>
<ul class="zuo f z12 dong webul" style="margin-top:10px">
<a href='webqd4412'> ← 随机点名（原创） </a>
</ul>
<ul class="zuo f z12 dong webul" style="margin-top:10px">
<a href='webqd4407'> → tab栏的排他功能 </a>
</ul>
<ul class="f zuo xgdm" style="margin-top:10px">
<h4 style="font-size: 16px;font-weight: bold;">相关代码</h4>
<a href="./webqd4408"><span class='HighLighter'>表格</span>内容的增删（原创）</a>
<a href="./webqd6009">列表实现<span class='HighLighter'>增加</span><span class='HighLighter'>删除</span></a>
<a href="./webqd6369"><span class='HighLighter'>增加</span><span class='HighLighter'>删除</span>上传数量（原创）</a>
<a href="./webqd2228">table<span class='HighLighter'>表格</span>动态添加<span class='HighLighter'>删除</span>行</a>
<a href="./webqd2793">js<span class='HighLighter'>表格</span>排序<span class='HighLighter'>删除</span>操作</a>
<a href="./webqd4632">tab导航切换关闭(原创)</a>
<a href="./webqd6518">vue表单动态数据交互</a>
</ul>
<div class="df"></div>
</div>
</div>
<div class="webright">
<div class="webright_content" style="padding-bottom:82px">
<div class="web50 zuoze" style="overflow-y:auto;">
<div class="dtab" style="background-image:-webkit-linear-gradient(to top, #1b1b1b, #fff); background-image:linear-gradient(to top,#1b1b1b, #fff);">
<div class="dtop">
<div class="dtac f" style="width:100%">
<ul class="dz dq" style="margin-left:2%">Html</ul>
<ul class="dz">Css</ul>
<ul class="dz">Js</ul>
<div class="df"></div>
</div>
</div>
<div class="dt1" style="display: block;">
<pre id="editor"></pre>
<pre id="pvhtm" style="display:none"><input type="button" value="生成表格" id="btn" class="button" />
<br />

<div id="dv">
    <table border="1" cellpadding="0" cellspacing="0">
        <thead>
            <tr>
                <td>姓名</td>
                <td>科目</td>
                <td>分数</td>
                <td>操作</td>
            </tr>
        </thead>
        <tbody id="tbd">

        </tbody>
    </table>
</div>

<input type="button" value="添加" id="btn2" class="button" /></pre>
</div>
<div class="dt1">
<div class="prekj">
<pre id="editor2">table {
	text-align:center;
}
thead td {
	width:100px;
	height:30px;
	background:#ccc;
}
tbody td {
	height:25px;
}
input {
	width:70px;
	height:20px;
}
.button {
	width:70px;
	height:30px;
	margin:10px 0 10px 0;
}
</pre></div>
</div>
<div class="dt1" ">
<pre id="editor3"></pre><textarea id="e3" style="display:none">    function zy$(id) {
        return document.getElementById(id)
    };
    var arr = [{
            "name": "张三",
            "subject": "语文",
            "score": "80"
        },
        {
            "name": "李四",
            "subject": "数学",
            "score": "78"
        },
        {
            "name": "王五",
            "subject": "英语",
            "score": "90"
        }
    ];
    //注册点击事件，生成现有表格
    zy$("btn").onclick = function() {
        //tbody中的内容只出现一次
        if (!zy$("tbd").firstElementChild) {
            //遍历arr
            for (var i = 0; i < arr.length; i++) {
                //创建一行
                var trObj = document.createElement("tr");
                //追加到tbody中
                zy$("tbd").appendChild(trObj);
                //修改ID值
                trObj.id = "cc" + i;
                //创建列
                //第一列
                var td1 = document.createElement("td");
                trObj.appendChild(td1);
                td1.innerHTML = arr[i].name;
                //第二列
                var td2 = document.createElement("td");
                trObj.appendChild(td2);
                td2.innerHTML = arr[i].subject;
                //第三列
                var td3 = document.createElement("td");
                trObj.appendChild(td3);
                td3.innerHTML = arr[i].score;
                //第四列
                var td4 = document.createElement("td");
                trObj.appendChild(td4);
                //创建a标签
                var aObj = document.createElement("a");
                td4.appendChild(aObj);
                //a的跳转地址
                aObj.href = "javascript:void(0)";
                aObj.innerText = "删除";
                //点击删除
                aObj.onclick = function() {
                    this.parentNode.parentNode.parentNode.
                    removeChild(this.parentNode.parentNode);
                };
            }
        }
    }

    //注册点击事件，添加
    zy$("btn2").onclick = function() {
        //创建一行
        var trObj = document.createElement("tr");
        //追加到tbody中
        zy$("tbd").appendChild(trObj);
        //创建列
        //一列
        var td1 = document.createElement("td");
        trObj.appendChild(td1);
        var input1 = document.createElement("input");
        td1.appendChild(input1);
        //二列
        var td2 = document.createElement("td");
        trObj.appendChild(td2);
        var input2 = document.createElement("input");
        td2.appendChild(input2);
        //三列
        var td3 = document.createElement("td");
        trObj.appendChild(td3);
        var input3 = document.createElement("input");
        td3.appendChild(input3);
        //四列
        var td4 = document.createElement("td");
        trObj.appendChild(td4);
        //a标签确定标签
        var aObj = document.createElement("a");
        td4.appendChild(aObj);
        aObj.href = "javascript:void(0)";
        aObj.innerText = "确定";
        //注册点击事件，确定
        aObj.onclick = function() {
            td1.innerText = input1.value;
            td2.innerText = input2.value;
            td3.innerText = input3.value;
            //点击确定之后，第四列会发生变化
            //删除现有第四列
            this.parentNode.parentNode.removeChild(this.parentNode);
            //创建新的第四列
            var td4 = document.createElement("td");
            trObj.appendChild(td4);
            //第四列中的内容
            var aObj = document.createElement("a");
            td4.appendChild(aObj);
            aObj.innerText = "删除";
            aObj.href = "javascript:void(0)";
            //删除
            aObj.onclick = function() {
                this.parentNode.parentNode.parentNode.removeChild(this.parentNode.parentNode);
            };
        };
        //a标签，取消标签
        var aObj2 = document.createElement("a");
        td4.appendChild(aObj2);
        aObj2.href = "javascript:void(0)";
        aObj2.innerText = "取消";
        //注册点击事件，取消
        aObj2.onclick = function() {
            this.parentNode.parentNode.parentNode.removeChild(this.parentNode.parentNode);
        };

    };</textarea>
</div>
</div>
<div class="dtadown">
<div class="f corfff z12">↑上面代码改变，会自动显示代码结果 jQuery调用版本：<b>1.11.3</div>
<a href="javascript:void(0)" onclick="dmdown()" data-toggle="modal" data-target="#mydown"><div class="r dtadownbut"> <div class="inner2"><i class="fa fa-cloud-download"></i> &nbsp;立即下载 </div></div></a>
<div class="dr"></div>
</div>
</div>
<script>
                    var e3 = $("#e3").val().replace(/</g, "&lt;");
                    e3 = e3.replace(/>/g, "&gt;");
                    $("#editor3").html(e3);
                    var editor = ace.edit("editor");
                    editor["\x73\x65\x73\x73\x69\x6f\x6e"]["\x73\x65\x74\x4d\x6f\x64\x65"]("\x61\x63\x65\x2f\x6d\x6f\x64\x65\x2f\x68\x74\x6d\x6c"); editor["\x73\x65\x74\x54\x68\x65\x6d\x65"]("\x61\x63\x65\x2f\x74\x68\x65\x6d\x65\x2f\x74\x77\x69\x6c\x69\x67\x68\x74"); editor["\x73\x65\x74\x4f\x70\x74\x69\x6f\x6e\x73"]({ enableBasicAutocompletion: true, enableSnippets: true, enableLiveAutocompletion: true }); var jEJbPLKFV1 = $("\x23\x70\x76\x68\x74\x6d")["\x68\x74\x6d\x6c"](); var XZZ2 = jEJbPLKFV1; editor["\x73\x65\x74\x56\x61\x6c\x75\x65"](XZZ2);
                    var editor2 = ace.edit("editor2");
                    editor2["\x73\x65\x73\x73\x69\x6f\x6e"]["\x73\x65\x74\x4d\x6f\x64\x65"]("\x61\x63\x65\x2f\x6d\x6f\x64\x65\x2f\x63\x73\x73"); editor2["\x73\x65\x74\x54\x68\x65\x6d\x65"]("\x61\x63\x65\x2f\x74\x68\x65\x6d\x65\x2f\x74\x77\x69\x6c\x69\x67\x68\x74"); editor2["\x73\x65\x74\x4f\x70\x74\x69\x6f\x6e\x73"]({ enableBasicAutocompletion: true, enableSnippets: true, enableLiveAutocompletion: true }); var NBmMYTr1 = $("\x23\x70\x76\x68\x74\x6d")["\x68\x74\x6d\x6c"]();
                    var editor3 = ace.edit("editor3");
                    editor3["\x73\x65\x73\x73\x69\x6f\x6e"]["\x73\x65\x74\x4d\x6f\x64\x65"]("\x61\x63\x65\x2f\x6d\x6f\x64\x65\x2f\x6a\x61\x76\x61\x73\x63\x72\x69\x70\x74"); editor3["\x73\x65\x74\x54\x68\x65\x6d\x65"]("\x61\x63\x65\x2f\x74\x68\x65\x6d\x65\x2f\x74\x77\x69\x6c\x69\x67\x68\x74"); editor3["\x73\x65\x74\x4f\x70\x74\x69\x6f\x6e\x73"]({ enableBasicAutocompletion: true, enableSnippets: true, enableLiveAutocompletion: true });
                 </script>
<div class="web50">
<div class="dtab" style="height:98%">
<div class="dtop" style="border-bottom: 1px solid #e8e8e8;height: 35px;">
<div class="f"><h2>表格内容的增删（原创）</h2></div>
<div class="r">
<div class="bdsharebuttonbox" data-tag="share_1">
<a class="ttqq" data-cmd="sqq" title="分享到QQ好友"></a>
<a class="ttwx" data-cmd="weixin" href="#"></a>
<a class="ttqzone" data-cmd="qzone"></a>
<a class="ttsina" data-cmd="tsina"></a>
<a class="ttbdhome" data-cmd="bdhome"></a>
<a class="ttfbook" data-cmd="fbook"></a>
<a class="ttmore" data-cmd="more"></a>
</div>
</div>
<div class="dr"></div>
</div>
<div class="dt2">
<iframe class="ifcss" id="if" src="" style="height:100%; width:100%"></iframe>
</div>
<div class="dt3">
<div class="alert cjms top20" role="alert">代码描述：对表格内容进行增加删除</div>
<div class="cjms2 top20"></div>
</div>
</div>
</div>
<div class="mlztx"><span>4</span><i class="fa fa-comments"></i></div>
<div class="mlz" style="overflow: auto; max-height: 500px;">
<ul class="mm1">
<div style="background-color: #2b93e6">
<div class="f"><h4><i class="fa fa-comment"></i> 最新</h4>
</div><div class="r" style="line-height: 32px; padding-right: 10px;"><a class="mpl" href="#xpl"><i class="fa fa-pencil-square-o"></i> 发表评论</a> <a class="mpl" href="webpl4408"><i class="fa fa-comments"></i> 全部评论</a> <a class="mpl mplgb" href="javascript:void(0);"><i class="fa fa-times"></i></a></div>
<div class="df"></div>
</div>
<div class="mypl1" style="display: none;">暂时没有评论！</div>
<div class="pl">
<div class="tx"><a href="http://www.jq22.com/mem827914"><img src="//www.jq22.com/tx/31.png"></a></div>
<ul class="plbg">
<div class="f"> Felix<span class="jl">0</span></div>
<div class="r"> <span class="z12">2018/5/14 15:23:50</span></div>
<div class="dr"></div>
</ul>
<ul style="word-wrap: break-word;width: 100%;padding-top:5px">
求助<br>
<ul style="padding:0px 0px">
<div class="pl">
<div class="tx tx2"><a href="http://www.jq22.com/mem792516"><img src="//www.jq22.com/tx/54.png"></a></div>
<ul class="plbg plbg2">
<div class="f"> yuebanzhou<span class="jl">0</span></div>
<div class="r"> <span class="z12">2018/5/14 15:27:40</span></div>
<div class="dr"></div>
</ul>
<ul style="padding-bottom: 5px;word-wrap: break-word;width: 100%">
参照我发布的另一个例子，全选和全不选，做出复选框的基本效果。点击删除按钮的时候，做一个检测，如果全选按钮是选中状态，直接清空表格内容。<br>
</ul>
</div>
</ul>
<a class="hf" name="958">回复</a>
<div class="lyhf"></div>
<div class="dr"></div>
</ul>
</div>
<div class="pl">
<div class="tx"><a href="http://www.jq22.com/mem827914"><img src="//www.jq22.com/tx/31.png"></a></div>
<ul class="plbg">
<div class="f"> Felix<span class="jl">0</span></div>
<div class="r"> <span class="z12">2018/5/14 15:19:40</span></div>
<div class="dr"></div>
</ul>
<ul style="word-wrap: break-word;width: 100%;padding-top:5px">
可以做一些批量删除的<br>
<ul style="padding:0px 0px">
<div class="pl">
<div class="tx tx2"><a href="http://www.jq22.com/mem792516"><img src="//www.jq22.com/tx/54.png"></a></div>
<ul class="plbg plbg2">
<div class="f"> yuebanzhou<span class="jl">0</span></div>
<div class="r"> <span class="z12">2018/5/14 15:23:32</span></div>
<div class="dr"></div>
</ul>
<ul style="padding-bottom: 5px;word-wrap: break-word;width: 100%">
是的，加上复选框，可以实现。谢谢指教。<br>
</ul>
</div>
</ul>
<a class="hf" name="957">回复</a>
<div class="lyhf"></div>
<div class="dr"></div>
</ul>
</div>
<div class="in2" style="border-top: 1px solid #e8e8e8;padding-top:20px;margin-top:20px;background-color:#f7f7f7">
<a name="xpl"></a>
<div id="err" class="alert alert-danger" role="alert" style="display:none"><i class="fa fa-smile-o"></i> 登录后才可以评论</div>
<div id="err2" class="alert alert-warning" role="alert" style="display:none"><i class="fa fa-smile-o"></i> 30秒后在评论吧!</div>
<textarea id='textarea1' style='height:200px; width:100%;min-height: 300px' placeholder="您有什么想法要说的吗？帮助他人、分享技术会获得奖励！"></textarea>
<div class="r top10">
<button onclick="getPlainTxt()" type="button" id="myButton" data-loading-text="Loading..." class="btn btn-primary" autocomplete="off">发表评论</button>
</div>
<div class="dr"></div>
</div>
</ul>
</div>
</div>
</div>
</div>
<div class="huif2">
<ul>
<textarea id='textarea2' style='height:205px; width:100%;' placeholder="您有什么想法要说的吗？帮助他人、分享技术会获得奖励！"></textarea>
<button onclick="hftj()" type="button" class="btn btn-primary top10">回复</button>
<a class="qxhf" onclick="qx()" style="padding-top: 10px;">取消回复</a>
</ul>
</div>
<textarea id="head" style="display: none">
&lt;!doctype html&gt;
&lt;html&gt;
&lt;head&gt;
&lt;meta charset=&quot;utf-8&quot;&gt;
&lt;title&gt;表格内容的增删（原创）-jq22.com&lt;/title&gt;
&lt;script src=&quot;https://libs.baidu.com/jquery/1.11.3/jquery.min.js&quot;&gt;&lt;/script&gt;
&lt;style&gt;
</textarea>
<textarea id="jw" style="display: none">
&lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
</textarea>
<textarea id="jw1" style="display: none">
&lt;script&gt;
</textarea>
<textarea id="jw2" style="display: none">
&lt;/script&gt;
</textarea>
<textarea id="food" style="display: none">
&lt;/body&gt;
&lt;/html&gt;
</textarea>
<script>
        window.onresize = function () {
            if ($(window).width() >= 800) {
                scrollTo(0, 0);
            }
        }
        var k = 0;
        $(".cjms2").mouseover(function () {
            if ($(".cjms2").text().length > 300 && k == 0) {
                $(".dt2,.dt3").stop();
                $(".dt2").animate({ height: '40%' }, 400);
                $(".dt3").animate({ height: '60%' }, 400);
                k = 1;
            }
        });
        $(".dt2,.zuoze").mouseover(function () {
            if (k == 1) {
                $(".dt2,.dt3").stop();
                $(".dt2").animate({ height: '60%' }, 400);
                $(".dt3").animate({ height: '40%' }, 400);
                k = 0;
            }
        });



        function getPlainTxt() {
            if ($('#textarea1').val().length > 5) {
                myButton.disabled = true;
            } else { }
            setTimeout(function () {
                if (k == "n") {
                    $("#err").css("display", "block");
                } else {
                    myLogin($('#textarea1').val())
                }
            }, 1000);
        }
        var a = "4408";
        var k = "n";
        var b = "792516";
        function myLogin(aa) {
            var jhf = aa;
            jhf = jhf.replace(/<(script)[\S\s]*?\1>|style\=".+?"|title\=".+?"|class\=".+?"/gi, "");
            jhf = jhf.replace(/<table((?!>)[\s\S])*>/gi, "<table>");
            jhf = jhf.replace(/<tbody((?!>)[\s\S])*>|<\/tbody((?!>)[\s\S])*>|<pre((?!>)[\s\S])*>|<\/pre((?!>)[\s\S])*>/gi, "");
            jhf = jhf.replace(/<tr((?!>)[\s\S])*>/gi, "<tr>");
            jhf = jhf.replace(/<th((?!>)[\s\S])*>/gi, "<th>");
            jhf = jhf.replace(/<p><br><\/p>|<p><\/p>/gi, "");
            jhf = jhf.replace(/<\/?(textarea)[^>]*>/gi, "");
            var encodeHTML = encodeURIComponent(jhf);
            if (aa.length > 3) {
                var yz = $.ajax({
                    type: 'post',
                    url: '/weblyadd.aspx',
                    data: { wz: a, nr: encodeHTML, zz: b },
                    cache: false,
                    dataType: 'text',
                    success: function (data) {
                        if (data == "y") {
                            window.location.reload();
                        }
                        else if (data == "s") {
                            window.location.href = "sjyz.aspx";
                        }
                        else {
                            $("#err2").css("display", "block");
                            $("#err2").addClass("dou2");
                        }
                    },
                    error: function () { }
                });
            }
        }
        var a = "4408";
        var k = "n";
        $(".hf").click(function () {
            pid = $(this).attr("name");
            //$(".hf").css("padding-bottom", "10px");
            $(".huif2").css({ "display": "block" });
            // $(this).css("padding-bottom", "300px");
        });
        function qx() {
            $(".hf").css("padding-bottom", "10px");
            $(".huif2").css("display", "none");
        }
        function hftj() {
            if (k != "n") {
                var jhf = document.getElementById("textarea2").value;
                jhf = jhf.replace(/<(script)[\S\s]*?\1>|style\=".+?"|title\=".+?"|class\=".+?"/gi, "");
                jhf = jhf.replace(/<table((?!>)[\s\S])*>/gi, "<table>");
                jhf = jhf.replace(/<tbody((?!>)[\s\S])*>|<\/tbody((?!>)[\s\S])*>|<pre((?!>)[\s\S])*>|<\/pre((?!>)[\s\S])*>/gi, "");
                jhf = jhf.replace(/<tr((?!>)[\s\S])*>/gi, "<tr>");
                jhf = jhf.replace(/<th((?!>)[\s\S])*>/gi, "<th>");
                jhf = jhf.replace(/<p><br><\/p>|<p><\/p>/gi, "");
                jhf = jhf.replace(/<\/?(textarea)[^>]*>/gi, "");
                var hfHTML = encodeURIComponent(jhf);
                if (hfHTML.length > 5) {
                    var h = $.ajax({
                        type: 'post',
                        url: '/weblyhf.aspx',
                        data: { yy: pid, nr: hfHTML, ww: a },
                        cache: false,
                        dataType: 'text',
                        success: function (data) {
                            if (data == "y") {
                                window.location.reload();
                            }
                            else if (data == "s") {
                                window.location.href = "sjyz.aspx";
                            }
                            else {
                                $("#err2").css("display", "block");
                                $("#err2").addClass("dou2");
                            }
                        },
                        error: function () { }
                    });
                }
            } else {
                $("#myModal").modal();
            }
        }

        function sc() {
            var yz = $.ajax({
                type: 'post',
                url: '/shou-web.aspx',
                data: { wz: a },
                cache: false,
                dataType: 'text',
                success: function (data) {
                    if (data == "m") {
                        $("#myModal").modal();
                    } else {
                        ycss();
                        window.location.href = window.location;
                        lytjbut.disabled = false;
                    }
                },
                error: function () { }
            });
        }
        function zuozhe() {
            var yz = $.ajax({
                type: 'post',
                url: '/zuozhe.aspx',
                data: { z: b },
                cache: false,
                dataType: 'text',
                success: function (data) {
                    if (data == "m") {
                        $("#myModal").modal();
                    } else {
                        ycss();
                        window.location.href = window.location;
                    }
                },
                error: function () { }
            });
        }

        if ($(".cjms2").text().length < 10) {
            $(".dt3").css("height", "20%");
            $(".dt2").css("height", "75%");
        }

        var k = 0;

        $(".mlztx,.mplgb").click(function () {
            if (k == 0) {
                $(".mlz").fadeIn();
                k = 1;
            } else {
                k = 0;
                $(".mlz").fadeOut();
            }
        });

        function pxfon() {

            var m1 = editor.getValue().length;
            var m2 = editor2.getValue().length;
            var m3 = editor3.getValue().length;
            var max = (m1 > m2 ? m1 : m2) > m3 ? (m1 > m2 ? m1 : m2) : m3;
            if (m1 == max) {
                $(".dz").eq(0).addClass("dq").siblings().removeClass("dq");
                $(".dt1").hide().eq(0).show();
            } else if (m2 == max) {
                $(".dz").eq(1).addClass("dq").siblings().removeClass("dq");
                $(".dt1").hide().eq(1).show();
            } else if (m3 == max) {
                $(".dz").eq(2).addClass("dq").siblings().removeClass("dq");
                $(".dt1").hide().eq(2).show();
            }

        }
        $(document).ready(function () {

            $(".dt1").eq(0).css("display", "block");
            $(".dtab ul").click(function () {
                $(".dz").eq($(this).index()).addClass("dq").siblings().removeClass("dq");
                $(".dt1").hide().eq($(this).index()).show();
            })

            function timedMsg() {
                var t = setTimeout('pxfon()', 500);
            }
            timedMsg();

        });
        function ycss() {
            if (typeof localStorage.yanse == 'undefined') {
                localStorage.yanse = 1;
            } else {
                localStorage.yanse = parseInt(localStorage.yanse) + 1;
            }
        }
        var bb = "1.11.3";
        function Run() {
            var codehtml = editor.getValue();
            var codecss = '<style>' + editor2.getValue() + '</style>';
            var jqbb = '<scr' + 'ipt src=' + 'https://libs.baidu.com/jquery/' + '1.11.3' + '/jquery.min.js' + '></scr' + 'ipt>';
            var codejs = '<scr' + 'ipt>' + editor3.getValue() + '</scr' + 'ipt>';
            var Fy1 = window["\x64\x6f\x63\x75\x6d\x65\x6e\x74"]["\x67\x65\x74\x45\x6c\x65\x6d\x65\x6e\x74\x42\x79\x49\x64"]('\x69\x66')["\x63\x6f\x6e\x74\x65\x6e\x74\x57\x69\x6e\x64\x6f\x77"]["\x64\x6f\x63\x75\x6d\x65\x6e\x74"]; Fy1["\x6f\x70\x65\x6e"](); if (bb["\x6c\x65\x6e\x67\x74\x68"] < 2) { Fy1["\x77\x72\x69\x74\x65"](codecss + codehtml + codejs); } else { Fy1["\x77\x72\x69\x74\x65"](codecss + jqbb + codehtml + codejs); } Fy1["\x63\x6c\x6f\x73\x65"]();
        }
        Run(); var zK1 = 1; var kgda2; $("\x74\x65\x78\x74\x61\x72\x65\x61")["\x62\x69\x6e\x64"]("\x69\x6e\x70\x75\x74 \x70\x72\x6f\x70\x65\x72\x74\x79\x63\x68\x61\x6e\x67\x65", function () { zK1 = 1; clearInterval(kgda2); kgda2 = setInterval(Codeshow, 1000); }); function Codeshow() { zK1++; if (zK1 > 2) { clearInterval(kgda2); zK1 = 1; Run(); } }

        var hh = "\n\n";
        var hh1 = "\n";
        function dmdown() {
            var atxt = $("#head").val() + editor2.getValue() + $("#jw").val() + editor.getValue() + hh + $("#jw1").val() + editor3.getValue() + hh1 + $("#jw2").val() + hh1 + $("#food").val();
            var blob = new Blob([atxt], { type: "text/plain;charset=utf-8" });
            var num = Math.random();
            num = Math.ceil(num * 10000);
            saveAs(blob, "jq22" + num + ".html");
        }
        $(".jl").each(function () {
            if ($(this).text() > 0) {
                $(this).css('display', 'inline-block');
                $(this).html("评论奖励 " + $(this).text() + " jQ币");
            }
        });

        window._bd_share_config = {
            common: {
                bdText: '表格内容的增删（原创）',
                            bdDesc: '对表格内容进行增加删除',
            },
            share: [{
                "bdSize": 24
            }],
        }

    </script>
<style>
        h1, .h1, h2, .h2, h3, .h3 {
            margin-top: 0px;
            margin-bottom: 10px;
        }.ace-twilight .ace_comment {font-style: inherit}
    </style>

<nav class="foot navbar-inverse" style="overflow: hidden;position: fixed;bottom:0px;width:100%;z-index:999">
<ul class="list-inline">
<li class="footer-ss"><a href="copyright.aspx">版权声明</a></li>
<li class="footer-ss"><a href="feedback.aspx">在线反馈</a></li>
<li class="footer-ss"><a href="cooperation.aspx">广告合作</a></li>
<li class="footer-ss"><a href="web-article1">网页技术</a></li>
<li class="footer-ss"><a href="https://www.jq22.com/work-jq22-tool">jq22工具库</a></li>
<li class="footer-ss"><a href="label1">jquery插件</a></li>
<li style="float:left">2012-2019 jQuery插件库版权所有. 备案号:<a href="http://www.miitbeian.gov.cn/" target="_blank" rel="nofollow">沪ICP备13043785号-1</a> <a target="_blank" href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=33041102000314" style="display:inline-block;text-decoration:none;height:20px;line-height:20px;"><img src="img/batb.png" style="float:left;padding-top: 3px;" /><p style="float:left;height:20px;line-height:20px;margin: 4px 0px 0px 5px; color:#939393;">浙公网安备 33041102000314号</p></a></li>
</ul>
<ul class="list-inline text-right">
<li>
</li>
</ul>
</nav>
<script>
    var _hmt = _hmt || [];
    (function () {
        var hm = document.createElement("script");
        hm.src = "//hm.baidu.com/hm.js?b3a3fc356d0af38b811a0ef8d50716b8";
        var s = document.getElementsByTagName("script")[0];
        s.parentNode.insertBefore(hm, s);
    })();
    (function(){
        var bp = document.createElement('script');
        var curProtocol = window.location.protocol.split(':')[0];
        if (curProtocol === 'https') {
            bp.src = 'https://zz.bdstatic.com/linksubmit/push.js';
        }
        else {
            bp.src = 'http://push.zhanzhang.baidu.com/push.js';
        }
        var s = document.getElementsByTagName("script")[0];
        s.parentNode.insertBefore(bp, s);
    })();
</script>
<style>@media screen and (max-width:930px){.nggys {display: none}}</style>

</body>
</html>
