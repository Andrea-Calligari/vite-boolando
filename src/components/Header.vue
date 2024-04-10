<script>
export default{
  data(){
    return{
      message:'Hello!'
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
                    <img src="../public/boolean-logo.png" alt="Logo-Boolean">
                </div>
                <div class="menu">
                    <ul>
                        <li>img</li>
                        <li>img</li>
                        <li>img</li>
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
</style>