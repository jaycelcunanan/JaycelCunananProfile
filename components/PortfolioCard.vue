<template>
    <div class="portfolio-card" :class="classname">
        <div class="portfolio-card__image">
            <img src="https://mattfarley.ca/img/projects/wfdesignbuild.png" />
        </div>
        <div class="portolio-card__details flex items-center justify-center">
            <div class="portolio-card__details--inner">
                <h3 class="text-white font-primary-bold mb-5">High-end, custom residential renovaters serving Fraser Valley homeowners.</h3>
                <a class="btn btn-small btn-border text-white hover-primary font-primary-bold" href="#" target="_blank">Visit Website</a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'PortfolioCard',
    props: ['data', 'id', 'classname'],
}
</script>

<style scoped>
    .portfolio-card {
        width: calc(33.33% - 30px);
        margin: 15px;
        height: 300px;
        overflow: hidden;
        position: relative;
    }
    .portfolio-card__image,
    .portolio-card__details {
        position: absolute;
        left: 0px;
        top: 0px;
        width: 100%;
        height: 100%;
        z-index: 1;
    }
    .portfolio-card__image>img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: all ease 0.2s;
    }
    .portolio-card__details {
        z-index: 10;
        text-align: center;
        padding: 30px;
        font-size: 22px;
        line-height: 26px;
        background-color: #04c2c9;
        visibility: hidden;
        opacity: 0;
        transition: opacity ease 0.5s, visibility ease 0.5s;
    }
    .portolio-card__details a {
        border-radius: 50px;
        padding: 3px 20px;
    }
    .portfolio-card:hover .portolio-card__details {
        visibility: visible;
        opacity: 1;
        /* display: none; */
    }
    .portfolio-card:hover .portfolio-card__image>img {
        transform: scale(1.1);
    }

    @media screen and (max-width: 1023px) {
       .portfolio-card {
           width: calc(50% - 20px);
           margin: 10px;
       }
    }

    @media screen and (max-width: 767px) {
       .portfolio-card {
           width: 100%;
           margin: 10px 0px;
       }
    }
</style>