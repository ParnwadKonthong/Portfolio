<script setup lang="ts">
import SkillItem from '../components/SkillItem.vue';
</script>

<template>
    <div class="flex flex-col items-center justify-center mt-10 mb-40">
        <div class="font-bold text-4xl mb-12">CONTACT ME</div>

        <div class="flex flex-wrap justify-center gap-4">
            <SkillItem icon="../public/logo-mail.png" name="Parnwad.konthong@gmail.com" />
            <SkillItem icon="../public/logo-github.png" name="ParnwadKonthong" />
            <SkillItem icon="../public/logo-phone.png" name="097-072-6523" />
        </div>
        
    </div>
</template>