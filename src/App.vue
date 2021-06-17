<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    mpType: 'app',
    onLaunch() {
        console.log(`%c onLaunch`, 'color: #67c23a;')
    },
    onShow() {
        console.log('App Show')
    },
    onHide() {
        console.log('App Hide')
    }
})
</script>

<style lang="scss">
@import 'uview-ui/index.scss';
</style>
