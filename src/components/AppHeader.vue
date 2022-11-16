<script>
export default {
    name: 'AppHeader'
}
</script>


<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="/dc-logo.png" alt="logo">
            </div>
            
            <nav class="menu">
                    <ul>
                        <li
                        v-for="(link, index) in menu"
                        :key="index"
                        ><a 
                        :class="{'active': link.current}"
                        :href="link.href"
                        href="#">
                        {{link.text}}
                        </a></li>
                     </ul>
            </nav>
        </div>    
    </header>
</template>

<style lang="scss" scoped>

    ul {
        display: flex;
        li {
         list-style: none;
         margin: 10px; 
         a {
            text-decoration: none;
            color: black;
            font-weight: 600;
          }
        }
    }

</style>