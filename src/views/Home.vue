<template>
  <div class="flex flex-col items-center justify-center mt-20">
    <div class="text-center">
      <div class="text-3xl">Hello, I'm</div>
      <div class="font-bold text-6xl mt-4">PARNWAD KONTHONG</div>
    </div>
    <div class="flex justify-center gap-4 mt-12">
      <a
        href="https://github.com/ParnwadKonthong"
        target="_blank"
        rel="noopener noreferrer"
      >
        <button class="btn btn-color flex justify-center items-center gap-2">
          View My GitHub
          <img src="/icon-external-link.png" alt="External lim=nk icon" class="w-5 h-5"/>
        </button>
      </a>
      <a
        href="/Resume_Parnwad.pdf"
        download="Resume_Parnwad.pdf"
        rel="noopener noreferrer"
      >
        <button class="btn btn-color flex justify-center items-center gap-2">
          Download Resume
          <img src="/icon-download.png" alt="Download icon" class="w-5 h-5"/>
        </button>
      </a>
    </div>

    <div class="mt-10">
      <img src="../assets/img-home.png" />
    </div>
  </div>
</template>

<style scoped>
.btn {
  padding: 0.5rem 1.5rem;
  font-weight: 600;
  border-radius: 9999px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  cursor: pointer;
}

.btn:hover {
  opacity: 0.9;
  font-weight: 700;
}
.btn-color {
  margin: 0;
  background: linear-gradient(135deg, #ff9db4, #ffd793);
}
</style>
