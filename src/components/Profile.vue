<template style="background-color: #0d0d0d;">
    <b-container fluid>
        <b-row style="background-color: #0B0C10; height: 40vh">
            <img style="padding: 0px" src="../assets/bgimage2.jpg" />
        </b-row>
        <b-row h-60 style="background-color: #0d0d0d; height: 100%">
            <b-col cols="1"></b-col>
            <b-col cols="10">
                <b-card style="z-index: 10; height: 100vh; margin-top: -100px; margin-bottom: 50px;  background-color: #1F2833;">
                    <b-row>
                        <b-col cols="3"></b-col>
                        <b-col cols="6" style="text-align: center"><img src="../assets/profileImgBW.jpg" alt="a picture of Jaydon Goodrich" style="width: 150px; padding: 0px; margin-top: -100px; border-radius: 50%;"></b-col>
                        <b-col cols="3"></b-col>
                    </b-row>
                    <b-row>
                        <b-col cols="2"></b-col>
                        <b-col cols="8"><h2 style="text-align: center; color: #66FCF1; font-size: 30px; font-weight: bold; padding-top: 5px;">Jaydon Goodrich</h2></b-col>
                        <b-col cols="2"></b-col>
                    </b-row>
                    <b-row>
                        <b-col cols="2"></b-col>
                        <b-col cols="8"><p style="text-align: center; color: #C5C6C7; font-weight: bold;">FULL STACK DEVELOPER</p></b-col>
                        <b-col cols="2"></b-col>
                    </b-row>
                    <b-row>
                        <b-col cols="2"></b-col>
                        <b-col cols="8" style="text-align: center;">
                            <b-row style="padding-top: 30px; text-align: center;">
                                <b-col cols="4"><b-icon @click="display('tech')" icon="tools" font-scale="2.5" class="rounded p-2" :style="techSection == false ? 'color: #66FCF1; border: 1px solid #66FCF1;' : 'color: white; border: 1px solid white' "></b-icon></b-col>
                                <b-col cols="4"><b-icon @click="display('projects')" icon="grid-fill" font-scale="2.5" class="rounded p-2" :style="projectSection == false ? 'color: #66FCF1; border: 1px solid #66FCF1;' : 'color: white; border: 1px solid white' "></b-icon></b-col>
                                <b-col cols="4"><b-icon @click="display('about')" icon="person-fill" font-scale="2.5" class="rounded p-2" :style="aboutSection == false ? 'color: #66FCF1; border: 1px solid #66FCF1;' : 'color: white; border: 1px solid white' "></b-icon></b-col>
                            </b-row>
                        </b-col>
                        <b-col cols="2"></b-col>
                    </b-row>
                    <b-row v-if="techSection" style="margin: 0px; text-align: center">
                        <b-col cols="12" style="text-align: center; padding-top: 30px">
                        <b-row>
                            <b-col cols="2"></b-col>
                            <b-col cols="8"><p style="color: #C5C6C7; font-weight: bold;">TECHNOLOGIES</p></b-col>
                            <b-col cols="2"></b-col>
                        </b-row>
                        <b-row class="pt-3" style="text-align: center; padding: 0px;">
                            <b-col cols="4"><img src="../assets/html_logo.png" alt="Dart logo" style="width: 50px;"></b-col>
                            <b-col cols="4"><img src="../assets/css_logo.png" alt="Dart logo" style="width: 50px;"></b-col>
                            <b-col cols="4"><img src="../assets/js_logo.png" alt="Dart logo" style="width: 50px;"></b-col>
                        </b-row>
                        <b-row class="pt-3" style="text-align: center">
                            <b-col cols="4"><img src="../assets/node_logo.png" alt="Dart logo" style="width: 50px;"></b-col>
                            <b-col cols="4"><img src="../assets/php-logo.svg" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                            <b-col cols="4"><img src="../assets/vue_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                        </b-row>
                        <b-row class="pt-3" style="text-align: center">
                            <b-col cols="4"><img src="../assets/react_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                            <b-col cols="4"><img src="../assets/laravel_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                            <b-col cols="4"><img src="../assets/Flutter.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                        </b-row>
                        <b-row class="pt-3" style="text-align: center">
                            <b-col cols="4"><img src="../assets/firebase_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                            <b-col cols="4"><img src="../assets/mysql_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                            <b-col cols="4"><img src="../assets/dart_logo.png" alt="Dart logo" style="width: 50px; padding: 0px;"></b-col>
                        </b-row>
                        </b-col>
                    </b-row>
                    <b-row v-if="projectSection" style="text-align: center">
                        <b-col cols="12" style="text-align: center; padding-top: 30px">
                            <b-row>
                                <b-col cols="2"></b-col>
                                <b-col cols="8"><p style="color: #C5C6C7; font-weight: bold; text-align: center">PROJECTS</p></b-col>
                                <b-col cols="2"></b-col>    
                            </b-row>
                            <b-row>
                                <b-col cols="6" style="padding: 5px;"><a href="https://flight-deck-avionics.vercel.app/" target="_blank"><img style="width: 100%" src="../assets/flight_deck.png" alt=""></a></b-col>
                                <b-col cols="6" style="padding: 5px;"><a href="https://jaydon-goodrich.github.io/ultimatertis/" target="_blank"><img style="width: 100%" src="../assets/ultimatetris.png" alt=""></a></b-col>
                            </b-row>
                            <b-row>
                                <b-col cols="6" style="padding: 5px;"><a href="https://ancient-lake-97986.herokuapp.com/" target="_blank"><img style="width: 100%" src="../assets/dine_Store1.png" alt=""></a></b-col>
                                <b-col cols="6" style="padding: 5px;"><a href="https://github.com/Jaydon-Goodrich/game-finder" target="_blank"><img style="width: 100%" src="../assets/game_finder.png" alt=""></a></b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                    <b-row v-if="aboutSection" style="padding-top: 30px;">
                        <b-col cols="12" style="text-align: center; padding-top: 30px">
                            <b-row>
                                <b-col cols="2"></b-col>
                                <b-col cols="8"><p style="color: #C5C6C7; font-weight: bold; text-align: center">ABOUT ME</p></b-col>
                                <b-col cols="2"></b-col>
                            </b-row>
                            <b-row>
                                <b-col cols="2"></b-col>
                                <b-col cols="8"><p style="color: #66FCF1; text-align: center">Thanks for visiting! <br><br> My name is Jaydon and I love web development. <br><br> Feel free to reach out!</p></b-col>
                                <b-col cols="2"></b-col>
                            </b-row>
                            <b-row style="padding-top: 30px; text-align: center;">
                                <b-col cols="4"><a href="https://www.linkedin.com/in/jaydon-goodrich-438a55167/" target="_blank"><b-icon icon="linkedin" font-scale="2.5" class="rounded p-2" style="color: #66FCF1;"></b-icon></a></b-col>
                                <b-col cols="4"><a href="https://github.com/Jaydon-Goodrich" target="_blank"><b-icon icon="github" font-scale="2.5" class="rounded p-2" style="color: #66FCF1;"></b-icon></a></b-col>
                                <b-col cols="4"><a href="JaydonGoodrichResume.pdf" download><b-icon icon="file-earmark-arrow-down" font-scale="2.5" class="rounded p-2" style="color: #66FCF1;"></b-icon></a></b-col>
                            </b-row>
                        </b-col>
                    </b-row>
                </b-card>
            </b-col>
            <b-col cols="1"></b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: 'Profile',
    props: {
        msg: String
    },
    data() {
        return {
            techSection: false,
            projectSection: false,
            aboutSection: false
        }
    },
    created() {
        this.display('tech');
    },
    methods: {
        display(section) {
            this.techSection = false;
            this.projectSection = false;
            this.aboutSection = false;

            switch(section) {
                case 'tech':
                   this.techSection = true; 
                break;
                case 'projects':
                   this.projectSection = true; 
                break;
                case 'about':
                   this.aboutSection = true; 
                break;
            }
        }
    }
}
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Oooh+Baby&display=swap'); 
    h2 {
        font-family: 'Oooh Baby', cursive;
    }
    .clicked {
        color: white;
    }
    /* 
        0B0C10
        1F2833
        C5C6C7
        66FCF1
        45A29E
        
        */

</style>