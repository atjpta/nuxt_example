<template>
  <div>
    <div class="bg-base-200 pt-1 text-xl">
      <div class="md:w-4/5 mx-auto flex justify-between">
        <nuxt-link to="/" class="btn btn-ghost"> wblogit </nuxt-link>
        <div class="">
          <div class="">
            <input
              type="text"
              placeholder="Search…"
              class="input md:w-96 w-20 input-bordered mx-1"
            />
            <button class="btn btn-square">
              <OtherVIcon icon="fa-solid fa-magnifying-glass" />
            </button>
          </div>
        </div>
        <div class="flex">
          <OtherVTheme2/>
          <OtherVAvatarDD />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { authStore } from '~~/stores/auth.store';

const useAuth = authStore();

</script>>


<style scoped>
.router-link-exact-active {
  color: white;
  background: rgb(120, 0, 255);
}
</style>