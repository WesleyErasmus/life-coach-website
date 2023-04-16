<template>
    <!-- Main content -->
    <v-card class="hero-banner" color="primary">
        <v-container>
            <v-card class="hero-card bg-transparent" variant="default">
                <div class="d-flex justify-center align-items-center">
                    <v-card-item class="card-text-container text-white flex-grow-1">
                        <div class="text-h4 mb-4 font-weight-bold">
                            Let's get to work
                        </div>
                        <div class="text-white text-subtitle-1">
                            Unlock Your Full Potential with Strategic Life Coaching. Contact Us Today to Schedule a Session
                            and Start Your Transformation.
                        </div>
                    </v-card-item>
                    <v-card-actions>
                        <v-btn class="rounded-pill px-8 py-2" variant="elevated" size="large">Get In
                            Touch</v-btn>
                    </v-card-actions>
                </div>
            </v-card>
        </v-container>
    </v-card>
</template>

<script>
export default {
    data() {
        return {};
    },
};
</script>

<style scoped>
.hero-banner {
    /* background: var(--primary-gradient-bg); */
    /* Fallback for older browsers */
    /* background: -webkit-linear-gradient(to right, #0074D9, #4DC0B5);
    background: -moz-linear-gradient(to right, #0074D9, #4DC0B5);
    background: -o-linear-gradient(to right, #0074D9, #4DC0B5);
    background-size: cover; */
    padding: 2rem 0;
}

.hero-card {
    /* display: flex;
    justify-content: center;
    align-items: center; */
}

.card-text-container {
    max-width: 80%;
}
</style>
