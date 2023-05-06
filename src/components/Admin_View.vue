<script setup>
import { ref } from 'vue';

defineProps({
    msg: String,
})

const count = ref(0)
</script>
    
<template>
    <div class="admin-view mt-5">
        <h3 class="mb-4">Welcome (name of Admin)</h3>
        <div class="row align-items-center">
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <input type="text" class="form-control" id="student_name" value="Name of the student" disabled>
                </div>
            </div>
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <input type="text" class="form-control" id="year_section" value="Year and Section" disabled>
                </div>
            </div>
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <input type="text" class="form-control" id="student_name" value="Group code" disabled>
                </div>
            </div>
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <input type="text" class="form-control" id="student_name" value="School ID number" disabled>
                </div>
            </div>
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <div class="d-grid">
                        <a href="" class="btn primary-bg">Edit Information</a>
                        <a href="" class="btn primary-bg">Return Information</a>
                    </div>
                </div>
            </div>
            <div class="col-md-6 pb-4">
                <div class="mb-3">
                    <div class="d-grid">
                        <a href="" class="btn primary-bg">Delete Information</a>
                        <a href="" class="btn primary-bg">Search Information</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .primary-bg {
        background-color: #5891ff;
    }
    .admin-view{
        background-color: #fff;
        max-width: 100%;
        margin: auto;
        padding: 50px 70px;
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.075);
    }

    .admin-view input{
        font-size: 18px;
    }

    .admin-view *:disabled{
        border: none;
        background-color: #fff;
        border-bottom: #5891ff 2px solid;
        border-radius: 0;
    }

    .admin-view a{
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