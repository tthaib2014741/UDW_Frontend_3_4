<template>

    <div  class="page">
        <h4>Thêm Liên hệ</h4>
        <ContactForm :contact="contact" @submit:contact="addContact"  />
        <p>{{ message }}</p>
    </div>
</template> 

<script>
    import ContactForm from "@/components/ContactForm.vue";
    import ContactService from "@/services/contact.service";
    export default {
        components: {
            ContactForm,
        },
        props: {
            id: {
                type: String,
                
            },
        },
        data() {
            return {
                contact: null,
                message: "",
            };
        },
        methods: {
           
            async addContact(data) {
                try {
                    await ContactService.create(data);
                  
                    console.log(data);
                    this.message = "Liên hệ được thêm thành công.";
                } catch (error) {
                    console.log(error);
                }
            },
            
        },
       
    };
</script>


