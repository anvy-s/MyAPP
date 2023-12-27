<script lang="ts">
 import {ref, reactive,onMounted } from "vue";
    export default{
        methods: {  
        searchFunc: async function() {
            console.log(this.search);
                if(this.search=='Dubai')
                {
                    
                    this.searchText=this.search;
                    this.searchText1="Unfortunately, this name is not available for registration. Please select another."
                    this.issue=true;
                }

            }
        },
        setup(){
            let searchText: string = "Company formation made easy";
            let search: string=""
            let searchText1: string = "Register a company, open a business bank account,and stay compliant - all in one place.";
            let searchIssue: string=""
            let searchIssueText: string=""
            let issue=ref(false);;
            return{
                searchText,
                searchText1,
                search,
                searchIssue,
                searchIssueText,
                issue
            }
        },
    }
</script>

<template>
  <div class="greetings">

    <placeholder style="align-items: center;">
        <h1 id="myDiv" v-if="!issue">{{ searchText }}</h1>
        <h1 id="myDiv" v-else>
            <img alt="Vue logo" style="align-items: center;text-align: center;" v-if="issue" src="@/assets/Error.png" width="50" height="50">
            <br/>
            {{ searchText }}</h1>
        <h4 id="myDiv2" v-if="!issue">{{ searchText1 }}</h4>
        <h4 id="myDiv2" v-else>{{ searchText1 }}</h4>
    </placeholder>

    
    

    <div class="search-box" style="padding-top: 5%;">
        <input 
        type="text" 
        class="search-bar" 
        placeholder="Find your perfect company Name..."
        v-model="search"
        style="align-items: center;font-size: larger;width: 500px;height: 50px;"
        />
        <button class="button"><a style="align-items: center;font-size: larger;" @click="searchFunc">Search</a></button>
        
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
  width: 100%;
  align-items: center;
  color: white;
}
.greetings h4 {
  text-align: center;
  color: white;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
}
.search-box{
  align-items: center;
  font-size: large;
  text-align: center;
}
.button {
  font-size: 18px;
  border-radius: 4px;
  background-color: #a9b502;
  color: white;
  cursor: pointer;
  border: 2px solid #a9b502;;
  height: 50px;
}
</style>
