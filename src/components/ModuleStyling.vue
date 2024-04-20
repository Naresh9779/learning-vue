<template>
    <!-- <h1 :class="$style['my-power']"> I Am Back With New Powerr</h1> -->

    <h1 :class="myclass.anotherpower"> I Am Back With New Powerr</h1>
</template>

<style module="myclass">
.my-power{
    background-color: yellow;
    color: aqua;
}

.anotherpower{
    background-color: red;
    color: white;
}

</style>