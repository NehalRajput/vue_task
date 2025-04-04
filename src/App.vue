<!----<script setup>
import { ref } from 'vue';

const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <div>
    <p>Count: {{ count }}</p>
    <button @click="increment">Increase</button>
  </div>
</template>
-->
<!-----<script setup>
   const msg = "Hello";
</script>

<template>
   <p style="color: blue; font-size: larger;">{{ msg }}</p>  
</template>
-->

<!---
<script setup>
import { ref } from 'vue';

const message = ref("<b>Hello</b> <br> <p>world</p>");
</script>

<template>
  <div>
    <p v-html="message"></p>

    <span style="color: blueviolet;">Hello</span>
  </div>
</template>

-->
<!---
<script setup>
import { ref } from 'vue';

const textColor = ref("pink");
const dynamicId = ref("white");
const isButtonDisabled = true;

</script>


<template>
  <button :disabled="isButtonDisabled">Button</button>
  <div v-bind:id="dynamicId" style="font-size: large;">this is binding the id</div>
  <p :style="{ color: textColor, fontSize: '25px'}">Dynamic Style Example</p>
</template>
-->
<!---
<script setup>
import { ref } from 'vue';

const message = ref("Hello!");

function changeText() {
  message.value = "Text Changed!";
}
</script>


<template>
  <div>
    <p>{{ message }}</p>
    <button @click="changeText">Click Me</button>
  </div>
</template>

-->
<!---
Reactivity Using ref()
The ref() function creates reactive variables in Vue.

<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <button @click="increment">
    {{ count }}
  </button>
</template>
-->

<!---
<script setup>
import { ref } from 'vue'

const obj = ref({
  nested: { count: 0 },
  arr: ['foo', 'bar']
})

function mutateDeeply() {
  obj.value.nested.count++ 
  obj.value.arr.push('baz')
}
</script>
<template>
  <div>

    <p>Count: {{ obj.nested.count }}</p>
    <p>Array: {{ obj.arr }}</p>
    <button @click="mutateDeeply">Update</button>
  </div>
</template>
-->

<!---
<script setup>

const awesome = true;                               

</script>
<template>

<h1 v-if="awesome">Vue is awesome!</h1>
</template>
-->
<script setup>

import {ref} from 'vue'
const items = ref([{ message: 'Foo' }, { message: 'Bar' }])
</script>

<template>

  <li v-for="item in items">
  {{ item.message }}
</li>
</template>