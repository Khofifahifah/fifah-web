<script setup>
import ProfilePic from '@/components/Home/ProfilePic.vue';
</script>

<template>
  <header class="py-5">
    <div class="container px-5 pb-5">
      <div class="row gx-5 align-items-center">
        <div class="col-lg-5">
          <!-- Header text content-->
          <div class="text-center text-lg-start">
            <div class="mb-4">
              <div class="text-uppercase">
                Data Analyst &middot; Data Enthusiast
              </div>
            </div>
            <div class="fs-4 fw-light text-muted">Hello There!👋</div>
            <h1 class="display-4 fw-bolder mb-5">
              I'm <span class="text-gradient d-inline">Khofifah</span>
            </h1>
            <div
              class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xxl-start mb-3"
            >
              <div>
                <RouterLink
                  to="/resume"
                  class="btn btn-light btn-lg px-5 py-3 fs-6 fw-bolder"
                  >Resume</RouterLink
                >
              </div>
              <div>
                <button
                  @click="$emit('eventScroll')"
                  class="btn btn-outline-dark btn-lg px-4 py-3 fs-6 fw-bolder"
                >
                  About Me
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-7">
          <!-- Header profile picture-->
          <div class="d-flex justify-content-center mt-5 mt-xxl-0">
            <ProfilePic />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>
