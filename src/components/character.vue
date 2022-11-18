<template>
    <div>
        
        <h1>Profile</h1>
        <div>
            <div class="BD">
                
                <br>
               <img :src="character.thumbnail.path+'.'+character.thumbnail.extension" alt="character.name">
            </div>
            <div class="BD2">
                <div class="BD2">
                    <h3 class="link">{{character.name}}</h3>
                <ul>
                    <li>ID: {{character.id}}</li>
                <li><span class="green" id="status" v-if="character.status=='Alive'"></span> 
                    <span class="red" id="status" v-else-if="character.status=='Dead'"></span>
                    <span class="blue" id="status" v-if="character.status=='unknown'"></span>
                    Modified: {{character.modified}}</li>
                <li>Description: {{character.description}}</li>


                <li>Series: {{character.series.available}}</li>
                <!-- <li>No. Episodes: {{character.episode.length}}</li> -->
                <li>Comics: {{character.comics.available}}</li>
                <li>Stories: {{character.stories.available}}</li>
                <li>Events: {{character.stories.available}}</li>
            </ul>
                </div>
                
            </div>
        </div>
    </div>
    </template>
    <script>
    export default {
        name: 'character',
        data(){
            return{
                character: {},
            }
        },
        methods:{
            callingAPI(link){
                fetch(link).then(res=>res.json().then((json)=>{
                    this.character=json.data.results[0] 
                    console.log(json.data.results[0])
                }))
            }
        },
          openCharacterSeries(se){
            this.$router.push(`/series/${id}`)
            this.$router.push({path:'/series',params:{se:se}})
            this.$router.push({name:'series',params:{se:se}})
          },
          openCharacterComics(co){
            this.$router.push(`/comics/${id}`)
            this.$router.push({path:'/comics',params:{co:co}})
            this.$router.push({name:'comics',params:{co:co}})
          },
          openCharacterStories(st){
            this.$router.push(`/stories/${id}`)
            this.$router.push({path:'/stories',params:{st:st}})
            this.$router.push({name:'stories',params:{st:st}})
          },
          openCharacterEvents(ev){
            this.$router.push(`/events/${ev}`)
            this.$router.push({path:'/events',params:{ev:ev}})
            this.$router.push({name:'events',params:{ev:ev}})
          },
        mounted(){
            this.callingAPI(`https://gateway.marvel.com/v1/public/characters/${this.$route.params.id}?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=0`)
        }
        
    }
    </script>
    <style scoped>
    body{
        background-color:rgb(172, 58, 58)
    }
    h1{color: rgb(241, 241, 243);}
    div{
        display: inline-block;
        justify-content: left;
        background-color: black;
        color: gold;
        margin-bottom: 10px;
    }
    .BD{
        display: flex;
        background-color: rgb(68, 72, 72);
        border-radius: 5px;
        color: rgb(21, 21, 20);
    }
    .BD2{
        display: flex;
        flex-direction: column;
        background-color: rgb(83, 76, 76);
        border-radius: 5px;
        color: gold;
        margin-left: 5px;
        margin-right: 5px;
    }
    .link:hover{
        color:gold
    }
    .nextButton{
        background-color: rgb(83,76,76);
        border-radius: 30%;
        color: white;
        
    }
    
    button{padding: 1%;}
    button:hover{color: gold}
    #status{
        height: 10px;
        width: 10px;
        border-radius: 50%;
        display: inline-block;
    }
    .green{
        background-color: green;
    }
    .red{
        background-color: red;
    }
    .blue{
        background-color: blue;
    }
    div>ul{
        margin-bottom: 0px;
        margin-top: 0px;
        list-style: none;
        padding: 0px;
    }
    div>img{
        margin-left: 10px;
        margin-right: 10px;
        justify-content: left;
    }
    div>h3{
        color: aliceblue;
    }
    </style>