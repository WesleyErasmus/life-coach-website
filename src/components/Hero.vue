<template>
    <!-- Main content -->
    <v-container class="hero-banner" fluid>
        <v-container>
        <v-row>
            <v-col class="d-flex justify-center" md="6">
                <v-card class="hero-card bg-transparent" variant="none">
                    <v-card-item class="text-white">
                        <div class="text-h3 mb-4">
                            Strategic Life Coaching
                        </div>
                        <p class="text-body-1 mb-4 pl-1">
                            Guiding individuals in identifying their strengths, setting goals, creating action plans, and implementing strategies to achieve personal and professional success while maintaining balance and fulfillment in life.
                        </p>
                    </v-card-item>
                    <v-card-actions>
                        <v-btn class="ml-2 rounded-pill px-8 py-2" variant="elevated" color="primary" size="x-large">View services</v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
            <v-col class="d-flex justify-end" md="6">
                <img class="coaching-gif elevation-0 rounded-circle ma-8" src="../assets/career-coaching.gif" alt="Coaching-Asset">
            </v-col>
        </v-row>
        </v-container>
    </v-container>
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
</style>
