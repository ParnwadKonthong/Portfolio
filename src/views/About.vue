<script setup lang="ts">
import SkillItem from '../components/SkillItem.vue';
</script>

<template>
  <div class="flex flex-col items-center justify-center mt-10">
    <div class="font-bold text-4xl mb-12">ABOUT ME</div>

    <div class="flex flex-col items-center lg:flex-row lg:justify-between">
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
            <div class="w-[450px] p-6 border border-gray-300 rounded-xl shadow-md bg-white/72 text-center mb-4 lg:text-center">
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
        <SkillItem icon="../public/logo-skill/logo-html.png" name="HTML" />
        <SkillItem icon="../public/logo-skill/logo-CSS.png" name="CSS" />
        <SkillItem icon="../public/logo-skill/logo-javascript.png" name="JavaScript" />
        <SkillItem icon="../public/logo-skill/logo-typescript.png" name="TypeScript" />
        <SkillItem icon="../public/logo-skill/logo-python.png" name="Python" />
        <SkillItem icon="../public/logo-skill/logo-tailwind.png" name="Tailwind" />
        <SkillItem icon="../public/logo-skill/logo-bootstrap.png" name="bootstrap" />
        <SkillItem icon="../public/logo-skill/logo-quasar.png" name="Quasar" />
        <SkillItem icon="../public/logo-skill/logo-vuejs.png" name="Vue.js" />
        <SkillItem icon="../public/logo-skill/logo-react.png" name="React" />
        <SkillItem icon="../public/logo-skill/logo-nodejs.png" name="Node.js" />
        <SkillItem icon="../public/logo-skill/logo-mongodb.png" name="MongoDB" />
        <SkillItem icon="../public/logo-skill/logo-vscode.png" name="VS Code" />
        <SkillItem icon="../public/logo-skill/logo-figma.png" name="Figma" />
        <SkillItem icon="../public/logo-skill/logo-canva.png" name="Canva" />
        <SkillItem icon="../public/logo-skill/logo-microsoftoffice.png" name="Microsoft office" />
    </div>
  </div>
</template>
