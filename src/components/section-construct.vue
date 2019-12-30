<template>
    <section class="promo d-flex justify-center flex-wrap align-items-center promo-hello">
        <div class="d-flex justify-center align-items-center santa-foto-wrap">
            <img src="@/assets/img/santa-krug.png" alt="" class="santa-bacground">
            <img src="@/assets/img/santa.png" alt="" class="santa-foto">

            <!-- consruct-1  -->

            <img src="@/assets/img/sigvei.png"
                v-if="pictures.santaSigvei.isVisible"
                alt=""
                class="santa-accses accses-1 santa-sigvei">

            <img src="@/assets/img/robot.png"
                 v-if="pictures.santaRobot.isVisible"
                alt=""
                class="santa-accses accses-1 santa-robot">

            <img src="@/assets/img/copter.png"
                 v-if="pictures.santaCopter.isVisible"
                alt=""
                class="santa-accses accses-1 santa-copter">

            <img src="@/assets/img/sani-santi.png"
                 v-if="pictures.santaSani.isVisible"
                alt=""
                class="santa-accses accses-1 santa-sani">

            <!-- consruct-2  -->

            <img src="@/assets/img/prom-manipuljator.png"
                 v-if="pictures.santaManipuljator.isVisible"
                 alt=""
                 class="santa-accses accses-2 santa-manipuljator">

            <img src="@/assets/img/cat-icecreem.png"
                 v-if="pictures.santaCatIcecreem.isVisible"
                 alt=""
                 class="santa-accses accses-2 santa-cat-icecreem">

            <img src="@/assets/img/monitor.png"
                 v-if="pictures.santaMonitor.isVisible"
                 alt=""
                 class="santa-accses accses-2 santa-monitor">

            <img src="@/assets/img/elf.png"
                 v-if="pictures.santaElf.isVisible"
                 alt=""
                 class="santa-accses accses-2 santa-elf">

            <!-- consruct-3  -->

            <img src="@/assets/img/telescop.png"
                 v-if="pictures.santaTelescop.isVisible"
                 alt=""
                 class="santa-accses accses-3 santa-telescop">

            <img src="@/assets/img/nii-center.png"
                 v-if="pictures.santaNiiCenter.isVisible"
                 alt=""
                 class="santa-accses accses-3 santa-nii-center">

            <img src="@/assets/img/raketa.png"
                 v-if="pictures.santaRaketa.isVisible"
                 alt=""
                 class="santa-accses accses-3 santa-raketa">

            <img src="@/assets/img/snegovik.png"
                 v-if="pictures.santaSnegovik.isVisible"
                 alt=""
                 class="santa-accses accses-3 santa-snegovik">

            <!-- consruct-4  -->

            <img src="@/assets/img/racija.png"
                 v-if="pictures.santaRacija.isVisible"
                 alt=""
                 class="santa-accses accses-4 santa-racija">

            <img src="@/assets/img/power-bank.png"
                 v-if="pictures.santaPowerBank.isVisible"
                 alt=""
                 class="santa-accses accses-4 santa-power-bank">

            <img src="@/assets/img/vr-glass.png"
                 v-if="pictures.santaVr.isVisible"
                 alt=""
                 class="santa-accses accses-4 santa-vr">


            <!-- consruct-5  -->

            <img src="@/assets/img/binokle.png"
                 v-if="pictures.santaBinokle.isVisible"
                 alt=""
                 class="santa-accses accses-5 santa-binokle">

            <img src="@/assets/img/ssd-disc.png"
                 v-if="pictures.santaSsdDisc.isVisible"
                 alt=""
                 class="santa-accses accses-5 santa-ssd-disc">

            <img src="@/assets/img/5g-seti.png"
                 v-if="pictures.santaSeti.isVisible"
                 alt=""
                 class="santa-accses accses-5 santa-5g-seti">

            <img src="@/assets/img/mail-box.png"
                 v-if="pictures.santaMailBox.isVisible"
                 alt=""
                 class="santa-accses accses-5 santa-mail-box">

            <!-- consruct-6  -->

            <img src="@/assets/img/cap-coffe.png"
                 v-if="pictures.santaCapCoffe.isVisible"
                 alt=""
                 class="santa-accses accses-6 santa-cap-coffe">

            <img src="@/assets/img/glass-juce.png"
                 v-if="pictures.santaGlassJuce.isVisible"
                 alt=""
                 class="santa-accses accses-6 santa-glass-juce">

            <img src="@/assets/img/santa-retrit.png"
                 v-if="pictures.santaRetrit.isVisible"
                 alt=""
                 class="santa-accses accses-6 santa-retrit">

            <img src="@/assets/img/pie-cake.png"
                 v-if="pictures.santaPieCake.isVisible"
                 alt=""
                 class="santa-accses accses-6 santa-pie-cake">
        </div>

        <choise-one
                v-if="currentChoise == 'choise1'"
                :setRobotVisible="setRobotVisible"
                :setRobotHover="setRobotHover"
                :setSaniVisible="setSaniVisible"
                :setSaniHover="setSaniHover"
                :setScuteerVisible="setScuteerVisible"
                :setScuteerHover="setScuteerHover"
                :setsetDronVisible="setDronVisible"
                :setsetDronHover="setDronHover"
        />
        <choise-tou
                v-if="currentChoise == 'choise2'"
                :setManipuljatorVisible="setManipuljatorVisible"
                :setCatIcecreemVisible="setCatIcecreemVisible"
                :setMonitorVisible="setMonitorVisible"
                :setElfVisible="setElfVisible"
                :setManipuljatorHover="setManipuljatorHover"
                :setCatIcecreemHover="setCatIcecreemHover"
                :setMonitorHover="setMonitorHover"
                :setElfHover="setElfHover"
        />
        <choise-three
                v-if="currentChoise == 'choise3'"
                :setTelescopVisible="setTelescopVisible"
                :setNiiCenterVisible="setNiiCenterVisible"
                :setRaketaVisible="setRaketaVisible"
                :setSnegovikVisible="setSnegovikVisible"
                :setTelescopHover="setTelescopHover"
                :setNiiCenterHover="setNiiCenterHover"
                :setRaketaHover="setRaketaHover"
                :setSnegovikHover="setSnegovikHover"
        />
        <choise-fou
                v-if="currentChoise == 'choise4'"
                :setRacijaVisible="setRacijaVisible"
                :setPowerBankVisible="setPowerBankVisible"
                :setVrVisible="setVrVisible"
                :setRacijaHover="setRacijaHover"
                :setPowerBankHover="setPowerBankHover"
                :setVrHover="setVrHover"
        />
        <choise-five
                v-if="currentChoise == 'choise5'"
                :setBinokleVisible="setBinokleVisible"
                :setSsdDiscVisible="setSsdDiscVisible"
                :setSetiVisible="setSetiVisible"
                :setMailBoxVisible="setMailBoxVisible"
                :setBinokleHover="setBinokleHover"
                :setSsdDiscHover="setSsdDiscHover"
                :setSetiHover="setSetiHover"
                :setMailBoxHover="setMailBoxHover"
        />
        <choise-six
                v-if="currentChoise == 'choise6'"
                :setCapCoffeVisible="setCapCoffeVisible"
                :setGlassJuceVisible="setGlassJuceVisible"
                :setRetritVisible="setRetritVisible"
                :setPieCakeVisible="setPieCakeVisible"
                :setCapCoffeHover="setCapCoffeHover"
                :setGlassJuceHover="setGlassJuceHover"
                :setRetritHover="setRetritHover"
                :setPieCakeHover="setPieCakeHover"
        />
        <end-mission
                v-if="currentChoise == 'choise7'"
        />
    </section>
