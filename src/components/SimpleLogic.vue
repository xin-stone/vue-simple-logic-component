<template>
    <div>
        {{this.renderNode(value)}}
    </div>
</template>

<script>
    export default {
        name: "SimpleLogic",
        props: {
            value: {
                nodeType: String,
                logicType: String,
                values: []
            }
        },
        watch: {
            'value': function (o, n) {
                this.value = n;

            }
        },
        methods: {
            renderNode: function (rootGroupNode) {

            },
            renderGroupNode: function (groupNode) {

            },
            renderRuleNode: function (ruleNode) {
                return `<div> hello world render rule node</div>`;
            }
        }
    }
</script>

<style scoped>

</style>