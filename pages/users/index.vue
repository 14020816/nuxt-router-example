<template>
    <div>
        <v-list>
            <v-list-item v-for="item in 10" :key="item">
                <nuxt-link :to="'users/' + item">{{"User: " + item}}</nuxt-link>
            </v-list-item>
        </v-list>
    </div>
</template>

<script>
export default {
    
}
</script>