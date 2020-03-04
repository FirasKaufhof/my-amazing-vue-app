<template>
  <div id="app">
    <div class="welcome">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Amazing Vue App"/>
    </div>
    <div class="pattern-library-content">
    <MyButton :isDisabled="false" label="Hello 1st npm package"></MyButton>

    <List tag="ol" type="A">
        <ListItem tag="li" text="I am the first item.">
        </ListItem>
        <ListItem tag="li" text="I am the second item.">
        </ListItem>
        <ListItem tag="li" text="I am the third item.">
        </ListItem>
    </List>
    <Badge status="warning"></Badge>
    <CustomerCard />
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Components from '@galeria-demo/my-amazing-storybook-app'

export default {
  name: 'app',
  components: {
    HelloWorld,
    ...Components
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  text-align: center;
}

.pattern-library-content {
list-style: inside;
}
</style>
