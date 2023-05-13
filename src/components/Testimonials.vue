<template>
    <div class="bg-grey-lighten-4 py-15">
        <v-card class="text-center bg-transparent pb-0" variant="default">
            <v-card-title class="text-h4 text-primary font-weight-bold mb-2">Testimonials</v-card-title>
            <v-card-text class="text-medium-emphasis text-h6 mb-7">Real Success Stories: Hear from Thriving Clients.
            </v-card-text>
        </v-card>
        <v-carousel class="bg-transparent" cycle height="340" hide-delimiter-background show-arrows="hover">
            <v-carousel-item v-for="(slide, i) in slides" :key="i">
                <v-sheet class="bg-transparent" height="100%">
                    <div class="d-flex fill-height justify-center align-start">
                        <v-card class="carousel-card mx-auto elevation-0 pa-3" max-width="680">
                            <v-card-text class="text-body-2 text-medium-emphasis py-2">
                                <v-icon color="primary">mdi-format-quote-open</v-icon>
                                {{ slide.testimonial }}
                                <v-icon color="primary">mdi-format-quote-close</v-icon>
                            </v-card-text>


                            <v-card-actions>
                                <v-list-item class="w-100">
                                    <template v-slot:prepend>
                                        <v-avatar color="grey-darken-3" size="85" :image="slide.avatar"></v-avatar>
                                    </template>

                                    <v-list-item-title class="text-h6">{{ slide.name }}</v-list-item-title>

                                    <v-list-item-subtitle class="text-body-1">{{ slide.title }}</v-list-item-subtitle>
                                </v-list-item>
                            </v-card-actions>
                        </v-card>
                    </div>
                </v-sheet>
            </v-carousel-item>
        </v-carousel>
    </div>
</template>

<script>
export default {
    data() {
        return {
            slides: [
                {
                    avatar: 'https://randomuser.me/api/portraits/women/88.jpg',
                    name: 'Sara Johnson',
                    title: 'Marketing Manager',
                    testimonial: "Working with my strategic life coach has been a game-changer. I've been able to set and achieve specific, measurable, and meaningful goals through effective planning, motivation, and action strategies. My coach has helped me unlock my potential and reach new heights in my career and personal life.",
                },
                {
                    avatar: 'https://randomuser.me/api/portraits/men/41.jpg',
                    name: 'Michael Thompson',
                    title: 'Entrepreneur',
                    testimonial: "I highly recommend strategic life coaching to anyone looking to level up in their business or personal life. My coach has provided me with invaluable guidance and support in setting and achieving my goals. The strategies and techniques I've learned have helped me overcome challenges and achieve success beyond my expectations.",

                },
                {
                    avatar: 'https://randomuser.me/api/portraits/women/51.jpg',
                    name: 'Emily Chen',
                    title: 'Software Engineer',
                    testimonial: "As a software engineer, I face various challenges in my career. Working with my strategic life coach has been a game-changer. My coach has helped me develop effective strategies to overcome obstacles, enhance my skills, and achieve my professional goals. I'm more confident and focused in my career now, thanks to my coach.",

                },
                {
                    avatar: 'https://randomuser.me/api/portraits/women/76.jpg',
                    name: 'Jessica Lee',
                    title: 'Small Business Owner',
                    testimonial: "Strategic life coaching has been a game-changer for my small business. My coach has helped me develop clear business strategies, improve my leadership skills, and achieve my business goals. The guidance and support I've received have been invaluable, and I've seen significant positive changes in my business since I started working with my coach.",

                },
            ],

        }
    }
}
</script>
<style scoped>
.carousel-card {
    padding-top: 1rem;
    border-top: 2px solid #1976D2;
    border-radius: 0px;
}
@media (max-width: 890px) {
  /* .v-window__next, .v-window__prev {
  display: none !important;
}
  .v-window__left, .v-window__right {
  visibility: hidden !important;
}
.v-window__controls {
    display: none !important;
  }

  .v-btn, button {
    display: none !important;
  } */
}
</style>