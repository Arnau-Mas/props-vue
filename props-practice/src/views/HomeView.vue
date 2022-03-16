<template>
  <div class="home">
    <div v-for="card in cards" :key="card.title">
      <Card :title="card.title" :content="card.content" :buttonText="buttonContent">
      <h2>Subtitle</h2>
      </Card>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/Card.vue'

export default {
  name: 'HomeView',
  data(){
    return{
      cards:[{
        title: "Card 1",
        content: "Card 1 content dolor sit amet consectetur, adipisicing elit. Voluptatibus qui repellat aperiam quam impedit vel necessitatibus reiciendis, consectetur, ea nihil nobis a soluta eveniet maxime doloribus? Maiores temporibus totam culpa."
      },
      {
        title: "Card 2",
        content: "Card 2 content dolor sit amet consectetur, adipisicing elit. Voluptatibus qui repellat aperiam quam impedit vel necessitatibus reiciendis, consectetur, ea nihil nobis a soluta eveniet maxime doloribus? Maiores temporibus totam culpa."
      },
      {
        title: "Card 3",
        content: "Card 3 content dolor sit amet consectetur, adipisicing elit. Voluptatibus qui repellat aperiam quam impedit vel necessitatibus reiciendis, consectetur, ea nihil nobis a soluta eveniet maxime doloribus? Maiores temporibus totam culpa."
      }],
      buttonContent:"Click"
    }
  },
  components: {
    Card
  }
}
</script>

<style>
  .home{
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>