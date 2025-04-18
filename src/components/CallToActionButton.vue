<template>
    <div class="call-to-action-button">
        <button @click="">
            <slot name="title"></slot>
        </button>
    </div>
</template>

<style>
    .call-to-action-button button{
        border: none;
        border-radius: 10px;
        padding: 10px 12px;
        background-color: #fff;
        color: var(--vt-c-green);
        font-size: 1em;
    }
</style>