</template>

<script>
    import ChoiseOne from "./button-choise/choise-one";
    import ChoiseTou from "./button-choise/choise-tou";
    import ChoiseThree from "./button-choise/choise-three";
    import ChoiseFou from "./button-choise/choise-fou";
    import ChoiseFive from "./button-choise/choise-five";
    import ChoiseSix from "./button-choise/choise-six";
    import EndMission from "./button-choise/end-mission";

    export default {
        name: "section-construct",
        components: {
            EndMission,
            ChoiseSix,
            ChoiseFive,
            ChoiseFou,
            ChoiseThree,
            ChoiseTou,
            ChoiseOne
        },
        data(){
            return {
                currentChoise: 'choise1',
                pictures: {
                    santaSigvei: { isVisible: false, id: 1 },
                    santaRobot: { isVisible: false, id: 2 },
                    santaCopter: { isVisible: false, id: 3 },
                    santaSani: { isVisible: false, id: 4 },
                    santaManipuljator: { isVisible: false, id: 5 },
                    santaCatIcecreem: { isVisible: false, id: 6 },
                    santaMonitor: { isVisible: false, id: 7 },
                    santaElf: { isVisible: false, id: 8 },
                    santaTelescop: { isVisible: false, id: 9 },
                    santaNiiCenter: { isVisible: false, id: 10 },
                    santaRaketa: { isVisible: false, id: 11 },
                    santaSnegovik: { isVisible: false, id: 12 },
                    santaRacija: { isVisible: false, id: 13 },
                    santaPowerBank: { isVisible: false, id: 14 },
                    santaVr: { isVisible: false, id: 15 },
                    santaBinokle: { isVisible: false, id: 16 },
                    santaSsdDisc: { isVisible: false, id: 17 },
                    santaSeti: { isVisible: false, id: 18 },
                    santaMailBox: { isVisible: false, id: 19 },
                    santaCapCoffe: { isVisible: false, id: 20 },
                    santaGlassJuce: { isVisible: false, id: 21 },
                    santaRetrit: { isVisible: false, id: 22 },
                    santaPieCake: { isVisible: false, id: 23 },
                },
                activePictures: [],
            }
        },
        methods: {

            setRobotVisible() {
                this.pictures.santaRobot.isVisible = true;
                this.activePictures.push(this.pictures.santaRobot.id);
                this.currentChoise = 'choise2';
            },

            setScuteerVisible() {
                this.pictures.santaSigvei.isVisible = true;
                this.activePictures.push(this.pictures.santaSigvei.id);
                this.currentChoise = 'choise2';
            },

            setDronVisible() {
                this.pictures.santaCopter.isVisible = true;
                this.activePictures.push(this.pictures.santaCopter.id);
                this.currentChoise = 'choise2';
            },

            setSaniVisible() {
                this.pictures.santaSani.isVisible = true;
                this.activePictures.push(this.pictures.santaSani.id);
                this.currentChoise = 'choise2';
            },

            setRobotHover() {
                this.pictures.santaRobot.isVisible = !this.pictures.santaRobot.isVisible;
            },
            setDronHover() {
                this.pictures.santaCopter.isVisible = !this.pictures.santaCopter.isVisible;
            },
            setScuteerHover() {
                this.pictures.santaSigvei.isVisible = !this.pictures.santaSigvei.isVisible;
            },
            setSaniHover() {
                this.pictures.santaSani.isVisible = !this.pictures.santaSani.isVisible;
            },

            setManipuljatorVisible() {
                this.pictures.santaManipuljator.isVisible = true;
                this.activePictures.push(this.pictures.santaManipuljator.id);
                this.currentChoise = 'choise3';
            },
            setCatIcecreemVisible() {
                this.pictures.santaCatIcecreem.isVisible = true;
                this.activePictures.push(this.pictures.santaCatIcecreem.id);
                this.currentChoise = 'choise3';
            },
            setMonitorVisible() {
                this.pictures.santaMonitor.isVisible = true;
                this.activePictures.push(this.pictures.santaMonitor.id);
                this.currentChoise = 'choise3';
            },
            setElfVisible() {
                this.pictures.santaElf.isVisible = true;
                this.activePictures.push(this.pictures.santaElf.id);
                this.currentChoise = 'choise3';
            },

            setManipuljatorHover() {
                this.pictures.santaManipuljator.isVisible = !this.pictures.santaManipuljator.isVisible;
            },
            setCatIcecreemHover() {
                this.pictures.santaCatIcecreem.isVisible = !this.pictures.santaCatIcecreem.isVisible;
            },
            setMonitorHover() {
                this.pictures.santaMonitor.isVisible = !this.pictures.santaMonitor.isVisible;
            },
            setElfHover() {
                this.pictures.santaElf.isVisible = !this.pictures.santaElf.isVisible;
            },

            setTelescopVisible() {
                this.pictures.santaTelescop.isVisible = true;
                this.activePictures.push(this.pictures.santaTelescop.id);
                this.currentChoise = 'choise4';
            },
            setNiiCenterVisible() {
                this.pictures.santaNiiCenter.isVisible = true;
                this.activePictures.push(this.pictures.santaNiiCenter.id);
                this.currentChoise = 'choise4';
            },
            setRaketaVisible() {
                this.pictures.santaRaketa.isVisible = true;
                this.activePictures.push(this.pictures.santaRaketa.id);
                this.currentChoise = 'choise4';
            },
            setSnegovikVisible() {
                this.pictures.santaSnegovik.isVisible = true;
                this.activePictures.push(this.pictures.santaSnegovik.id);
                this.currentChoise = 'choise4';
            },

            setTelescopHover() {
                this.pictures.santaTelescop.isVisible = !this.pictures.santaTelescop.isVisible;
            },
            setNiiCenterHover() {
                this.pictures.santaNiiCenter.isVisible = !this.pictures.santaNiiCenter.isVisible;
            },
            setRaketaHover() {
                this.pictures.santaRaketa.isVisible = !this.pictures.santaRaketa.isVisible;
            },
            setSnegovikHover() {
                this.pictures.santaSnegovik.isVisible = !this.pictures.santaSnegovik.isVisible;
            },

            setRacijaVisible() {
                this.pictures.santaRacija.isVisible = true;
                this.activePictures.push(this.pictures.santaRacija.id);
                this.currentChoise = 'choise5';
            },
            setPowerBankVisible() {
                this.pictures.santaPowerBank.isVisible = true;
                this.activePictures.push(this.pictures.santaPowerBank.id);
                this.currentChoise = 'choise5';
            },
            setVrVisible() {
                this.pictures.santaVr.isVisible = true;
                this.activePictures.push(this.pictures.santaVr.id);
                this.currentChoise = 'choise5';
            },

            setRacijaHover() {
                this.pictures.santaRacija.isVisible = !this.pictures.santaRacija.isVisible;
            },
            setPowerBankHover() {
                this.pictures.santaPowerBank.isVisible = !this.pictures.santaPowerBank.isVisible;
            },
            setVrHover() {
                this.pictures.santaVr.isVisible = !this.pictures.santaVr.isVisible;
            },

            setBinokleVisible() {
                this.pictures.santaBinokle.isVisible = true;
                this.activePictures.push(this.pictures.santaBinokle.id);
                this.currentChoise = 'choise6';
            },
            setSsdDiscVisible() {
                this.pictures.santaSsdDisc.isVisible = true;
                this.activePictures.push(this.pictures.santaSsdDisc.id);
                this.currentChoise = 'choise6';
            },
            setSetiVisible() {
                this.pictures.santaSeti.isVisible = true;
                this.activePictures.push(this.pictures.santaSeti.id);
                this.currentChoise = 'choise6';
            },
            setMailBoxVisible() {
                this.pictures.santaMailBox.isVisible = true;
                this.activePictures.push(this.pictures.santaMailBox.id);
                this.currentChoise = 'choise6';
            },

            setBinokleHover() {
                this.pictures.santaBinokle.isVisible = !this.pictures.santaBinokle.isVisible;
            },
            setSsdDiscHover() {
                this.pictures.santaSsdDisc.isVisible = !this.pictures.santaSsdDisc.isVisible;
            },
            setSetiHover() {
                this.pictures.santaSeti.isVisible = !this.pictures.santaSeti.isVisible;
            },
            setMailBoxHover() {
                this.pictures.santaMailBox.isVisible = !this.pictures.santaMailBox.isVisible;
            },

            setCapCoffeVisible() {
                this.pictures.santaCapCoffe.isVisible = true;
                this.activePictures.push(this.pictures.santaCapCoffe.id);
                this.currentChoise = 'choise7';
            },
            setGlassJuceVisible() {
                this.pictures.santaGlassJuce.isVisible = true;
                this.activePictures.push(this.pictures.santaGlassJuce.id);
                this.currentChoise = 'choise7';
            },
            setRetritVisible() {
                this.pictures.santaRetrit.isVisible = true;
                this.activePictures.push(this.pictures.santaRetrit.id);
                this.currentChoise = 'choise7';
            },
            setPieCakeVisible() {
                this.pictures.santaPieCake.isVisible = true;
                this.activePictures.push(this.pictures.santaPieCake.id);
                this.currentChoise = 'choise7';
            },

            setCapCoffeHover() {
                this.pictures.santaCapCoffe.isVisible = !this.pictures.santaCapCoffe.isVisible;
            },
            setGlassJuceHover() {
                this.pictures.santaGlassJuce.isVisible = !this.pictures.santaGlassJuce.isVisible;
            },
            setRetritHover() {
                this.pictures.santaRetrit.isVisible = !this.pictures.santaRetrit.isVisible;
            },
            setPieCakeHover() {
                this.pictures.santaPieCake.isVisible = !this.pictures.santaPieCake.isVisible;
            },
        }
    }
</script>

<style scoped>

</style>