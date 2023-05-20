<template>
    <v-container class="mt-16 mb-10">
        <v-row class="fill-height" align="start" justify="center">
            <template v-for="(item, i) in items" :key="i">
                <v-col cols="12" lg="3" md="4" sm="6">
                    <v-hover v-slot="{ isHovering, props }">
                        <v-card class="pa-4 elevation-0" :variant="isHovering ? 'tonal' : undefined"
                            :color="isHovering ? 'primary' : undefined" v-bind="props">
                            <div>
                                <div class="img-container">
                                    <img class="services-card-images-top" :src="item.img" alt="Services-card-images">
                                </div>
                                <v-card-text class="card-title-container text-h6 font-weight-bold d-flex flex-column">
                                    <p class="mt-0">
                                        {{ item.title }}
                                    </p>
                                </v-card-text>
                                <v-card-text>
                                    <p class="card-text-container text-caption font-weight-medium text-medium-emphasis">
                                        <!-- {{ shortSubtext[i] }} -->
                                        {{ item.subtitle }}
                                    </p>
                                </v-card-text>
                                <v-expand-transition>
                                    <div v-show="show[i]">
                                        <!-- <v-divider class="text-primary"></v-divider> -->

                                        <v-card-text class="mt-0 pt-0">
                                            <!-- Expand "see more" heading -->
                                            <h3 class="text-primary">
                                                "{{ item.expand }}"
                                            </h3>
                                        <p class="text-body-2 text-medium-emphasis" >
                                            <!-- {{ shortSubtext[i] }} -->
                                            {{ item.subtext }}
                                        </p>
                                    </v-card-text>
                                    </div>
                                </v-expand-transition>
                                  <v-card-actions class="mt-0 pt-0">
                                        <v-btn class="rounded-pill px-4" size="small" variant="outlined" color="primary"
                                           :prepend-icon="show[i] ? 'mdi-chevron-up' : 'mdi-chevron-down'"
                                          @click="show[i] = !show[i]"
                                            >
                                            See More
                                        </v-btn>
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
          // Card see more button that expands the services card
        show: [],
        items: [
            {
                img: "https://i.postimg.cc/7PVrDkh8/chart.png",
                title: 'Setting Your Course',
                expand: "Goals",
                subtitle: 'A personalized approach to assist individuals in setting and achieving specific goals.',
                subtext: 'A personalized approach to assist individuals in setting and achieving specific goals through effective planning, and action strategies. I help individuals identify their priorities, develop a road map, and overcome obstacles to reach their desired outcomes and create a fulfilling life.',

            },
            {
                img: "https://i.postimg.cc/kgLkwM18/goal.png",
                title: 'Getting Your Career Back On Track',
                expand: "Career",
                subtitle: 'Provides a tailored approach to help individuals improve their professional skills.',
                subtext: 'My "Getting Your Career Back On Track" coaching service provides a supportive and tailored approach to help individuals improve their professional skills, set achievable career goals, and enhance job prospects for career advancement and success. Our experienced career coaches assist in exploring individual interests, values, strengths, and provide strategic planning to help individuals reach their full potential.',

            },
            {
                img: "https://i.postimg.cc/wT4KyQDw/balance.png",
                title: 'Finding Traction In Your Relationships',
                expand: "Relationships",
                subtitle: 'The quest for spirituality(SQ) and the value of emotional intelligence as a people leader.',
                subtext: 'A depth of forgiveness and spiritual well being. With the aid of a relational eco- map we will journey through the process of conflict.finding a deeper sense of identity - The quest for spirituality(SQ) and the value of emotional intelligence as a people leader.',

            },
            {
                img: "https://i.postimg.cc/cCsqYDDb/interview.png",
                title: 'Thinking Like a Leader',
                expand: "Leadership",
                subtitle: 'Be willing to explore your circle of influence whilst setting up a strategic plan.',
                subtext: 'Developing good habits early on through the use of a habit tracker and journaling. Be willing to explore your circle of influence whilst setting up a strategic plan for your business sphere and life.The use of vision boards, life swots and key questions will assist us in moving form “Here to There"',

            },
        ],
    }),
    computed: {
        shortSubtext() {
            return this.items.map(item => {
                const words = item.subtext.split(' ')
                return words.slice(0, 25).join(' ') + (words.length > 25 ? '...' : '')
            })
        }
    }

}
</script>
<style scoped>
.services-card-images-top {
    width: 55px;
    margin-left: 1rem;
}

.card-title-container {
    height: 55px;
}

.card-text-container {
    /* height: 90px; */
    overflow: hidden;
    position: relative;
}

.v-card:hover {
    border-top: 2px solid #1976D2;
}

@media (max-width: 959px) {
    .services-card-images-top {
        width: 85px;
        margin-left: 1rem;
    }
}

@media (max-width: 736px) {
    .img-container {
        text-align: center;
    }

    .services-card-images-top {
        width: 105px;
    }

    .v-card-title {
        text-align: center;
    }
}
</style>