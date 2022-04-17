<template>
    <div class="html-content">
        <div class="about__content">
            <div class="about__content-item">
                <div class="page-title">
                    <div class="html-code indent-3">&#60;h1&#62;</div>  
                    <h1 class="indent-4 color-primary">
                       Me, Myself & I
                    </h1>
                    <div class="html-code indent-3">&#60;/h1&#62;</div>  
                </div>
                <div class="page-content">
                    <div class="html-code indent-3">&#60;p&#62;</div>  
                    <div class="indent-4">
                        <p>
                            I’m a Front-End Developer located in Poland. I have a serious passion for UI effects, animations and creating intuitive, dynamic user experiences.
                        </p>
                        <p>
                            Well-organised person, problem solver, independent employee with high attention to detail. Fan of MMA, outdoor activities, TV series and English literature. A family person and father of two fractious boys,
                        </p>
                        <p>
                            Interested in the entire frontend spectrum and working on ambitious projects with positive people.
                        </p>
                        <p>
                            <nuxt-link to="/contact" class="color-primary">
                                Let’s make something special.
                            </nuxt-link>
                        </p>
                    </div>
                    <div class="html-code indent-3">&#60;/p&#62;</div>  
                </div>    
            </div>    
            <div class="about__content-item">
                <span class="content"></span>
            </div>    
        </div>
    </div> 
</template>

<script>
export default {
    name: 'AboutPage',
    data: function() {
        return {
            windowWidth: window.outerWidth,
        }
    },

    async mounted() {
        let myTags = [
            'JavaScript', 'CSS', 'SASS', 'HTML',
            'Laravel', 'WordPress', 'PHP',
            'Python', 'jQuery', 'NodeJS', 'VueJS',
            'MySQL','git', 
        ];

        let tagCloud = TagCloud('.content', myTags, {
            // radius in px
            radius: this.windowWidth >= 768 ? 300: 160,

            // animation speed
            // slow, normal, fast
            maxSpeed: 'fast',
            initSpeed: 'fast',

            // 0 = top
            // 90 = left
            // 135 = right-bottom
            direction: 135,

            // interact with cursor move on mouse out
            keep: true
        }); 
    }
}

</script>

<style>
    .tagcloud {  
        font-size: 20px;
        font-weight: 650;
        margin-left: 30%;
        cursor: pointer;
        margin-left: 0;
        width: 100%!important;
    }
    .tagcloud--item {
        color: #08FDD8;
    }
    .tagcloud--item:hover {
        color: #fff;
    }
</style>   
