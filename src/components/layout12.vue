<template>
  <section class="py-10     flex flex-col justify-center items-center">
    <div class="flex flex-col md:flex-row justify-center items-center">
      <div class="w-full md:w-1/4 py-6 flex flex-col justify-center items-center space-y-8">
        <div class="img-right-section">
          <div class="inline-block img-container p-2 rounded bg-yellow-100">
            <img src="../assets/share.png" alt="share" width="25px" />
          </div>
        </div>
        <div class="text-section flex flex-col space-y-4  p-4 md-p-0">
            <h4 class="text-xl font-bold">Generate Ideas</h4>
            <p class="text-sm text-center">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. A, tenetur!
            </p>
        </div>
      </div>
      <div class="w-full md:w-1/4 py-6 flex flex-col justify-center items-center space-y-8">
        <div class="img-section">
          <div class="inline-block img-container p-2 rounded bg-purple-100">
            <img src="../assets/comment-alt.png" alt="share" width="25px" />
          </div>
        </div>
        <div class="text-section flex flex-col space-y-4 p-4 md-p-0">
            <h4 class="text-xl font-bold">Collect Contents</h4>
            <p class="text-sm text-center">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. A, tenetur!
            </p>
        </div>
      </div>
      <div class="w-full md:w-1/4 py-6 flex flex-col justify-center items-center space-y-8">
        <div class="img-section">
          <div class="inline-block img-container p-2 rounded bg-green-100">
            <img src="../assets/briefcase.png" alt="share" width="25px" />
          </div>
        </div>
        <div class="text-section flex flex-col space-y-4 p-4 md-p-0">
            <h4 class="text-xl font-bold">Create Design</h4>
            <p class="text-sm text-center">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. A, tenetur!
            </p>
        </div>
      </div>
      <div class="w-full md:w-1/4 py-6 flex flex-col justify-center items-center space-y-8">
        <div class="img-left-section">
          <div class="inline-block img-container p-2 rounded bg-red-100">
            <img src="../assets/document.png" alt="share" width="25px" />
          </div>
        </div>
        <div class="text-section flex flex-col space-y-4 p-4 md-p-0">
            <h4 class="text-xl font-bold">Launch Project</h4>
            <p class="text-sm text-center">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. A, tenetur!
            </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.img-right-section, .img-left-section, .img-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  background-repeat: no-repeat;
  background-position: center;
  object-fit: cover;
}

.img-right-section {
  background-image: url('../assets/right-line.png');
}

.img-left-section {
  background-image: url('../assets/left-line.png');
}

.img-section {
  background-image: url('../assets/Line.png');
}

.text-section{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

@media (max-width: 991px) {
  .img-right-section, .img-left-section, .img-section {
    background-image: none;
  }
}
</style>