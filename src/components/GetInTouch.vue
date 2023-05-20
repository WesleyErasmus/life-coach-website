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
                            Get back on track with Strategic Life Coaching. Get In Touch to Schedule a Session
                            and Start Your Transformation.
                        </div>
                    </v-card-item>
                    <v-card-actions class="contact-btn-container">
                        <v-btn class="rounded-pill px-8 py-2" variant="elevated" size="large" @click="dialog = true">
                            <!-- <a href="mailto:daryl@ontrackcoaching.co.za?subject=Online Coaching Enquiry"
                                class="text-decoration-none text-black"> -->
                            Get In Touch
                            <!-- </a> -->
                        </v-btn>
                    </v-card-actions>
                </div>
            </v-card>
        </v-container>
    </v-card>

    <!-- Get in touch form -->

    <v-row justify="center">
        <v-dialog v-model="dialog" persistent width="1024">
            <v-card>
                <v-card-title class="pa-0">
                    <!-- Dialog Title -->
                    <v-toolbar dark color="primary">
                        <v-toolbar-title>Get In Touch</v-toolbar-title>
                        <v-spacer></v-spacer>
                        <!-- Dialog close button -->
                        <v-btn icon dark @click="dialog = false">
                            <v-icon>mdi-close</v-icon>
                        </v-btn>
                    </v-toolbar>
                </v-card-title>
                <v-card-text>
                    <v-container>
                        <v-row>
                            <v-col cols="12" sm="6" md="6">
                                <!-- First Name Input -->
                                <v-text-field label="First name*" required></v-text-field>
                            </v-col>
                            <v-col cols="12" sm="6" md="6">
                                <!-- Last Name Input -->
                                <v-text-field label="Last name*" required></v-text-field>
                            </v-col>

                            <!-- Email Input -->
                            <v-col cols="12">
                                <v-text-field label="Email*" required></v-text-field>
                            </v-col>
                            <v-col cols="12" sm="12">
                                <!-- Select Services -->
                                <v-autocomplete
                                    :items="['Setting Your Course', 'Getting Your Career Back On Track', 'Finding Traction In Your Relationships', 'Thinking Like a Leader']"
                                    label="Select Coaching Services*" multiple required
                                    hint="You can select more than one"></v-autocomplete>
                            </v-col>
                            <!-- Message Textarea -->
                            <v-col cols="12">
                                <v-textarea label="Message*" required></v-textarea>
                            </v-col>
                        </v-row>
                    </v-container>
                    <!-- Required note -->
                    <small>*indicates required field</small>
                </v-card-text>
                <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn color="" variant="text" @click="dialog = false">
                        Close
                    </v-btn>
                    <v-btn color="primary" variant="text" @click="dialog = false">
                        Send
                    </v-btn>
                </v-card-actions>
            </v-card>
        </v-dialog>
    </v-row>

    <!-- End of get in touch form -->
</template>

<script>
export default {
    data() {
        return {
            dialog: false,
        };
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
}
</style>