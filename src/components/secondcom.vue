<template>
    <div>My name is {{ name }} <br>
        My Father name is {{ fathername }} <br>
        My CNIC is {{ CNIC }}
    </div>
</template>

<script>
    export default{
        props:['name' , 'fathername' , 'CNIC']
    }
</script>