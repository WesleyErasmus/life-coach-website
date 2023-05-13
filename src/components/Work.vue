<template>
    <!-- Main content -->
    <v-card class="card-container" color="primary">
        <v-container>
            <v-card class="bg-transparent" variant="default">
                <div class="card-contents-flex-container d-flex justify-space-between align-items-center">
                    <v-card-item class="card-text-container text-white flex-grow-1">
                        <div class="text-h4 mb-4 font-weight-bold">
                            Let's get to work
                        </div>
                        <div class="text-white text-subtitle-1">
                            Unlock Your Full Potential with Strategic Life Coaching. Contact Us Today to Schedule a Session
                            and Start Your Transformation.
                        </div>
                    </v-card-item>
                    <v-card-actions class="contact-btn-container">
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
.card-container {
    padding: 1rem 0;
}

.card-text-container {
    max-width: 70%;
}

@media only screen and (max-width: 767px) {
    .card-text-container {
        max-width: 100%;
    }

    .card-text-container div {
        font-size: 1.5rem;
        line-height: 1.5;
        text-align: center;
    }

    .card-contents-flex-container {
        align-items: center;
        flex-direction: column;
    }

    .contact-btn-container {
        padding-top: 1rem;
    }
}</style>