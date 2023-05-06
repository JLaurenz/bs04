<script setup>
import { ref } from 'vue';

defineProps({
    msg: String,
})

const count = ref(0)
</script>
    
<template>
    <div class="student-dashboard mt-5">
        <div class="student-dashboard-icon primary-bg">
            <span><i class="fa fa-graduation-cap"></i></span>
        </div>
        <h3 class="mb-3">Student Dashboard</h3>
        <div class="d-grid">
            <a href="" class="btn primary-bg">Profile</a>
            <a href="" class="btn primary-bg">Thesis Consultation</a>
            <a href="" class="btn primary-bg">Appoinrment Schedule</a>
        </div>
    </div>
</template>

<style scoped>
    .primary-bg {
        background-color: #5891ff;
    }
    .student-dashboard{
        background-color: #fff;
        max-width: 100%;
        margin: auto;
        padding: 50px 70px;
        border-radius: 30px;
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.075);
    }

    .student-dashboard .student-dashboard-icon{
        text-align: center;
        border-radius: 50%;
        font-size: 40px;
        color: white;
        width: 100px;
        height: 100px;
        margin: auto;
        margin-bottom: 50px;
        line-height: 100px;
    }

    .student-dashboard a{
        border-radius: 30px;
        padding: 10px 20px;
        font-size: 18px;
        font-weight: bold;
        border: none;
        color: white;
        margin-top: 20px;
    }

    a:hover{
        background-color: #1F69FF;
    }
</style>