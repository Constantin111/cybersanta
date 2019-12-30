<template>
    <div id="app" class="container-fluid d-flex">
        <div class="lapa-eli-left">
            <img src="@/assets/img/lapa-eli-left.png" alt=""/>
        </div>
        <div class="lapa-eli-right">
            <img src="@/assets/img/lapa-eli-right.png" alt=""/>
        </div>
        <section-hello v-if="currentPage == 'page1'" @start-begin="startBegin"/>
        <section-begin v-if="currentPage == 'page2'" @start-construct="startConstruct"/>
        <section-construct v-if="currentPage == 'page3'"/>
    </div>
</template>

<script>
    import sectionHello from './components/section-hello.vue'
    import sectionBegin from './components/section-begin.vue'
    import sectionConstruct from './components/section-construct.vue'

    export default {
        name: 'app',
        data() {
            return {
                currentPage: 'page1',
            }
        },
        components: {
            sectionHello,
            sectionBegin,
            sectionConstruct,
        },
        methods: {
            startBegin() {
                /*this.pictures.robot.isVisible = true;
                this.activePictures.push(this.pictures.robot.path);*/
                this.currentPage = 'page2';
            },
            startConstruct(){
                /*this.pictures.robot.isVisible = true;
                this.activePictures.push(this.pictures.robot.path);*/
                this.currentPage = 'page3';
            }
        }

    }
</script>

<style>

</style>
