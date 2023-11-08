<template>
    <div class="side">
        <aside>
            <div class="item">
                <h1>about</h1>
            </div>
            <div class="item">
                <h1>prices</h1>
            </div>
            <div class="item">
                <h1>contact</h1>
            </div>
            <div class="item">
                <h1>services</h1>
            </div>
        </aside>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.side{
    background: #ff5983;
    color: white;
    padding: .75em;
    aside{
        display: flex;
        gap: 1em;
        align-items: center;
        .item{
            cursor: pointer;
            transform: 200ms;
            &:hover{
                color: rgb(255, 210, 47);
            }
        }
    }
}
</style>