<template>  

    <div class="wrapper">

        <div>
            <h2>Логистические данные:</h2>
        </div>
                <div class="tableheader">
                    <span class="radius"></span>
                <div class="hr"></div>
                    <table class="table">  
                        <tr><th>Вес шт.<br> Брутто, кг</th>
                        <th> Кол-во шт.<br> в упаковке</th>
                        <th> Тип<br> упаковки</th>
                        <th> Вес упаковки<br> Брутто, кг</th>
                        <th colspan="3">Размер упаковки, мм<br>
                     <div class="tableflex">
                        <div>длина</div>
                        <div>ширина</div>
                         <div>высота</div>
                        </div>
                        </th>
                        <th> Объем, м3</th>
                        </tr>
                        <tr><td> {{weight}}</td>
                        <td> {{amountInBox}}</td>
                        <td> {{BoxType}}</td>
                        <td> {{weightBox}}</td>
                        <td>380</td><td style="border: none">255</td><td style="border: none">315</td>
                        <td> {{volumeBox}}</td>
                        </tr>
                    </table> 
                         
                    </div>
                        <div class="content">
                            <div class="content1">
                            <img src='../IMG/box1878.jpg'>
                            
                                <div class="centerinfo">
                                    <div class="kginfo">
                                        <img src="../IMG/Group_1866.svg" alt=""><span>13,77</span>
                                    </div>
                                    <div class="vo">
                                        <span>V=0,03</span>
                                    </div>
                                    <div class="hig">
                                    <span>195&nbsp;мм</span> 
                                 </div>    
                            
                            <div>
                            <div class="len"><span>310 мм</span>
                            </div>
                            <div class="wid">
                                <span>518 мм</span>
                            </div>
                        </div>
                        </div>
                    
                        </div>
                            <div class="content1"> 
                                <div class="boxtwoinfo">
                                <div class="kgtwoinfo">
                                        <img src="../IMG/Group_1866.svg" alt=""><span><b>232</b></span>
                                    </div> 
                                </div> 
                                <div class="boxtitle">
                                    <h3><span>2</span><br>короба</h3>
                                </div>
                                <img src='../IMG/box1877.jpg'>   
                            </div>
                
            
                        </div>
    </div>
</template>



<script>
    
export default {
name: 'App',
data(){
  return{
      weight: '0,277',
      amountInBox: 36,
      BoxType: 'Короб',
      weightBox: 65,
      sizeBox:{
          lengthBox: 380,
          widthBox: 255,
          heightBox: 315 
      },
      volumeBox: '0,3'

  }}

}
</script>

<style>
   
/*Основная часть*/ 
#app{
    display: flex;
    justify-content: center;
    font-family: Arial; 
    color: #404040;
}
h2{
    font-size: 20px;
}
body{
    background-color:#E9E9E9;
}
.wrapper{
    background-color:white;
    width: 900px;
    height: 450px;
    padding: 1% 5%;
    border-radius:15px;
}
/*контент*/ 
.content{
    margin-top: 10%;
    display: flex;
    justify-content: space-between;
    position: relative;
    width: 100%;
}
.content span{
    font-weight: bold;
}
.content1{
    width: 50%;
    display: flex;
    justify-content: center;
}
.centerinfo{
    width: 350px;
    height: 120px;
    position: absolute;

}
.boxtwoinfo{
    width: 350px;
    height: 120px;
    position: absolute;
}
.hig{
    position: absolute;
    top: 50%;
    left: 85%;
}
.vo{
    position: absolute;
    top: 50%;
    left: 55%;
    font-size: 14px;
}
.len{
    position: absolute;
    top: 100%;
    left: 15%; 
}
.wid{
    position: absolute;
    top: 100%;
    left: 75%; 
}
.boxtitle{
    position: absolute;
    text-align: center;
    font-size: 14px;
    bottom:85%;
    font-weight: normal;
}
.boxtitle span{
    font-size: 24px;
}
.kginfo{
    display: flex;
    width: 35px;
    position: absolute;
    left: 30%;
    top: 50%;
    font-size: 14px;
    align-items: flex-end;

} 
.kginfo span{
    margin-left: 2px;
}
.kgtwoinfo{
    display: flex;
    width: 35px;
    position: absolute;
    left: 41%;
    top: 40%;
    background-color:white;
    opacity: 100;
    z-index: 3;
    align-items: center;
    align-items: flex-end;
}
.kgtwoinfo span{
    margin-left: 5px;
}
/*таблица*/ 
.radius{
    width: 100%;
    height: 63px;
    background-color:#C4C4C4;
    border-radius: 15px;
    Opacity: 7%;   
    display: block;
    position: absolute;   
}
.tableheader{
    width: 100%; 
    height: 20%;
    position: relative;
}
.table{
    width: 100%;  
    text-align: center;
    line-height:20px;
    border-spacing: 0 15px;   
}
.hr{
    border-bottom: 1px solid #C4C4C4;
    width: 900px;
    position: absolute;
    top: 63px;
}


.table th:not(:nth-child(1)){
    border-left: 1px solid #E9E9E9 ;
}
.table td:not(:nth-child(1)){
    border-left: 1px solid #E9E9E9 ;
}
.tableflex{
    display: flex;
    justify-content: space-around;
    width: 100%;
    font-size: 15px;
    color:#9B9B9B;
    line-height:17.25px;
}
.table tr{
height: 40px;
}
table th
{
    font-style: Regular;
    font-weight: 400;
    font-size: 16px;
    line-height:18.4px;
    
}
table td
{
    font-weight: 100;
    font-size: 15px;
    font-style: Regular;
}
.three:not(:nth-child(1)){
    display: inline-block;
    padding-left: 20px;
}
.three:first-child{
    padding-right: 40px;
}
hr{
    width: 900px;
}


</style>