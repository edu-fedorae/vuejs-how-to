<template>
    <div>
        <router-link to="/">
            <img alt="Vue logo" src="../assets/logo.png">
        </router-link>
        <form action="">
            <div>
                <input type="text" placeholder="Username">
                <br />
                <input type="password" placeholder="Password">
            </div>
            <div>
                <button>Login</button>
            </div>
        </form>
    </div>
</template>

<script>
import Login from "@/layouts/Login.vue"

export default {
    created() {
        this.$emit('update:layout', Login)
    }
}
</script>