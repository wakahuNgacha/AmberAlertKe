<template>
    <div class="holder">
        <div class="image">
            <img src="" alt="">
        </div>
        <div class="text">
            <div class="name">
                <span>Name</span>
                <span>Age: Gender: </span>
            </div>
            <div class="details">
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae sint fuga et ab perspiciatis dicta illo aspernatur exercitationem totam iure! Itaque accusamus possimus, porro facilis repudiandae ad fuga eos laborum.</span>
            </div>
            <div class="tip">
                <form action="">
                    <input type="text" name="" id="" placeholder="Have helpful info to help find them?">

                </form>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
.holder{
    height: 100vh;
    width: 100%;
    display: flex;
}
.image{
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: var(--amberalert-green);
}
.text{
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
}
.name{
    height: 20%;
}
.details{
    height: 50%;
}
.tip{
    height: 30%;
}
</style>