<template>
    <div> Country:{{ country }} <br> CapitalCity:{{ capitalCity }} <br> Langauge:{{ language }} </div>
</template>
<script>
    export default {
        props: ["country" , "capitalCity", "language"]

    }
</script>