<script>
import Card from './Card.vue'

export default{
  data(){
    return{

      message:'Hello!',
      products: [
    {
      id: 1,
      frontImage: "1.webp",
      backImage: "1b.webp",
      brand: "Levi's",
      name: "Relaxed Fit",
      price: 29.99,
      isInFavorites: true,
      badges: [
        {
          type: "tag",
          value: "Sostenibilità"
        },
        {
          type: "discount",
          value: "-50%"
        }
      ]
    },
    {
      id: 2,
      frontImage: "2.webp",
      backImage: "2b.webp",
      brand: "Guess",
      name: "Roses Tee",
      price: 20.99,
      isInFavorites: true,
      badges: [
        {
          type: "discount",
          value: "-30%"
        }
      ]
    },
    {
      id: 3,
      frontImage: "3.webp",
      backImage: "3b.webp",
      brand: "Come Zucchero Filato",
      name: "Voglia di colori pastello",
      price: 129.99,
      isInFavorites: false,
      badges: [
        {
          type: "discount",
          value: "-30%"
        }
      ]
    },
    {
      id: 4,
      frontImage: "4.webp",
      backImage: "4b.webp",
      brand: "Levi's",
      name: "Tee Unisex",
      price: 14.99,
      isInFavorites: false,
      badges: [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      id: 5,
      frontImage: "5.webp",
      backImage: "5b.webp",
      brand: "Maya Deluxe",
      name: "Stripe Bodice",
      price: 99.99,
      isInFavorites: true,
      badges: [
        {
          type: "tag",
          value: "Sostenibilità"
        },
        {
          type: "discount",
          value: "-50%"
        }
      ]
    },
    {
      id: 6,
      frontImage: "6.webp",
      backImage: "6b.webp",
      brand: "Esprit",
      name: "Maglione - Black",
      price: 29.99,
      isInFavorites: true,
      badges: [
        {
          type: "tag",
          value: "Sostenibilità"
        }
      ]
    }
        ]
    }
  },
  components:{
        Card
    },  
}

</script>

<template>
  <Card :item="products"/>
 


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
    background-image: url('../../public/1.webp');
    
 
} 
.col-4-2 .overlay{
    
    background-image: url('../../public/2.webp');
    @include overlay-mixin;

}  
.col-4-3 .overlay{

    @include overlay-mixin;
    background-image: url('../../public/3.webp');
   
}  
.col-4-4 .overlay{
   
    @include overlay-mixin;
	background-image: url('../../public/4.webp');
  
}  
.col-4-5 .overlay{

    @include overlay-mixin;
	background-image: url('../../public/5.webp');
   
}  
.col-4-6 .overlay{
    @include overlay-mixin;
	background-image: url('../../public/6.webp');
   
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