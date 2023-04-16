<template>
    <v-container class="my-15">
        <v-row class="fill-height" align="center" justify="center">
            <template v-for="(item, i) in items" :key="i">
                <v-col cols="12" md="3">
                    <v-hover v-slot="{ isHovering, props }">
                        <v-card class="pa-4 elevation-0" :variant="isHovering ? 'tonal' : undefined" :color="isHovering ? 'primary' : undefined" v-bind="props">
                            <div>
                                <img class="services-card-images-top" :src="item.img" alt="Services-card-images">
                                <v-card-title class="text-h6 d-flex flex-column">
                                    <p class="mt-4">
                                        {{ item.title }}
                                    </p>

                                </v-card-title>
                                <v-card-text>
                                    <p class="text-caption font-weight-medium text-medium-emphasis">
                                        {{ item.subtext }}
                                    </p>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn variant="tonal" icon="mdi-arrow-right-thin"></v-btn>
                                </v-card-actions>
                            </div>
                        </v-card>
                    </v-hover>
                </v-col>
            </template>
        </v-row>
    </v-container>
</template>
<script>
export default {
    data: () => ({
        items: [
            {
                img: '../../public/icons/chart.png',
                title: 'Reach Your Goals',
                text: `It's New Release Friday`,
                subtext: 'Setting and achieving specific, measurable, and meaningful goals through effective planning, motivation, and action strategies.',

            },
            {
                img: '../../public/icons/goal.png',
                title: 'Career Growth',
                text: 'Greatest Rock Hits',
                subtext: 'Advancing professional skills, achieving career goals, and improving job prospects for career advancement and success.',

            },
            {
                img: '../../public/icons/balance.png',
                title: 'Lifestyle Balance',
                text: 'Ambient Bass',
                subtext: 'Striking a healthy balance between work, personal life, health, and well-being for improved overall quality of life.',

            },
            {
                img: '../../public/icons/interview.png',
                title: 'Interview Preparation',
                text: 'Ambient Bass',
                subtext: 'Coaching and guidance to prepare for job interviews, including mock interviews, resume review, and interview techniques.',

            },
        ],
    }),
}
</script>
<style scoped>
.services-card-images-top {
    width: 55px;
    margin-left: 1rem;
}
.v-card:hover {
  border-top: 2px solid #1976D2;
  cursor: pointer;
}
</style>