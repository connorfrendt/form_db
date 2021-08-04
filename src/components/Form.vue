<template>
    <form @submit.prevent="asdf">
        <div>
            <label>
                Name:
                <input v-model="info.name" type="textbox">
            </label>
        </div>

        <div>
            <label>
                Email:
                <input v-model="info.email" type="textbox">
            </label>
        </div>

        <div>
            <label>
                Username:
                <input v-model="info.username" type="textbox">
            </label>
        </div>

        <button>SUBMIT</button>

    </form>
</template>

<script>
export default {
    data() {
        return {
            info: {
                name: '',
                email: '',
                username: ''
            }
        }
    },
    methods: {
        asdf() {
            console.log('Name: ', this.info.name,`\n`, 'Email: ', this.info.email,`\n`, 'Username: ', this.info.username);
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>