<template>
    <div class="html-content">
        <div class="work__header flex flex-wrap items-center">
            <div class="work__hero w-1/2">
                <div class="page-title">
                    <div class="html-code indent-3">&#60;h1&#62;</div>  
                    <h1 class="indent-4 color-primary">
                        Work   
                    </h1>
                    <div class="html-code indent-3">&#60;/h1&#62;</div>  
                </div>
                <div class="page-content">
                    <div class="html-code indent-3">&#60;p&#62;</div>  
                    <div class="indent-4">
                        Here are some of the projects that I'm part with:
                    </div>
                    <div class="html-code indent-3">&#60;/p&#62;</div>  
                </div> 
            </div> 
            <div class="work__featured w-1/2">
                <PortfolioCard :key="0" :data="0" :classname="'featured'"/>
            </div>
        </div>    
        <div class="work__archive flex flex-wrap">
            <PortfolioCard v-for="i in 12" :key="i" :data="i" />
        </div>   
    </div> 
</template>

<script>
export default {
    name: 'WorkPage'
}
</script>
