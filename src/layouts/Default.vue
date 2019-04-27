<template>
  <div class="font-sans text-gray-800 leading-normal">
    <header class="border-t-14 border-blue">
      <!--<strong>-->
        <!--<g-link to="/">{{ $static.metaData.siteName }}</g-link>-->
      <!--</strong>-->
      <nav class="container mx-auto flex justify-between items-center py-8">
        <a href="/">Logo</a>
        <ul class="uppercase tracking-wide font-bold flex items-center">
           <li class="mr-8"><g-link class="nav__link text-gray-800 hover:text-gray-600" to="/">Home</g-link></li>
           <li class="mr-8"><g-link class="nav__link text-gray-800 hover:text-gray-600" to="/about">About</g-link></li>
        </ul>
      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style src="../main.css" />
