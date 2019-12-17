<template>
  <div>
    <header>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      <nav>
        <g-link to="/">Home</g-link>
        <g-link to="/about/">About</g-link>
      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>