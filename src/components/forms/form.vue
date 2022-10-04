<template>
    <div class="container">
        <form action="">
            <label for="">Name</label>
            <input type="text" v-model="name"/>

            <label for="">Email</label>
            <input type="email"  v-model="email"/>

            <label >Role</label>
            <select v-model="role" >
                <option value="developer">Mobile Developer</option>
                <option value="designer">Web Designer</option>
            </select>

            <div class="terms">
                <input type="checkbox" require v-model="terms" />
                <label for="">accept terms and conditions</label>
            </div>

            <label >Select names</label>
            <div class="terms">
                <label for="">Eric</label>
                <input type="checkbox" value="Eric" require v-model="names" />
            </div>
            <div class="terms">
                <label for="">Ten</label>
                <input type="checkbox" value="Ten" require v-model="names" />
            </div>
            <div class="terms">
                <label for="">Hag</label>
                <input type="checkbox" require value="Hag" v-model="names" />
            </div>



            <button type="submit">Submit</button>
        </form>
        <p>Name: {{name}} </p>
        <p>Email: {{email}}</p>
        <p>Role: {{role}}</p>
        <p>Terms: {{terms ? "accepted" :"not accepted"}}</p>
        <p>Names: {{names}}</p>
    </div>
   
</template>

<script>
    export default{
        name:"MyForm",
        data(){
            return{
                email:"",
                name:"",
                role:"designer",
                terms:false,
                names:[]
            }
        }
    }
</script>

<style scoped>
    form{
        background-color: white;
        border-radius: 10px;
        padding: 30px;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        text-align: left;
        width: 40%;
        min-width: 500px;   
    }

    label{
        margin-top: 10px;
        font-size: 16px;
        font-weight: 600;
        color: rgb(187, 184, 184);
        
    }
    select,input{
        /* outline: none; */
        outline-color: rgb(163, 160, 160);
        border: none;
        border-bottom: 1px rgb(179, 175, 175) solid;
        padding: 10px;
        color: gray;
    }

    button{
        border: none;
        background-color: gray;
        color: white;
        width: 100%;
        margin-top: 30px;
        font-size: 15px;
        border-radius: 8px;
        padding: 5px;
    }
    .terms{
        display: inline-block;
        margin-top: 20px;
    }
</style>