<script setup>
import { ref } from 'vue';

import AppMenuItem from './AppMenuItem.vue';

const model = ref([
    {
        label: 'Inicio',
        items: [{ label: 'BIENVENIDA', icon: 'pi pi-fw pi-home', to: '/' }]
    },
    {
        label: 'Catálogos',
        items: [
            { label: 'Almacén 1', to:'/uikit/formlayout' },
            { label: 'Almacén 2', to:'/uikit/input' },
            { label: 'Refrigeradores', to:'/uikit/floatlabel' },
            { label: 'Solventes', to: '/uikit/invalidstate' },
            
        ]
    },

]);
</script>

<template>
    <ul class="layout-menu">
        <template v-for="(item, i) in model" :key="item">
            <app-menu-item v-if="!item.separator" :item="item" :index="i"></app-menu-item>
            <li v-if="item.separator" class="menu-separator"></li>
        </template>
        <li>
            <a href="https://www.primefaces.org/primeblocks-vue/#/" target="_blank">
             
            </a>
        </li>
    </ul>
</template>

<style lang="scss" scoped></style>
