<template>
  
  <main>
    <Suspense>
      <template #default>

        <ProfileCard/>
      </template>
  <template #fallback>

    <UserCardSkeleton />
  </template>
    </Suspense>
     
 
    
  </main>
 
</template>

<script setup>
import ProfileCard from "./components/ProfileCard.vue"
import UserCardSkeleton from "./components/UserCardSkeleton.vue"

</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap");

*,
::before,
::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: "Mouse Memoirs", sans-serif;
}

main {
  width: 620px;
  margin: 0 auto;
  padding-top: 32px;
  display: flex;
  flex-direction: column;
  gap: 16px;
}
</style>