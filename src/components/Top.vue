<template>
<header class="top">
    <h1>{{ top.title }}</h1>
    <p class="card-type">{{ top.type }}</p>
    </header>
</template>
<script>
export default {
    name: 'Top',
    props: {
        top: Object
    }
    
}
</script>