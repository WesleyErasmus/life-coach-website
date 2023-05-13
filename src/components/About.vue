<template>
    <!-- Main content -->
    <v-container class="pt-15 pb-10">
        <v-container fluid>
            <div class="text-h4 text-center text-primary font-weight-bold">
                <div class="mb-2">How Strategic Coaching Works</div>
                <p class="text-medium-emphasis text-subtitle-1 pa-0 ma-0">
                    SLC will empower you in your journey of continuous self-improvement.
                </p>
            </div>
            <v-row class="gif-and-content-container">
                <!-- Section GIF -->
                <v-col class="gif-container d-flex justify-start" md="6">
                    <img class="about-gif rounded-circle" src="../assets/learning-2.gif" alt="Coaching-Asset">
                </v-col>
                <!-- Section Content -->
                <v-col class="col-container-content d-flex justify-center" md="6">
                    <v-card class="about-card" variant="default">
                        <v-card-item>
                            <div class="text-h5 text-primary mb-4 text-medium-emphasis">
                                Empowering You with the Tools for Personal Transformation
                            </div>
                            <p class="font-weight-medium text-medium-emphasis text-body-2 mb-4 pl-1">
                                SLC empowers individuals in their journey of continuous self-improvement through
                                personalized assessments, actionable insights, and tracking tools. With our user-friendly
                                platform, individuals can gain self-awareness, set meaningful goals, and take tangible steps
                                towards personal growth, career advancement, and wellness. Unlock your full potential for
                                continuous improvement with our empowering service.
                            </p>
                            <p class="font-weight-medium text-medium-emphasis text-body-2 mb-0 pl-1">
                                With our user-friendly platform, individuals can gain self-awareness, set meaningful goals,
                                and take tangible steps towards personal growth, career advancement, and wellness. Unlock
                                your full potential for continuous improvement with our empowering service.
                            </p>
                        </v-card-item>
                        <v-card-actions class="card-btn-container">
                            <v-btn class="ml-2 rounded-pill px-8 py-2" variant="elevated" color="primary" size="large">Read
                                More</v-btn>
                        </v-card-actions>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
    </v-container>
</template>

<style scoped>
.about-card {
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-content: start;
    margin-top: 4rem;
}

.about-gif {
    max-width: 90%;
}

@media (max-width: 1280px) {
    .about-gif {
        max-width: 100%;
        min-width: 420px;
    }
/* }

@media (max-width: 965px) { */
    .about-card {
        min-width: 350px;
    }
    .gif-and-content-container {
        justify-content: center;
    }
    .about-gif {
        min-width: 350px;
    }
    .gif-container {
        justify-content: center;
        text-align: center;
    }
/* } */

/* @media (max-width: 857px) { */
    .about-card {
        margin-top: 4rem;
        margin-bottom: 4rem;
        text-align: center;
    }

    .v-card-actions {
        justify-content: center;
    }

     .about-gif {
        width: 50%;
        min-width: 310px;
    }
    .gif-container {
        align-items: center;
        justify-content: center !important;
        
    }
/* } */

/* @media only screen and (max-width: 787px) { */
    .col-container-content {
        padding-top: 0;
    }
    .about-card {
        margin-top: 4rem;
    }
}

@media only screen and (max-width: 500px) {
    .about-card {
        margin: 0 15px;
    }
}</style>