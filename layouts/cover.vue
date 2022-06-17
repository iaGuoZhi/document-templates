<template>
  <div class="slidev-layout cover">
    <img src="/logo.png" class="logo" />
    <div class="my-auto w-full">
      <slot />
    </div>
  </div>
</template>
<style lang="postcss">
.slidev-layout.cover {
  padding: 0;

  .logo {
    position: fixed;
    height: 3rem;
    right: 2rem;
    top: 1rem;
  }

  .my-auto {
    &,
    > div {
      height: 100%;

      h1 {
        height: 66%;
        display: flex;
        align-items: flex-end;

        background-color: #bf504d;
        color: #fff;
        font-weight: bold;
      }

      h1,
      p {
        padding-left: 3.5rem;
        padding-right: 3.5rem;
      }
      h1 {
        padding-bottom: 1.2rem;
      }
      p:first-of-type {
        padding-top: 1.5rem;
      }
    }
  }
}
</style>