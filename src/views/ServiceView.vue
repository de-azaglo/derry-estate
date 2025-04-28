<script setup lang="ts">
import BuyHouseIcon from '@/components/icons/BuyHouseIcon.vue'
import HouseIcon from '@/components/icons/HouseIcon.vue'
import RentIcon from '@/components/icons/RentIcon.vue'
import ServiceCard from '@/components/ServiceCard.vue'
</script>

<template>
  <main class="services">
    <h1>Our Services</h1>
    <p>Derry Estate is ready to be a solution for you</p>
    <div class="card-container">
      <ServiceCard>
        <template #icon>
          <HouseIcon />
        </template>

        <template #title> New Property </template>

        <template #caption>
          Derry Estate will help you find new homes or ready-to-occupy houses with trusted
          facilities and affordable prices.
        </template>
      </ServiceCard>

      <ServiceCard>
        <template #icon>
          <RentIcon />
        </template>

        <template #title> Rent A House </template>

        <template #caption>
          Rent houses with various strategic facilities and locations for temporary occupancy.
        </template>
      </ServiceCard>
      <ServiceCard>
        <template #icon>
          <BuyHouseIcon />
        </template>

        <template #title> Rent A House </template>

        <template #caption>
          Rent houses with various strategic facilities and locations for temporary occupancy.
        </template>
      </ServiceCard>
    </div>
  </main>
</template>

<style>
@media (min-width: 1024px) {
  .services {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #f3fff4;
    width: 100%;
  }

  .services h1 {
    color: var(--vt-c-green);
    font-size: 4em;
    font-weight: 800;
  }

  .services p {
    color: black;
  }

  .card-container {
    display: flex;
    justify-content: space-around;
    width: 100%;
    margin-top: 8vh;
  }
}
</style>
