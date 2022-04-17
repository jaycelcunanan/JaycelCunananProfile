<template>
  <div class="main">
        <client-only placeholder="Loading...">
            <MainNavigation/>
            <div class="main-content">
                <div class="main-content__inner">
                    <div class="html-header">
                        <div class="html-code indent-1">&#60;html&#62;</div>   
                        <div class="html-code indent-2">&#60;body&#62;</div>   
                    </div> 
                    <Nuxt />
                    <div class="html-footer">
                        <div class="html-code indent-2">&#60;/body&#62;</div>   
                        <div class="html-code indent-1">&#60;/html&#62;</div>   
                    </div> 
                </div>
            </div>  
        </client-only>  
    </div>
</template>

<script>
export default {

}
</script>

<style>
</style>