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
                return `<div>group node </div>`;
            },
            renderRuleNode: function (ruleNode) {
                return `<div> rule node</div>`;
            }
        }
    }
</script>

<style scoped>

</style>