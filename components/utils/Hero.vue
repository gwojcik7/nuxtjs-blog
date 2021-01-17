<template>
    <div class="hero">
        <div class="hero__heading">
            <slot name="heading"></slot>
        </div>
        <div class="hero__text">
            <slot name="text"></slot>
        </div>
        <div class="hero__button">
            <slot name="button"></slot>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .hero {
        &__heading {
            font-size: 5rem;
            padding: 0 0 2rem;
            line-height: 5rem;
        }
        &__text {
            font-size: 1.2rem;
            padding-bottom: 2rem;
        }
        &__button {

        }
    }
</style>