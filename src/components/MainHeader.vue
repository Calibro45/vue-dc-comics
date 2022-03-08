<template>
    <header>
        <div class="container nav-wrapper">
            <figure class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <ol class="main-nav">
                <li class="nav-link">
                    <a href="#">character</a>
                </li>
                <li class="nav-link active">
                    <a href="#">comics</a>
                </li>
                <li class="nav-link">
                    <a href="#">movies</a>
                </li>
                <li class="nav-link">
                    <a href="#">tv</a>
                </li>
                <li class="nav-link">
                    <a href="#">games</a>
                </li>
                <li class="nav-link">
                    <a href="#">collectibles</a>
                </li>
                <li class="nav-link">
                    <a href="#">videos</a>
                </li>
                <li class="nav-link">
                    <a href="#">fans</a>
                </li>
                <li class="nav-link">
                    <a href="#">news</a>
                </li>
                <li class="nav-link">
                    <a href="#">shop</a>
                </li>
            </ol>
        </div>
    </header>
</template>

<script>
export default {
    name: 'mainHeader',
    
}
</script>

<style lang="scss" scoped>

.nav-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 15px 5px;

    .logo {
        width: 85px;
        height: 85px;
        flex-shrink: 0;
    }

    .main-nav {
        display: flex;
        align-items: center;
        gap: 30px;
        flex-wrap: wrap;

        .nav-link {
            padding: 5px 10px;
            text-transform: uppercase;
            font-size: 14px;
            font-weight: 700;
            position: relative;

            &.active {
                color: #579cfa
            }

            &.active::after {
                content: '';
                display: block;
                height: 5px;
                background-color: #579cfa;
                width: calc(100% - 20px);
                position: absolute;
                bottom: -100%;
            }

            &:hover {
                cursor: pointer;
                color: #579cfa;
            }
        }
    }
}


</style>