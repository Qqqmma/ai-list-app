<template>
  <div id="app">
    <div class="bg-blue"><header-description-component class="container-1200"/></div>
    <ai-cards-list :data-base-emulator="DataBaseEmulator"/>
  </div>
</template>

<script>
import AiCardsList from '../components/AICardsList/AICardsList.vue';
import HeaderDescriptionComponent from '../components/HeaderModule/components/HeaderDescriptionComponent.vue';

export default {
  data() {
    return {
      DataBaseEmulator: [
        {
          idKey: 1,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 2,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 3,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 4,
          name: "testForSearch",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 5,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 6,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 7,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 8,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 9,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 10,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 11,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 12,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 13,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 14,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 15,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
        
        {
          idKey: 16,
          name: "chatGPT",
          logoAI: require("../assets/images/ai-img.jpg"),
          transformInfo: "Text to text",
          taskAI: "Генерация текста",
          scopesOfApplication: ["Копирайтинг", "Чат-бот", "Маркетинг"],
          description: "lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem lorem!",
          linkOnAI: "https://chat.openai.com/",
        },
      ]
    }
  },
  components: {
    AiCardsList,
    HeaderDescriptionComponent
  },
  methods: {
    searchInDataBase(inputValue) {
      let searchResult = [];
      for (let item of this.DataBaseEmulator){
        if (item.name.includes(inputValue)) searchResult.push(item);
      }
      
    }
  }
}
</script>


<style scoped>
.bg-blue{
  background-color: #a7e3ff;
}
</style>