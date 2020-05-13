<template>
    <div class="home">
        <div>
            rootNodeType:{{this.logicData.logicType}}<br/>
            logicType:{{this.logicData.logicType}}<br/>
        </div>
        <br/>
        ===================================================
        <br/>

        <SimpleLogic v-model="logicData"/>
    </div>
</template>

<script>
    // @ is an alias to /src
    import SimpleLogic from "@/components/SimpleLogic.vue";

    export default {
        name: "Home",
        components: {
            SimpleLogic
        },
        data: function () {
            return {
                logicData: {
                    nodeType: "groupNode",
                    logicType: "and",
                    values: []
                }
            }
        }
    };
</script>
