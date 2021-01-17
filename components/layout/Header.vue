<template>
    <Container>
        <header class="header">
            <div class="header__brand">
                <NuxtLink to="/">Grzesiek Wójcik</NuxtLink>
            </div>
            <nav class="header__nav">
                <ul>
                    <li>
                    <NuxtLink to="/o-mnie">O mnie</NuxtLink>
                    </li>
                    <li>
                    <NuxtLink to="/baza-wiedzy">Baza wiedzy</NuxtLink>
                    </li>
                    <li>
                    <NuxtLink to="/kontakt">Kontakt</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>
    </Container>
</template>
<script lang="ts">
import Vue from 'vue'
import Container from '~/components/layout/Container.vue'
export default Vue.extend({
    components: {
        Container
    }
})
</script>
<style lang="scss" scoped>
    .header {
        display: grid;
        grid-template-columns: 300px auto;
        &__brand {
            font-size: 1.8rem;
            font-weight: bold;
        }
        &__nav {
            justify-self: end;
            align-self: center;
            ul {
                list-style-type: none;
                padding-left: 0;
                margin: 0;
                li {
                    display: inline-block;
                    a {
                        padding: 1rem;
                    }
                }
            }
        }
    }
</style>