<template>
    <view class="content">
        <h1>{{ count }}</h1>

        <u-button type="primary"
                  size="medium"
                  @click="countChangeHandle">
            Count
        </u-button>
    </view>
</template>

<script lang="ts">
import { Component, Vue, Watch } from 'vue-property-decorator'

@Component
export default class Test extends Vue {
    count: number = 0

    @Watch('count', { immediate: true })
    onCountChange(val: string, oldVal: string) {
        console.log(`%c count onchange === `, 'color: #67c23a;', val, oldVal)
    }

    countChangeHandle() {
        this.count++
    }
}
</script>

<style>
</style>
