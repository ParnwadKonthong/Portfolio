<script setup lang="ts">
import SkillItem from '../components/SkillItem.vue';
</script>

<template>
  <div class="flex flex-col items-center justify-center mt-10">
    <div class="font-bold text-4xl mb-12">ABOUT ME</div>

    <div class="flex flex-col items-center lg:flex-row lg:justify-between w-full">
        <!-- Introduction -->
        <div class="mr-4">
            <div class="font-bold text-2xl mb-4">PARNWAD KONTHONG</div>
            <div class="text-base indent-20 mb-4">I am eager to apply the knowledge and skills gained during my 4 years of study in Computer Science at the
                Faculty of Information Technology and Innovation, Bangkok University, to contribute value and innovation to
                your company. I am excited about the opportunity to work in a related position, expand my understanding of
                technology, and gain practical experience that will enable me to grow alongside your organization.</div>
        </div>
        <!-- Education -->
        <div>
            <div class="w-auto p-6 border border-gray-300 rounded-xl shadow-md bg-white/72 text-center mb-4 lg:text-center lg:w-[450px]">
                <div class="font-bold text-2xl mb-4">EDUCATION</div>
                <div class="text-base">
                    <div>BANGKOK UNIVERSITY 2020 - 2024</div>
                    <div>Bachelor of Information Technology and Innovation</div>
                    <div>Major Computer Science</div>
                    <div>GPAX 3.51</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Skill -->
    <div class="flex flex-wrap justify-center gap-4">
        <SkillItem icon="../logo-html.png" name="HTML" />
        <SkillItem icon="../logo-css.png" name="CSS" />
        <SkillItem icon="../logo-javascript.png" name="JavaScript" />
        <SkillItem icon="../logo-typescript.png" name="TypeScript" />
        <SkillItem icon="../logo-tailwind.png" name="Tailwind" />
        <SkillItem icon="../logo-bootstrap.png" name="bootstrap" />
        <SkillItem icon="../logo-vuejs.png" name="Vue.js" />
        <SkillItem icon="../logo-react.png" name="React" />
        <SkillItem icon="../logo-nodejs.png" name="Node.js" />
        <SkillItem icon="../logo-mongodb.png" name="MongoDB" />
        <SkillItem icon="../logo-vscode.png" name="VS Code" />
        <SkillItem icon="../logo-github.png" name="VS Code" />
        <SkillItem icon="../logo-figma.png" name="Figma" />
        <SkillItem icon="../logo-canva.png" name="Canva" />
        <SkillItem icon="../logo-postman.png" name="Postman" />
        <SkillItem name="Manual Testing" />
        <SkillItem name="Test Case" />
        <SkillItem name="Bug Report" />
        <SkillItem name="API/UI Testing" />
    </div>
  </div>
</template>
