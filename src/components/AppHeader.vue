<script>
export default{
  data(){
    return{
     
    }
  }
}

</script>

<template>
  <header class="page-header">
        <nav class="container">
            <div class="row">
                <div>
                    <ul>
                        <li>Uomo</li>
                        <li>Donna</li>
                        <li>Bambino</li>
                    </ul>
                </div>
                <div class="logo">
                    <img src="/boolean-logo.png" alt="Logo-Boolean">
                </div>
                <div class="menu">
                    <ul>
                        <li>&hearts;</li>
                        <li>&hearts;</li>
                        <li>&hearts;</li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>


</template>


<style lang="scss" scoped>
.page-header{
  height:auto;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  background-color: rgba(255, 69, 0, 0.9);
  box-shadow: 0px 0px 20px 0 rgba(0, 0, 0, 0.3);
  color: white;
  padding: 12px 0;
}
.page-header .row{
  justify-content: space-between;
  align-items: center;
   
}
li{
  display: inline ;
  padding: 0 5px;
    
}
.logo{
  max-width:150px;
  max-height: 22px;
    
}
</style>