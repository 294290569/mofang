##用css3做的一个动画魔方

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>无标题文档</title>
<style>
.box{
	perspective:1000px;}
.box1{
	width:500px;
	height:500px;
	margin:100px auto;
	position:relative;
	transform-style:preserve-3d;
	transition:all 50s linear;
	}
.box1:hover{
	transform:rotateX(3600deg) rotateY(3600deg);}
				
.a1,.a2,.a3,.a4,.a5,.a6{
			  width:200px;
			  height:200px;
			  position:absolute;
			  top:100px;
			  left:100px;
			  opacity: .5;
			  text-align:center;
	          line-height:200px;}
			  
			  
			  /*第一面魔方所有元素*/
.q1,.q2,.q3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.qa1,.qa2,.qa3,.qb1,.qb2,.qb3,.qc1,.qc2,.qc3{
	width:60px;
	height:60px;
	background-color:#09F;
	border:1px solid #666;}
	
.qa1,.qb1,qc1{
	position:absolute;
	top:0;
	left:0;}	
.qa2,.qb2,.qc2{
	position:absolute;
	top:0;
	left:65px;}
.qa3,.qb3,.qc3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.q1{
	position:absolute;
	top:5px;
	left:5px;}	
.q2{
	position:absolute;
	top:70px;
	left:5px;}	
.q3{
	position:absolute;
	top:135px;
	left:5px;}	
	
	/*第二面魔方元素*/
	
.w1,.w2,.w3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.wa1,.wa2,.wa3,.wb1,.wb2,.wb3,.wc1,.wc2,.wc3{
	width:60px;
	height:60px;
	background-color:#F0C;
	border:1px solid #666;}
	
.wa1,.wb1,wc1{
	position:absolute;
	top:0;
	left:0;}	
.wa2,.wb2,.wc2{
	position:absolute;
	top:0;
	left:65px;}
.wa3,.wb3,.wc3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.w1{
	position:absolute;
	top:5px;
	left:5px;}	
.w2{
	position:absolute;
	top:70px;
	left:5px;}	
.w3{
	position:absolute;
	top:135px;
	left:5px;}		
	
	
	/*第三面魔方*/
	
.e1,.e2,.e3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.ea1,.ea2,.ea3,.eb1,.eb2,.eb3,.ec1,.ec2,.ec3{
	width:60px;
	height:60px;
	background-color:#60C;
	border:1px solid #666;}
	
.ea1,.eb1,ec1{
	position:absolute;
	top:0;
	left:0;}	
.ea2,.eb2,.ec2{
	position:absolute;
	top:0;
	left:65px;}
.ea3,.eb3,.ec3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.e1{
	position:absolute;
	top:5px;
	left:5px;}	
.e2{
	position:absolute;
	top:70px;
	left:5px;}	
.e3{
	position:absolute;
	top:135px;
	left:5px;}		
	
     /*第四面魔方颜色*/
	 	
.r1,.r2,.r3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.ra1,.ra2,.ra3,.rb1,.rb2,.rb3,.rc1,.rc2,.rc3{
	width:60px;
	height:60px;
	background-color:#0F3;
	border:2px solid #666;}
	
.ra1,.rb1,rc1{
	position:absolute;
	top:0;
	left:0;}	
.ra2,.rb2,.rc2{
	position:absolute;
	top:0;
	left:65px;}
.ra3,.rb3,.rc3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.r1{
	position:absolute;
	top:5px;
	left:5px;}	
.r2{
	position:absolute;
	top:70px;
	left:5px;}	
.r3{
	position:absolute;
	top:135px;
	left:5px;}	
	
	/*第五块魔方面*/	
.t1,.t2,.t3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.ta1,.ta2,.ta3,.tb1,.tb2,.tb3,.tc1,.tc2,.tc3{
	width:60px;
	height:60px;
	background-color:#FF6;
	border:2px solid #666;}
	
.ta1,.tb1,tc1{
	position:absolute;
	top:0;
	left:0;}	
.ta2,.tb2,.tc2{
	position:absolute;
	top:0;
	left:65px;}
.ta3,.tb3,.tc3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.t1{
	position:absolute;
	top:5px;
	left:5px;}	
.t2{
	position:absolute;
	top:70px;
	left:5px;}	
.t3{
	position:absolute;
	top:135px;
	left:5px;}	



      /*第六块魔方面*/	
	
.u1,.u2,.u3{
	width:190px;
	height:60px;
	position:absolute;	
	}
.ua1,.ua2,.ua3,.ub1,.ub2,.ub3,.uc1,.uc2,.uc3{
	width:60px;
	height:60px;
	background-color:#630;
	border:2px solid #666;}
	
.ua1,.ub1,uc1{
	position:absolute;
	top:0;
	left:0;}	
.ua2,.ub2,.uc2{
	position:absolute;
	top:0;
	left:65px;}
.ua3,.ub3,.uc3{
	position:absolute;
	top:0;
	left:130px;}
				
		
.u1{
	position:absolute;
	top:5px;
	left:5px;}	
.u2{
	position:absolute;
	top:70px;
	left:5px;}	
.u3{
	position:absolute;
	top:135px;
	left:5px;}		
	
	/***********************************/					  
.a1{
	transform: translateZ(100px);}
.a2{
	background-color:#09F;
	transform: translateZ(-100px);}
.a3{
	background-color:#9C0;
	transform: rotateX(90deg) translateZ(100px);}
.a4{
	background-color:#63F;
	transform: rotateX(-90deg) translateZ(100px);}
.a5{
	background-color:#F39;
	transform: rotateY(90deg) translateZ(100px);}
.a6{
	background-color:#9FF;
	transform: rotateY(-90deg) translateZ(100px);}					
				  
	
</style>
</head>

<body>
<div class="box">
        <div  class="box1">
                 <div class="a1">
                           <div class="q1">
                                   <div class="qa1"></div>
                                   <div class="qa2"></div>
                                   <div class="qa3"></div>
                           </div>
                           <div class="q2">
                                   <div class="qb1"></div>
                                   <div class="qb2"></div>
                                   <div class="qb3"></div>
                                   
                           </div>
                           <div class="q3">
                                   <div class="qc1"></div>
                                   <div class="qc2"></div>
                                   <div class="qc3"></div>
                           </div>
                 </div>
                 <div class="a2">
                             <div class="w1">
                                   <div class="wa1"></div>
                                   <div class="wa2"></div>
                                   <div class="wa3"></div>
                           </div>
                           <div class="w2">
                                   <div class="wb1"></div>
                                   <div class="wb2"></div>
                                   <div class="wb3"></div>
                                   
                           </div>
                           <div class="w3">
                                   <div class="wc1"></div>
                                   <div class="wc2"></div>
                                   <div class="wc3"></div>
                           </div>
                 </div>
                 <div class="a3">
                             <div class="e1">
                                   <div class="ea1"></div>
                                   <div class="ea2"></div>
                                   <div class="ea3"></div>
                           </div>
                           <div class="e2">
                                   <div class="eb1"></div>
                                   <div class="eb2"></div>
                                   <div class="eb3"></div>
                                   
                           </div>
                           <div class="e3">
                                   <div class="ec1"></div>
                                   <div class="ec2"></div>
                                   <div class="ec3"></div>
                           </div>
                 </div>
                 <div class="a4">
                             <div class="r1">
                                   <div class="ra1"></div>
                                   <div class="ra2"></div>
                                   <div class="ra3"></div>
                           </div>
                           <div class="r2">
                                   <div class="rb1"></div>
                                   <div class="rb2"></div>
                                   <div class="rb3"></div>
                                   
                           </div>
                           <div class="r3">
                                   <div class="rc1"></div>
                                   <div class="rc2"></div>
                                   <div class="rc3"></div>
                           </div>
                 </div>
                 <div class="a5">
                           <div class="t1">
                                   <div class="ta1"></div>
                                   <div class="ta2"></div>
                                   <div class="ta3"></div>
                           </div>
                           <div class="t2">
                                   <div class="tb1"></div>
                                   <div class="tb2"></div>
                                   <div class="tb3"></div>
                                   
                           </div>
                           <div class="t3">
                                   <div class="tc1"></div>
                                   <div class="tc2"></div>
                                   <div class="tc3"></div>
                           </div>
                 </div>
                 <div class="a6">
                            <div class="u1">
                                   <div class="ua1"></div>
                                   <div class="ua2"></div>
                                   <div class="ua3"></div>
                           </div>
                           <div class="u2">
                                   <div class="ub1"></div>
                                   <div class="ub2"></div>
                                   <div class="ub3"></div>
                                   
                           </div>
                           <div class="u3">
                                   <div class="uc1"></div>
                                   <div class="uc2"></div>
                                   <div class="uc3"></div>
                           </div>
                 </div>
        </div>
</div>
</body>
</html>
