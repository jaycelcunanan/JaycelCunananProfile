<template>
    <header class="navigation">
        <div id="logo" class="logo">
            <div class="logo__img">JMC</div>
            <div class="logo__name">Jaycel Cunanan</div>    
            <div class="logo__position">Web Developer</div>
            <a href="/" class="link-overlay"></a>
        </div>  
        <div class="navigation__links">
            <div class="navigation__links-toggle">
                <div class="burger-menu" :class="{'active': menu.isActive}" @click="toggleMenu()">
                    <div class="bar1"></div>
                    <div class="bar2"></div>
                    <div class="bar3"></div>
                </div>
            </div>
            <div class="navigation__links-inner" :class="{'active': menu.isActive}"  @click="toggleMenu()">
                <div class="navigation__links-item">
                    <nuxt-link to="/">Home</nuxt-link> 
                </div>
                <div class="navigation__links-item">
                    <nuxt-link to="/about">About</nuxt-link> 
                </div>
                <div class="navigation__links-item">
                    <nuxt-link to="/expertise">My Skills</nuxt-link> 
                </div>
                <div class="navigation__links-item">
                    <nuxt-link to="/work">Work</nuxt-link> 
                </div>
                <div class="navigation__links-item">
                    <nuxt-link to="/contact">Contact</nuxt-link> 
                </div>
            </div>  
        </div>  
        <div class="navigation__social"></div>  
    </header>
</template>

<script>
export default {
    name: 'MainNavigation',
    data: function() {
        return {
            menu: {
                isActive: false,
            }
        }
    },
    methods: {
        toggleMenu: function() {
            this.menu.isActive = !this.menu.isActive;
        }
    },
}
</script>