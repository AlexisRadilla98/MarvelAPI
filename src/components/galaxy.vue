<template>
    <div> 
        <div>
        <h1> Heroes and Villians </h1>
        <input type="text" v-model="input">
        <ul>
            
            <li v-for="(name, index) in filteredNames" v-bind:key="index">
                <router-link :to="{name: 'character', params:{id: name.id}}"><h3 class="link">{{name.name}}</h3><img :src="name.path+'.'+name.ext" alt=""></router-link>
            </li>
        
        </ul>
        <h1>{{names.length}}</h1>
        </div>
        <div class="pictures">
        <div  v-for="person1 in persons1.results" :key="person1.id">
            <div v-if="person1.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person1.id}}"><h3 class="link">{{person1.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person1.thumbnail.path+'.'+person1.thumbnail.extension" alt="person.name">
                <h4>{{person1.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person2 in persons2.results" :key="person2.id">
            <div v-if="person2.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person2.id}}"><h3 class="link">{{person2.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person2.thumbnail.path+'.'+person2.thumbnail.extension" alt="person.name">
                <h4>{{person2.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person3 in persons3.results" :key="person3.id">
            <div v-if="person3.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person3.id}}"><h3 class="link">{{person3.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person3.thumbnail.path+'.'+person3.thumbnail.extension" alt="person.name">
                <h4>{{person3.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person4 in persons4.results" :key="person4.id">
            <div v-if="person4.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person4.id}}"><h3 class="link">{{person4.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person4.thumbnail.path+'.'+person4.thumbnail.extension" alt="person.name">
                <h4>{{person4.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person5 in persons5.results" :key="person5.id">
            <div v-if="person5.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person5.id}}"><h3 class="link">{{person5.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person5.thumbnail.path+'.'+person5.thumbnail.extension" alt="person.name">
                <h4>{{person5.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person6 in persons6.results" :key="person6.id">
            <div v-if="person6.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person6.id}}"><h3 class="link">{{person6.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person6.thumbnail.path+'.'+person6.thumbnail.extension" alt="person.name">
                <h4>{{person6.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person7 in persons7.results" :key="person7.id">
            <div v-if="person7.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person7.id}}"><h3 class="link">{{person7.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person7.thumbnail.path+'.'+person7.thumbnail.extension" alt="person.name">
                <h4>{{person7.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person8 in persons8.results" :key="person8.id">
            <div v-if="person8.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person8.id}}"><h3 class="link">{{person8.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person8.thumbnail.path+'.'+person8.thumbnail.extension" alt="person.name">
                <h4>{{person8.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person9 in persons9.results" :key="person9.id">
            <div v-if="person9.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person9.id}}"><h3 class="link">{{person9.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person9.thumbnail.path+'.'+person9.thumbnail.extension" alt="person.name">
                <h4>{{person9.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person10 in persons10.results" :key="person10.id">
            <div v-if="person10.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person10.id}}"><h3 class="link">{{person10.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person10.thumbnail.path+'.'+person10.thumbnail.extension" alt="person.name">
                <h4>{{person10.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person11 in persons11.results" :key="person11.id">
            <div v-if="person11.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person11.id}}"><h3 class="link">{{person11.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person11.thumbnail.path+'.'+person11.thumbnail.extension" alt="person.name">
                <h4>{{person11.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person12 in persons12.results" :key="person12.id">
            <div v-if="person12.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person12.id}}"><h3 class="link">{{person12.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person12.thumbnail.path+'.'+person12.thumbnail.extension" alt="person.name">
                <h4>{{person12.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person13 in persons13.results" :key="person13.id">
            <div v-if="person13.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person13.id}}"><h3 class="link">{{person13.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person13.thumbnail.path+'.'+person13.thumbnail.extension" alt="person.name">
                <h4>{{person13.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person14 in persons14.results" :key="person14.id">
            <div v-if="person14.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person14.id}}"><h3 class="link">{{person14.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person14.thumbnail.path+'.'+person14.thumbnail.extension" alt="person.name">
                <h4>{{person14.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person15 in persons15.results" :key="person15.id">
            <div v-if="person15.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person15.id}}"><h3 class="link">{{person15.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person15.thumbnail.path+'.'+person15.thumbnail.extension" alt="person.name">
                <h4>{{person15.id}}</h4>
            </div>
            
        </div>
        <div  v-for="person16 in persons16.results" :key="person16.id">
            <div v-if="person16.thumbnail.path!='http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available'">
                <router-link :to="{name: 'character', params:{id: person16.id}}"><h3 class="link">{{person16.name}}</h3></router-link>
                <!--<h1 id="nombre">{{person.name}}</h1> -->
                <img :src="person16.thumbnail.path+'.'+person16.thumbnail.extension" alt="person.name">
                <h4>{{person16.id}}</h4>
            </div>
            
        </div>
        </div>
        
          
        <h1>
      {{ msg }}
        </h1>
        <p>
      <button class="nextButton" @click="callingAPI(url,offset,true)" id="NB" v-if="next!=null">NEXT</button>
      <button class="nextButton"  id="PB" @click="callingAPI(url,offset,false)" v-if="prev!=null">PREV</button>
      </p>
    </div>
    </template>
<script>
  export default {
      name: 'galaxy',
      props: {
      msg: String
      },
      data(){
          return{
              persons:[],
              persons1:[],
              persons2:[],
              persons3:[],
              persons4:[],
              persons5:[],
              persons6:[],
              persons7:[],
              persons8:[],
              persons9:[],
              persons10:[],
              persons11:[],
              persons12:[],
              persons13:[],
              persons14:[],
              persons15:[],
              persons16:[],
              next:'',
              previous:'',
              input:'',
              names:[],
              url:'https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=',
              next:1,
              prev:null,
              offset:100
          }
      },
      methods:{
          //todo(){this.persons=this.persons1.results.concat(this.persons2.results,this.persons3.results,this.persons4.results,this.persons5.results,this.persons6.results,this.persons7.results,this.persons8.results,this.persons9.results,this.persons10.results,this.persons11.results,this.persons12.results,this.persons13.results,this.persons14.results,this.persons15.results,this.persons16.results)},
          callingAPI1(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons1=json.data
                  for (let i = 0; i < 100; i++) {
                  this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                
                  } 
              }))
          },
          callingAPI2(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons2=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI3(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons3=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI4(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons4=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI5(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons5=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI6(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons6=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI7(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons7=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI8(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons8=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI9(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons9=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI10(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons10=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI11(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons11=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI12(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons12=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI13(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons13=json.data
                  for (let i = 0; i < 100; i++) {
                    this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI14(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons14=json.data
                  for (let i = 0; i < 100; i++) {
                  this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI15(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons15=json.data
                  for (let i = 0; i < 100; i++) {
                  this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          },
          callingAPI16(link){
              fetch(link).then(res=>res.json().then((json)=>{
                  this.persons16=json.data
                  for (let i = 0; i < 100; i++) {
                  this.names.push({name: json.data.results[i].name, id: json.data.results[i].id, path: json.data.results[i].thumbnail.path,ext: json.data.results[i].thumbnail.extension});
                  }
              }))
          }  
        },
          openCharacterId(id){
            this.$router.push(`/character/${id}`)
            this.$router.push({path:'/character',params:{id:id}})
            this.$router.push({name:'character',params:{id:id}})
          }
          
      ,//  https://rickandmortyapi.com/api/character   https://rickandmortyapi.com/api/character?page=2
      mounted(){
        //164eaff81b3a9bc2e5c3c85e70303775507a0a0614f3e5bfbccd06bf44405b26d11cafef2
          this.callingAPI1('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=0')
          this.callingAPI2('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=100')
          this.callingAPI3('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=200')
          this.callingAPI4('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=300')
          this.callingAPI5('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=400')
          this.callingAPI6('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=500')
          this.callingAPI7('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=600')
          this.callingAPI8('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=700')
          this.callingAPI9('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=800')
          this.callingAPI10('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=900')
          this.callingAPI11('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1000')
          this.callingAPI12('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1100')
          this.callingAPI13('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1200')
          this.callingAPI14('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1300')
          this.callingAPI15('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1400')
          this.callingAPI16('https://gateway.marvel.com/v1/public/characters?ts=1&apikey=4f3e5bfbccd06bf44405b26d11cafef2&hash=7e4f0355b8fab60646604d54058789e1&limit=100&offset=1500')
         // this.todo()
          //const button=document.getElementById('click',()=>this.callingAPI(this.next))   https://gateway.marvel.com:443
      },
      computed:{
    filteredNames(){
        console.log(this.names[0])
        return this.input !== ''? this.names.filter(name=>name.name.toLocaleLowerCase().includes(this.input.toLocaleLowerCase())):''
    }
  }
      
  }
  </script>
<style scoped>
.pictures{
    display:flex;
    flex-wrap: wrap;
    background-color: rgba(91, 77, 77, 0.132);
}
ul{ 
    display: flex;
    flex-wrap: wrap;
    list-style: none;justify-content: center;}
ul>li{font-style: normal; margin-right: 20px;}
a{
    color: black;
    background-color: rgba(0, 0, 0, 0.379);
}
a:hover{
    color: tomato;
}
h3{
    display:flex;
    justify-content: flex-start;}
h4{
    margin-top: 0%;
}
div{
    height: auto;
    margin: 10px;
    justify-content: center;
}
img{
    height: 30vh;
    width: 20vw;
}
</style>