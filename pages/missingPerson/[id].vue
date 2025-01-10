<template>
    <div class="holder">
        <div class="image">
            <img src="" alt="">
        </div>
        <div class="text">
            <div class="name">
                <span class="mediumText">Name</span>
                <span class="normalText">Age: Gender: </span>
            </div>
            <div class="details">
                <span class="normalText">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae sint fuga et ab perspiciatis dicta illo aspernatur exercitationem totam iure! Itaque accusamus possimus, porro facilis repudiandae ad fuga eos laborum.</span>
            </div>
            <div class="tip">
                <form action="">
                    <textarea 
                        id="messageBox" 
                        placeholder="Have helpful info to help find them?" 
                        maxlength="250"
                        class="large-textarea"
                    ></textarea>

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
    align-items: start;
    padding: 20px;
}
.name{
    height: 20%;
    display: flex;
    flex-direction: column;
}
.details{
    height: 50%;
}
.tip{
    height: 30%;
}
</style>