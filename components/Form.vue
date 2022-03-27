<template>
    <div class="form">
        <b-form-group
            label-for="name"
        >
            <b-form-input
                id="name"
                v-model="form.name"
                type="text"
                placeholder="Seu nome"
                required
            />
        </b-form-group>

        <b-form-group
            label-for="idade"
        >
            <b-form-input
                id="idade"
                v-model="form.age"
                type="text"
                placeholder="Sua idade"
                required
            />
        </b-form-group>

        <b-button 
            type="submit" 
            variant="secondary"
            class="btn-submit"
            @click="onSubmit"
        >
            Confirmar
        </b-button>
        
        <b-button 
            type="reset" 
            variant="warning"
            @click="onReset"
        >
            Limpar
        </b-button>
    </div>
</template>
<script>
export default {
    data() {
        return {
            form: {
                name: '',
                age: '',
            }
        }
    },
    methods: {
        onSubmit() {
            console.log("On Submit")   
            this.form.name = ''
            this.form.age = '' 
        },
        onReset() {
            console.log("On reset")    
        }
    }
    
}
</script>

<style lang="css">
    .form {
        max-width: 80%;
        margin: 0 auto;
        text-align: center;
    }
    .btn-submit, .btn-submit:after {
        background-color: #333;
        outline: none;
    }
</style>