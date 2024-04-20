<script setup>

import hello from './components/hello.vue';
import globalStyling from './components/globalStyling.vue';
import localStyling from './components/localStyling.vue';
import moduleStyling from './components/ModuleStyling.vue';
import myEvent from './components/myEvent.vue';
import reactiveComponent from './components/reactiveComponents.vue';
import refComponent from './components/refComponents.vue';
import computed from './components/computedProp.vue';
import conditionalRendering from './components/conditionalRendering.vue';
import itrationComponent from './components/itrationComponents.vue';
import vModel from './components/vModel.vue';
import prop from './components/props.vue';
import components from './components/component.vue';
import provideAndInject from './components/provideAndInject.vue';
import slots from './components/slots.vue'
import LifeCycleHooks from './components/LifeCycleComponents.vue';
import Watcher from './components/watchers.vue';
import reference from './components/reference.vue';
import friendList from './components/AsynchronousComponents.vue'
import composables from './components/composables.vue';
import customDirectives from './components/customDirectives.vue';
import dynamicComponents from './components/DynamicComponents.vue';
import fetchingData from './components/fatchingData.vue';
import {ref,defineAsyncComponent} from 'vue';
import {provide} from 'vue';


// const data={
//     name:['Naresh','Malu','Vinay'],
//     age:['20','21','22'],
//     gender:['Male','Female','Other']
// }
// const name='Pankaj';
//  const count=ref(0);

//  const userDetails=(name,email,password)=>{
//          console.log('Name',name);
//          console.log('Email',email);
//          console.log('Password',password);
// }

// provide('studentName','Naresh Thapa');
// provide('studentAge',21);
// provide('studentLoc',['Brampton','canada'])

// const show=ref(true);

let showFriend=ref(false);
const friendLists =defineAsyncComponent(()=>
              import('./components/AsynchronousComponents.vue')
        )
const toggleList=()=>{
        showFriend.value=!showFriend.value;
}
</script>

<template>
  <!-- <globalStyling/>
<localStyling/>
<moduleStyling/> -->
<!-- <myEvent/> -->
<!-- <reactiveComponent/> -->
<!-- <refComponent/> -->
<!-- <computed/> -->
<!-- <conditionalRendering/> -->

<!-- <itrationComponent/> -->
<!-- <vModel/> -->
 <!-- staticProp -->
               <!-- <prop name="nareshThapa"/> -->

<!-- DynaMIC prop -->

               <!-- <prop :firstName="firstName" :lastName="lastName"/> -->

<!--propValidation  -->
<!-- 
<prop :name="name"/> -->

<!-- <h1>count:{{ count }}</h1>
<components @incrementCounter="count++"/>                -->

<!-- <components @userInfo="userDetails"/> -->





                                          <!-- calling Slots -->
<!-- <slot>
<h1>helloWorld</h1>
</slot> -->
  
         <!-- FallBack  -->

<!-- <slots>
        <h1>i am Original</h1>

</slots> -->


<!-- <slots > -->


        <!-- <!-- <template #one></template>
        <!-- <template v-slot:two>
                <h1>I AM Slot One</h1> -->
        <!-- </template> -->

        <!-- <template #one>
                <h1> I am Slot Second</h1>
        </template>

        <template #default>
                 <h1>i am Default One</h1> 
                </template>
</slots>  -->

<!-- <provideAndInject/> -->


                    <!-- Life Cycle Hooks -->

<!-- <LifeCycleHooks v-if="show"/>

<button @click="show=!show">Show/hide</button> -->


                         <!-- Watchers -->

<!-- <Watcher/> -->



                            <!-- Template Reference -->
<!-- <reference/> -->



                             <!-- <!-- <!-- Asynchronous  -->

<!-- 
   <div v-if="showFriend">
       <friendLists/>
       
     </div>
     <button @click="toggleList"> Toggle Friend List</button> -->



                   <!-- composables -->

                   <!-- <composables/> -->

                   
              <!-- Custom Directives -->

              <!-- <customDirectives/> -->

              <!-- Dynamic components -->

              <!-- <dynamicComponents/> -->


          <!-- Fetching Data -->

          <fetchingData/>





</template>

