<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import TheWelcome from "./components/TheWelcome.vue";
import CustomTemplate from "./components/CustomTemplate.vue"
import ListRendering from "./components/ListRendering.vue";
import ComputedProperty from "./components/ComputedProperty.vue";
import LifecycleAndTemplateRefs from "./components/LifecycleAndTemplateRefs.vue";
import Watchers from "./components/Watchers.vue";
import ChildComponentWithProps from "./components/ChildComponentWithProps.vue";
import ChildComponentWithEmits from "./components/ChildComponentWithEmits.vue";
import { ref } from "@vue/reactivity";
import Slots from "./components/Slots.vue";

const childMsg = ref("No msg from child");
</script>

<template>

  <Slots><h1>This is from parent</h1></Slots>
  
  
  <!-- Child component with emits -->
  <!-- <ChildComponentWithEmits @response="(msg)=>childMsg = msg"/>
  <p>{{ childMsg }}</p> -->

  <!-- Child component with props -->
  <!-- <ChildComponentWithProps msg="Hello World"/> -->
  <!-- <header>
    <img
      alt="Vue logo"
      class="logo"
      src="./assets/logo.svg"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
      <CustomTemplate /> 
    </div>
  </header>

  <main>
    <TheWelcome />
  </main> -->
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
