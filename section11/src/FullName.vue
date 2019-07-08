<template>
    <div>
        <div class="form-group">
            <label>First Name</label>
            <input type="text" class="form-control" :value="firstName">
        </div>
        <div class="form-group">
            <label>Last Name</label>
            <input type="text" class="form-control" :value="lastName">
        </div>
    </div>
    
</template>

<script>
export default {
    props: ['value'], 
    methods: {

    }, 
    computed: {
        firstName() {
            return this.value.split(" ")[0];
        }, 
        lastName() {
            return this.value.split(" ")[1];
        }
    }
    
}

</script>
