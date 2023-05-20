<template>
    <v-footer class="text-center d-flex flex-column bg-grey-lighten-4">
        <v-container>
            <!-- <div>
                <v-btn v-for="icon in icons" :key="icon" class="mx-4" :icon="icon" variant="text"></v-btn>
            </div> -->
            <div class="pt-4">
                <div class="text-body-1">Email: <span class="text-primary"><a href="mailto:daryl@ontrackcoaching.co.za?subject=Online Coaching Enquiry"
                    class="text-decoration-none text-primary"
                    >daryl@ontrackcoaching.co.za</a></span></div>
                <div class="text-body-1">Phone: <span class="text-primary">
                    (123) 456-7890
                </span></div>
                 <div class="text-body-1">WhatsApp: <span class="text-primary">
                        <a href="https://wa.me/+27784046511" target="_blank"
                        class="text-decoration-none text-primary">(123) 456-7890</a>
                    </span></div>
            </div>
        </v-container>
        <v-divider></v-divider>

        <div class="copyright">
            &copy; {{ new Date().getFullYear() }} — <strong class="text-primary">The Bright Web.</strong> All rights
            reserved.
        </div>

    </v-footer>
</template>
<script>
export default {
    data: () => ({
        // icons: [
        //     'mdi-facebook',
        //     'mdi-twitter',
        //     'mdi-linkedin',
        //     'mdi-instagram',
        // ],
    }),
}
</script>
<style scoped>
.copyright {
    margin: 0;
    padding: 2rem 0;
    width: 100%;
}
</style>