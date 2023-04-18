<!-- 空白div占位400*300 -->
<script lang="ts">
import { useLocalesStore } from '../stores/locales'
const locales = (useLocalesStore()).lang
export default {
    name: 'HomeView',
    setup() {
        return {
            locales
        }
    }
}
</script>

<template>
    <div>
        <h1>9 Channel</h1>
        <p>{{ locales.siteInfo }}</p>
        <div>
            <ul>
                <li>
                    <a href="https://ygo.9-ch.com">Yu-Gi-Oh! Tools</a>
                </li>
                <li>
                    <a href="https://blog.9-ch.com">Blog</a>
                </li>
            </ul>
        </div>

    </div>
</template>
<style scoped>
h1 {
    font-size: 2rem;
    font-weight: 400;
    margin: 0;
    padding: 0;
    text-align: left;
}

p {
    font-size: 1.2rem;
    font-weight: 400;
    margin: 5rem 0 5rem 0;
    padding: 0;
    text-align: left;
}
</style>