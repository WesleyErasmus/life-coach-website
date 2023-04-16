<template>
    <!-- Main content -->
    <v-container fluid class="about-section">
        <v-container>
            <div class="text-h4 text-center text-primary font-weight-bold">
                <div class="mb-2">How Strategic Coaching Works</div>
                <p class="text-medium-emphasis text-subtitle-1 pa-0 ma-0">
                    SLC will empower you in your journey of continuous self-improvement.
                </p>
            </div>
            <v-row>
                <v-col class="d-flex justify-start" md="6">
                    <!-- Section GIF -->
                    <img class="coaching-gif rounded-circle" src="../assets/learning-2.gif" alt="Coaching-Asset">
                </v-col>
                <v-col class="d-flex justify-center" md="6">
                    <v-card class="about-card" variant="none">
                        <v-card-item class="">
                            <div class="text-h5 text-primary mb-4 text-medium-emphasis">
                                Empowering You with the Tools for Personal Transformation
                            </div>
                            <p class="font-weight-medium text-medium-emphasis text-body-2 mb-4 pl-1">
                                SLC empowers individuals in their journey of continuous self-improvement through personalized assessments, actionable insights, and tracking tools. With our user-friendly platform, individuals can gain self-awareness, set meaningful goals, and take tangible steps towards personal growth, career advancement, and wellness. Unlock your full potential for continuous improvement with our empowering service.
                            </p>
                            <p class="font-weight-medium text-medium-emphasis text-body-2 mb-0 pl-1">
                                With our user-friendly platform, individuals can gain self-awareness, set meaningful goals, and take tangible steps towards personal growth, career advancement, and wellness. Unlock your full potential for continuous improvement with our empowering service.
                            </p>
                        </v-card-item>
                        <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn class="ml-2 rounded-pill px-8 py-2" variant="elevated" color="primary"
                                size="medium">Read More</v-btn>
                        </v-card-actions>
                    </v-card>
                </v-col>
            </v-row>
            </v-container>
    </v-container>
</template>

<style scoped>
.about-section {
    /* padding: 3rem 0; */

}

.about-card {
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-content: start;
    margin-top: 4rem;
}

.about-container {}

.coaching-gif {
    max-width: 90%;
}
</style>