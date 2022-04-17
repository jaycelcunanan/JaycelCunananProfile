<template>
    <div class="html-content">
        <div class="about__content">
            <div class="about__content-item">
                <div class="page-title">
                    <div class="html-code indent-3">&#60;h1&#62;</div>  
                    <h1 class="indent-4 color-primary">
                    Contact me!
                    </h1>
                    <div class="html-code indent-3">&#60;/h1&#62;</div>  
                </div>
                <div class="page-content">
                    <div class="html-code indent-3">&#60;h2&#62;</div>  
                    <div class="indent-4">
                        <p>
                            I’m interested in freelance opportunities - especially ambitious or large projects. However, if you have other request or question, don’t hesitate to used the form.
                        </p>
                    </div>
                    <div class="html-code indent-3">&#60;/h2&#62;</div>  
                </div>
                <div class="page-form">
                    <div class="html-code indent-3">&#60;form&#62;</div>  
                    <form class="contact__form indent-4">
                        <div class="form-item">
                            <input type="text" class="input-control" placeholder="Name" name="name" required>
                        </div>
                        <div class="form-item">
                            <input type="text" class="input-control" placeholder="Email" name="email" required>
                        </div>
                        <div class="form-item w-100">
                            <input type="text" class="input-control" placeholder="Subject" name="email">
                        </div>
                        <div class="form-item w-100">
                            <textarea class="input-control contact__form-message" name="message" placeholder="Message"></textarea>
                        </div>
                        <div class="form-item w-100 contact__form-submit">
                           <button type="submit" class="btn btn-primary btn-outline">Contact me!</button>  
                        </div>
                    </form>    
                    <div class="html-code indent-3">&#60;/form&#62;</div>  
                </div>   
            </div>  
            <div class="about__content-item">
                
            </div>  
        </div> 
    </div> 
</template>

<script>
export default {
    name: 'ContactPage'
}
</script>
