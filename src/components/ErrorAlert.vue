<template>
    <dialog open>
        <slot></slot>
    </dialog>
</template>

<style scoped>
dialog {
    position: fixed;
    top: 35vh;
    left: 25%;
    width: 40%;
    background-color: white;
    box-shadow: 0 2px 8px rgba(0,0,0,0.26);
}
</style>