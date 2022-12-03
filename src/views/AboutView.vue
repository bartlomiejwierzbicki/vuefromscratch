<template>
  <div class="about">
    <h1>This is an about page</h1>
    <QuoteItem />
  </div>
</template>

<script>
import QuoteItem from "@/components/Quote.vue";
// import ButtonItem from "@/components/Button.vue"
export default {
  components: {
    // ButtonItem,
    QuoteItem
  }
}
</script>
