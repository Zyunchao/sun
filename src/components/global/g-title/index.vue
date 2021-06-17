<template>
    <view class="content">
        <h1>{{ title }}</h1>
    </view>
</template>

<script lang="ts">
import { Component, Prop, Vue, Watch } from 'vue-property-decorator'

@Component
export default class Test extends Vue {
    @Prop({ default: 'qwer', required: true, type: String })
    private title!: string
}
</script>

<style>
</style>
