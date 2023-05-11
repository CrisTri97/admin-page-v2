<template>
    <button
        class="app-button"
    >
      <slot></slot>
    </button>
</template>

<style >
  .app-button {
    position: relative;
    display: inline-flex;
    cursor: pointer;
    text-align: center;
    white-space: nowrap;
    align-items: center;
    justify-content: center;
    vertical-align: top;
    text-decoration: none;
    outline: none;
}
</style>