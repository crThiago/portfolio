<template>
  <a class="social bg--white d--inline-flex" target="_blank" href="https://github.com/crThiago">
    <img src="~/assets/images/github.svg" alt="Icone do github">
  </a>
</template>

<style lang="scss">
.social {
  padding: 20px;
  border-radius: 50%;
  padding: 11px;
  border: 2px dotted;

  &:hover {
    & img {
      animation: spin 2s linear reverse infinite;
    }
    animation: spin 2s linear infinite;
  }
}

@-moz-keyframes spin { 100% { -moz-transform: rotate(360deg); } }
@-webkit-keyframes spin { 100% { -webkit-transform: rotate(360deg); } }
@keyframes spin { 100% { -webkit-transform: rotate(360deg); transform:rotate(360deg); } }
</style>
