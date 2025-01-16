<template>
    <div class="headerHolder">
        <div class="top">
            <NuxtLink to="/" class="logo">
                <span>Amber Alert Ke</span>
            </NuxtLink>
            <div class="user">
                <NuxtLink to="/notification" class="notification">
                    <UIcon name="i-ic:baseline-notifications" class="icon"/>
                </NuxtLink>
                <NuxtLink to="/signUp" class="profile">
                    <UIcon name="i-ic:baseline-person" class="icon"/>
                </NuxtLink>
            </div>
        </div>

        <div class="bottom">
            <div class="search">
                <input 
                    type="text" 
                    v-model="searchQuery" 
                    placeholder="Search for a person..." 
                    class="searchBar"
                />
            </div>
            <div class="filter">
                <UIcon name="i-ic:baseline-filter-list" class="icon"/>
                <span class="normalText">filter</span>
            </div>

            <div class="sort">
                <UIcon name="i-ic:sharp-import-export"class="icon"/>
                <span class="normalText">sort</span> 
            </div>

        </div>
    </div>

</template>

<script setup>

const searchQuery = ref('');
</script>

<style scoped>
.headerHolder{
    width: 100%;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 5px;
    padding-bottom: 10px;
    display: flex;
    flex-direction: column;
    position: fixed;
    background-color: var(--amberalert-white);
    top: 0;
    z-index: 3;
    /* box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.4); */
}
.top{
    height: 50px;
    margin-bottom: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* background-color: blueviolet; */
}
.user{
    display: flex;
    justify-content: space-around;
    align-items: center;
}
.notification{
    display: flex;
}
.notification >*{
    margin-left: 5px;
    margin-right: 5px;
}
.profile{
    display: flex;
}
.profile >*{
    margin-left: 5px;
    margin-right: 5px;
}

.bottom{
    display: flex;
    align-items: center;
}
.bottom >*{
    display: flex;
    align-items: center;
    margin-left: 10px;
    margin-right: 10px;
}
.search{
    width: 30%;
}

</style>