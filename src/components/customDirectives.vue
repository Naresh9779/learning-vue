<script setup>
const vFormatDiv={

    mounted:(el,binding)=>{

        el.style.fontSize=binding.value +'px';
        el.style.color='red';
        // el.style.border="1px solid green"
        console.log(binding.value)

    //     switch(binding.arg)
    //    { case 'red':
    //    el.style.color='red';
    //    break;

    //    case 'orange':
    //    el.style.color='orange';
    
    
    // }

    }


}


</script>



<template>
  <!-- <div v-format-div:orange>My World</div> -->
  <div v-format-div="100">My World 1</div>
</template>