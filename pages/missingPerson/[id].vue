<template>
    <BackComponent></BackComponent>
    <div class="holder">
        <div class="left">
            <div class="image">
                <img src="" alt="">
            </div>            
        </div>

        <div class="right">
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
.left{
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

}
.image{
    width: 90%;
    height: 90%;
    border-radius: 20px;
    background-color: var(--amberalert-green);    
}
.right{
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 40px;
}
.text{
    height: 100%;
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