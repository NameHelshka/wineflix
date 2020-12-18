<template>
  <ResultItem :someProp="someState" />
  <Button @click="() => someState += 1"> Increment</Button>
</template>

<script>
import ResultItem from "@/ChildComponent"

export default {
  components: {
    ResultItem,
  },
  data() {
    return {
      someState: 1,
    }
  },
}
</script>

// ChildComponent.vue
<template>
  <p>{{ someProp }}</p>
</template>

<script>
export default {
  props: {
    someProp: Number,
  },
}
</script>
