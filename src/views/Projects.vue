<template>
    <div class="flex flex-col items-center justify-center mt-10">
        <div class="font-bold text-4xl mb-12">MY PROJECTS</div>

        <div class="flex flex-col items-center lg:flex-row lg:justify-between gap-4">
            <div class="w-auto p-6 border border-gray-300 rounded-xl shadow-md bg-white/72 text-center mb-4 lg:text-center">
                <img src="../assets/kongsak_shop.png">
                <div class="font-bold text-2xl my-4">KONGSAK SHOP</div>
                <div class="flex justify-center gap-2">
                    <a href="https://github.com/ParnwadKonthong/kongsak-vue-frontend" target="_blank" rel="noopener noreferrer">
                        <button class="btn btn-color1">
                            Github
                        </button>
                    </a>
                    <a href="https://kongsak-shop-oa2r.onrender.com" target="_blank" rel="noopener noreferrer">
                        <button class="btn btn-color1">
                            Live Demo
                        </button>
                    </a>
                </div>
            </div>
            <div class="w-auto p-6 border border-gray-300 rounded-xl shadow-md bg-white/72 text-center mb-4 lg:text-center">
                <img src="../assets/parnwad_shop.png">
                <div class="font-bold text-2xl my-4">PARNWAD SHOP</div>
                <div class="flex justify-center gap-2">
                    <a href="https://github.com/ParnwadKonthong/ecommerce-react-client" target="_blank" rel="noopener noreferrer">
                        <button class="btn btn-color2">
                            Github
                        </button>
                    </a>
                    <a href="https://ecommerce-react-client.onrender.com" target="_blank" rel="noopener noreferrer">
                        <button class="btn btn-color2">
                            Live Demo
                        </button>
                    </a>
                </div>
            </div>
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
.btn-color1 {
  margin: 0;
  background: linear-gradient(
    135deg, 
    #a8e6cf,  
    #87cefa
  );
}

.btn-color2 {
  margin: 0;
  background: linear-gradient(
    135deg, 
    #87cefa,  
    #b39ddb
  );
}

</style>