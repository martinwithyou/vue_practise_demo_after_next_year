<template>
  	<div class="border">

        <mt-header 
            fixed 
            title="杭州建筑摄影爱好者" 
            class="title-color">
        </mt-header>

    	<mt-swipe :auto="5000">
            <mt-swipe-item class="poster_a" >1</mt-swipe-item>
            <mt-swipe-item class="poster_b">2</mt-swipe-item>
            <mt-swipe-item class="poster_c">3</mt-swipe-item>
            <mt-swipe-item class="poster_d">4</mt-swipe-item>
            <mt-swipe-item class="poster_e">5</mt-swipe-item>
        </mt-swipe>

        <mt-tab-container  
        class="container"
        v-model="active">
            <mt-tab-container-item id="tab-container1">
                <mt-cell v-for="n in 10" title="tab-container 1"></mt-cell>
            </mt-tab-container-item>
        </mt-tab-container>
  	</div>
</template>




<script>
export default {
	name: 'item',
  	components: {
   		
  	},
  	created(){
     
  	}
}
</script>



<style lang="less">
    .border{
      width:100%;
      height:250px;
      border:0px solid #333333;
    }  
    .poster_a{
      background: url(../../images/09_40_58__12_04_2018.jpg);
      background-size:100% 250px;
    }
    .poster_b{
      background: url(../../images/09_41_31__12_04_2018.jpg);
      background-size:100% 250px;
    }
    .poster_c{
      background: url(../../images/09_42_51__12_04_2018.jpg);
      background-size:100% 250px;
    }
    .poster_d{
      background: url(../../images/09_43_56__12_04_2018.jpg);
      background-size:100% 250px;
    }
    .poster_e{
      background: url(../../images/09_46_20__12_04_2018.jpg);
      background-size:100% 250px;
    }
    .title-color{
        color:#ffffff;
    }
    .container{
        width:100%;
        height:400px;
        border:0px solid #333333;
    }
    .mint-tab-container-item{
        display:block !important;
    }
</style>
