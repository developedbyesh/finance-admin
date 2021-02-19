<template>
    <Layout>
        <b-row class="d-flex flex-row align-items-start justify-content-between w-100 body-container" no-gutters> 
            <b-col cols="12" lg="6" class="d-flex flex-column align-items-center justify-content-center logo-container">
                <b-img></b-img>
            </b-col>
            <b-col cols="12" lg="6" class="d-flex flex-column align-items-center justify-content-center inner-container">
                <slot></slot>
            </b-col>
        </b-row>
    </Layout>
</template>

<script>
import Layout from "@/layout/Layout";
export default {
    components: {
        Layout
    }    
}
</script>

<style scoped>
.body-container {
    min-height: 600px;
    height: 100vh;
}
.body-container .logo-container {
    height: 100vh;
    background-color: aqua;
}
.body-container .inner-container {
    height: 100vh;
    background-color: azure;
}

/* medium devices  */
@media (max-width: 991.98px) {
    .body-container .logo-container {
    height: 25vh;
    overflow: hidden;
}
.body-container .inner-container {
    height: 75vh;
}

/* extra small devices  */
@media (max-width: 575.98px) {
    .body-container .logo-container {
    height: 20vh;
}
}
.body-container .inner-container {
    height: 80vh;
}
}
</style>