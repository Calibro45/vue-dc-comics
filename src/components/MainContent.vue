<template>
    <main class="container-fluid main-content-wrap">
        <div class="container">
            <p>{{ text }}</p>
        </div>
    </main>
</template>

<script>
export default {
    name: 'mainContent',
    data() {
        return {
            text: '--> Content goes here <--',
        }
    },
}
</script>

<style lang="scss" scoped>
.main-content-wrap {
    background-color: #1c1c1c;
    padding: 50px 5px;

    p {
        font-size: 36px;
        color: #fff;
        font-weight: 700;
    }
}

</style>