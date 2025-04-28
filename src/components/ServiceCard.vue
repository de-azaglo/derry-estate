<template>
  <div class="card">
    <div class="icon">
      <slot name="icon"></slot>
    </div>
    <h2 class="title">
      <slot name="title"></slot>
    </h2>
    <p class="caption">
      <slot name="caption"></slot>
    </p>
  </div>
</template>

<style>
.card {
  background-color: white;
  width: 30vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 46vh;
  border-radius: 10px;
  padding: 25px;
}

.card:hover {
  background: linear-gradient(to bottom right, var(--vt-c-green), var(--vt-c-black));
}

.card:hover .icon {
  background-color: white;
}

.card:hover .title {
  color: white;
}
.card:hover .caption {
  color: white;
}

.icon {
  background-color: var(--vt-c-green);
  border-radius: 50%;
  padding: 6px 11px;
}

.title {
  color: var(--vt-c-green);
  font-weight: 700;
}

.caption {
  text-align: center;
  margin-top: 9px;
}
</style>
