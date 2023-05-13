<template>
    <!-- Main content -->
    <div class="hero-banner" fluid>
        <v-container>
            <v-row class="hero-content-flex-container">
                <v-col class="d-flex justify-center" md="6">
                    <v-card class="hero-card bg-transparent" variant="none">
                        <v-card-item class="text-white">
                            <div class="text-h3 mb-2 font-weight-bold">
                                ON TRACK
                            </div>
                            <div class="text-h6 mb-4 pl-1">Strategic Coaching with Darryl Henning</div>
                            <p class="text-body-1 mb-4 pl-1">
                                Strategic coaching will allow you to pause and take stock at whatever aspect of your life
                                journey you may find yourself on. A variety of tools and techniques will aid you to explore
                                whilst at the same time offer you the practical help required. The resetting of goals and
                                priorities could be one of job search, purpose, career, spirituality, relationships or
                                trauma.
                            </p>
                        </v-card-item>
                        <v-card-actions class="hero-btn-container">
                            <v-btn append-icon="mdi-chevron-down" class="ml-2 rounded-pill px-8 py-2" variant="elevated" color="primary"
                                size="x-large"
                                >Go to Services</v-btn>
                        </v-card-actions>
                    </v-card>
                </v-col>
                <v-col class="d-flex justify-end" md="6">
                    <img class="coaching-gif elevation-0 rounded-circle ma-8" src="../assets/career-coaching.gif"
                        alt="Coaching-Asset">
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    data() {
        return {
        };
    },
};
</script>

<style scoped>
.hero-banner {
    background: var(--primary-gradient-bg);
    /* Fallback for older browsers */
    background: -webkit-linear-gradient(to right, #0074D9, #4DC0B5);
    background: -moz-linear-gradient(to right, #0074D9, #4DC0B5);
    background: -o-linear-gradient(to right, #0074D9, #4DC0B5);
    background-size: cover;
    padding: 5rem 0;
}

.hero-card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
}

.coaching-gif {
    max-width: 70%;
}


@media (max-width: 855px) {
    .coaching-gif {
        max-width: 100%;
        width: 280px;
        height: 280px;
    }
}

@media (max-width: 736px) {
    .hero-content-flex-container {
        display: block;
        text-align: center;
    }

    .coaching-gif {
        display: none;
    }

    .hero-btn-container {
        margin: 0 auto;
    }
}</style>
