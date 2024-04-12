<script>
export default {
    data() {
        return {
        }
    },
    props: {
        item: Object,

    }
}
</script>

<template>
    <main class="page-content">
        <section class="section">
            <div class="container">
                <div class="row">
                    <div v-for="product in item" class="col-4 ">
                        <div class="card-product">
                            <div class="card-header">
                                <img :src="product.backImage " alt="">
                                <div  class="badge-red">-50%</div>
                                 <span class="badge-green">Sostenibilità</span> 
                                <div class="badge-heart">&hearts;</div>
                                <div class="overlay">
                                    <a class="btn" href="#">Comprami</a>
                                </div>
                            </div>
                            <div class="card-body">
                                <div>{{product.brand}}</div>
                                <h3>RELAXED FIT TEE UNISEX</h3>
                                <div>{{product.price}}&euro;</div>
                                <span class="last-price">29.99 &euro;</span>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>
    </main>


</template>



<style lang="scss" scoped>
@use '../style/partials/mixin' as *;


.card-header{
    position: relative ;
    /* border: 2px solid black; */
}
.card-header > img{
display: block;
}
.badge-red{
    position: absolute;
    bottom: 60px;
    width: 15%;
    background-color: red;
    color: white;
    line-height: 20px;
	font-size: 10px;
	padding: 0 12px;
}
.badge-green{
    position: absolute;
    bottom: 60px;
    left: 50px;
    background-color: green;
    color: white;
    line-height: 20px;
	font-size: 10px;
	padding: 0 12px;
}
.badge-green-solo{
    position: absolute;
    bottom: 60px;
    background-color: green;
    color: white;
    line-height: 20px;
	font-size: 10px;
	padding: 0 12px;
}
.badge-heart{
    background-color: white;
    position: absolute;
    right: 0;
    top: 20px;
    padding: 10px 10px;
}

h3 + div{
    color: orangered;
    display: inline-block;
}
.last-price{
    text-decoration: line-through;
}

.col-4 .overlay{
    @include overlay-mixin;
    background-image: url('/1.webp');
    
 
} 
.col-4-2 .overlay{
    
    background-image: url('/2.webp');
    @include overlay-mixin;

}  
.col-4-3 .overlay{

    @include overlay-mixin;
    background-image: url('/3.webp');
   
}  
.col-4-4 .overlay{
   
    @include overlay-mixin;
	background-image: url('/4.webp');
  
}  
.col-4-5 .overlay{

    @include overlay-mixin;
	background-image: url('/5.webp');
   
}  
.col-4-6 .overlay{
    @include overlay-mixin;
	background-image: url('/6.webp');
   
}  
.col-4:hover .overlay{
    opacity: 1;
}
 .col-4-2:hover .overlay {
 	opacity: 1;
   
 }
 .col-4-3:hover .overlay {
 	opacity: 1;
   
    
   
 }
 .col-4-4:hover .overlay {
 	opacity: 1;
   
 }
 .col-4-5:hover .overlay {
 	opacity: 1;
   
}
 .col-4-6:hover .overlay {
 	opacity: 1;
   
 }
</style>